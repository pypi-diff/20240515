# Comparing `tmp/aiosseclient-0.1.2.tar.gz` & `tmp/aiosseclient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosseclient-0.1.2.tar", last modified: Thu Apr 18 16:45:04 2024, max compression
+gzip compressed data, was "aiosseclient-0.1.3.tar", last modified: Wed May 15 18:43:04 2024, max compression
```

## Comparing `aiosseclient-0.1.2.tar` & `aiosseclient-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       16 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:04.011905 aiosseclient-0.1.2/aiosseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/aiosseclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:43:04.720574 aiosseclient-0.1.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       16 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-15 18:43:04.720574 aiosseclient-0.1.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:43:04.720574 aiosseclient-0.1.3/aiosseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-15 18:43:04.000000 aiosseclient-0.1.3/aiosseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 18:43:04.000000 aiosseclient-0.1.3/aiosseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:43:04.000000 aiosseclient-0.1.3/aiosseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:43:04.000000 aiosseclient-0.1.3/aiosseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 18:43:04.000000 aiosseclient-0.1.3/aiosseclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/aiosseclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 18:43:04.720574 aiosseclient-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-05-15 18:42:56.000000 aiosseclient-0.1.3/setup.py
```

### Comparing `aiosseclient-0.1.2/LICENSE` & `aiosseclient-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosseclient-0.1.2/PKG-INFO` & `aiosseclient-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosseclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous Server Sent Event streams client.
 Home-page: https://github.com/ebraminio/aiosseclient
 Author: Ebrahim Byagowi
 Author-email: ebrahim@gnu.org
 License: Copyright (c) 2017 Ebrahim Byagowi
```

### Comparing `aiosseclient-0.1.2/README.md` & `aiosseclient-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aiosseclient-0.1.2/aiosseclient.egg-info/PKG-INFO` & `aiosseclient-0.1.3/aiosseclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosseclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous Server Sent Event streams client.
 Home-page: https://github.com/ebraminio/aiosseclient
 Author: Ebrahim Byagowi
 Author-email: ebrahim@gnu.org
 License: Copyright (c) 2017 Ebrahim Byagowi
```

### Comparing `aiosseclient-0.1.2/aiosseclient.py` & `aiosseclient-0.1.3/aiosseclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import logging
 from typing import (
     List,
     Optional,
     AsyncGenerator,
     Final,
+    Dict
 )
 import aiohttp
 
 # pylint: disable=too-many-arguments, dangerous-default-value, redefined-builtin
 
 _SSE_LINE_PATTERN: Final[re.Pattern] = re.compile('(?P<name>[^:]*):?( ?(?P<value>.*))?')
 _LOGGER = logging.getLogger(__name__)
@@ -98,15 +99,15 @@
 # pylint: disable=too-many-arguments, dangerous-default-value
 async def aiosseclient(
     url: str,
     last_id: Optional[str] = None,
     valid_http_codes: List[int] = [200, 301, 307],
     exit_events: List[str] = [],
     timeout_total: Optional[float] = None,
-    headers: Optional[dict[str, str]] = None,
+    headers: Optional[Dict[str, str]] = None,
 ) -> AsyncGenerator[Event, None]:
     '''Canonical API of the library'''
     if headers is None:
         headers = {}
     # The SSE spec requires making requests with Cache-Control: nocache
     headers['Cache-Control'] = 'no-cache'
```

### Comparing `aiosseclient-0.1.2/setup.py` & `aiosseclient-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf8') as f:
     readme = f.read()
 with open('LICENSE', 'r', encoding='utf8') as f:
     license_txt = f.read()
 
 setup(
     name='aiosseclient',
-    version='0.1.2',
+    version='0.1.3',
     description='Asynchronous Server Sent Event streams client.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Ebrahim Byagowi',
     author_email='ebrahim@gnu.org',
     url='https://github.com/ebraminio/aiosseclient',
     license=license_txt,
```

