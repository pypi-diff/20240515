# Comparing `tmp/catway-1.0.tar.gz` & `tmp/catway-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catway-1.0.tar", last modified: Thu May  2 17:30:20 2024, max compression
+gzip compressed data, was "catway-1.1.tar", last modified: Wed May 15 21:11:22 2024, max compression
```

## Comparing `catway-1.0.tar` & `catway-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:30:20.174554 catway-1.0/
--rw-rw-rw-   0        0        0     1080 2024-05-02 17:27:24.000000 catway-1.0/LICENSE
--rw-rw-rw-   0        0        0     1007 2024-05-02 17:30:20.172558 catway-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-05-02 17:27:24.000000 catway-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 17:30:20.124688 catway-1.0/catway/
--rw-rw-rw-   0        0        0     1363 2024-05-02 17:28:08.000000 catway-1.0/catway/__init__.py
--rw-rw-rw-   0        0        0     1249 2024-05-02 17:27:24.000000 catway-1.0/catway/async_session.py
--rw-rw-rw-   0        0        0     1517 2024-05-02 17:27:24.000000 catway-1.0/catway/asyncio.py
--rw-rw-rw-   0        0        0     1409 2024-05-02 17:27:24.000000 catway-1.0/catway/session.py
--rw-rw-rw-   0        0        0     3470 2024-05-02 17:27:24.000000 catway-1.0/catway/types.py
--rw-rw-rw-   0        0        0      614 2024-05-02 17:27:24.000000 catway-1.0/catway/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:30:20.170564 catway-1.0/catway.egg-info/
--rw-rw-rw-   0        0        0     1007 2024-05-02 17:30:19.000000 catway-1.0/catway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-02 17:30:20.000000 catway-1.0/catway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:30:19.000000 catway-1.0/catway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-02 17:30:19.000000 catway-1.0/catway.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 17:30:19.000000 catway-1.0/catway.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      575 2024-05-02 17:27:58.000000 catway-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 17:30:20.175550 catway-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 21:11:21.997552 catway-1.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-15 18:54:03.000000 catway-1.1/LICENSE
+-rw-rw-rw-   0        0        0      982 2024-05-15 21:11:21.995556 catway-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-15 18:54:03.000000 catway-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 21:11:21.931726 catway-1.1/catway/
+-rw-rw-rw-   0        0        0     1388 2024-05-15 21:07:33.000000 catway-1.1/catway/__init__.py
+-rw-rw-rw-   0        0        0     1249 2024-05-15 18:54:03.000000 catway-1.1/catway/async_session.py
+-rw-rw-rw-   0        0        0     1542 2024-05-15 21:07:24.000000 catway-1.1/catway/asyncio.py
+-rw-rw-rw-   0        0        0     1409 2024-05-15 18:54:03.000000 catway-1.1/catway/session.py
+-rw-rw-rw-   0        0        0     3383 2024-05-15 21:06:17.000000 catway-1.1/catway/types.py
+-rw-rw-rw-   0        0        0      614 2024-05-15 18:54:03.000000 catway-1.1/catway/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:11:21.993563 catway-1.1/catway.egg-info/
+-rw-rw-rw-   0        0        0      982 2024-05-15 21:11:21.000000 catway-1.1/catway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-15 21:11:21.000000 catway-1.1/catway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:11:21.000000 catway-1.1/catway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 21:11:21.000000 catway-1.1/catway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 21:11:21.000000 catway-1.1/catway.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2024-05-15 21:10:20.000000 catway-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:11:21.997552 catway-1.1/setup.cfg
```

### Comparing `catway-1.0/LICENSE` & `catway-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catway-1.0/PKG-INFO` & `catway-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: catway
-Version: 1.0
+Version: 1.1
 Summary: Create tempmail based on https://mail.catway.org :D
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/catway
 Project-URL: Issues, https://github.com/zaid5o5/catway/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: pydantic
 
 # Install :
 ```commandline
 pip install -U catway
 ```
 
 # How to use :
```

### Comparing `catway-1.0/catway/__init__.py` & `catway-1.1/catway/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from .session import make_request
 from .types import Mail, MailBox
 from .utils import ApiExeption
 
 from typing import List
 
+__all__ = ["CatMail"]
+
 class CatMail:
     def __init__(self, email: str) -> None:
         """
         Args:
             email (str): the email, example : test@catway.org
         """
         self.email = email
```

### Comparing `catway-1.0/catway/async_session.py` & `catway-1.1/catway/async_session.py`

 * *Files identical despite different names*

### Comparing `catway-1.0/catway/asyncio.py` & `catway-1.1/catway/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .async_session import process_request, session_manager
 from .types import Mail, MailBox
 from .utils import ApiExeption
 
 from typing import AsyncGenerator, Any
 
+__all__ = ["CatMail"]
+
 class CatMail:
     def __init__(self, email: str) -> None:
         """
         Args:
             email (str): the email, example : test@catway.org
         """
         self.email = email
```

### Comparing `catway-1.0/catway/session.py` & `catway-1.1/catway/session.py`

 * *Files identical despite different names*

### Comparing `catway-1.0/catway/types.py` & `catway-1.1/catway/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from pydantic import BaseModel
+from dataclasses import dataclass
 from datetime import datetime
-from typing_extensions import TypedDict
+from typing import TypedDict
 
 from .utils import convert_to_datetime, convert_to_str
 
-class Object(BaseModel):
-    def __str__(self: "Object"):
-        return self.model_dump_json(indent=4)
-
 class MailDict(TypedDict):
     id: "str"
     senderEmail: "str"
     senderName: "str"
     subject: "str"
     createdAt: "str"
     updatedAt: "str"
     expireAt: "str"
 
-class Mail(Object):
+@dataclass(repr=True)
+class Mail:
     id: str
     sender_email: "str"
     sender_name: "str"
     subject: "str"
     created_at: "datetime"
     updated_at: "datetime"
     expire_at: "datetime"
@@ -63,15 +60,16 @@
     senderName: "str"
     subject: "str"
     createdAt: "str"
     updatedAt: "str"
     expireAt: "str"
     mailboxOwner: "str"
 
-class MailBox(Object):
+@dataclass(repr=True)
+class MailBox:
     id: "str"
     html: "str"
     content: "str"
     sender_email: "str"
     sender_name: "str"
     subject: "str"
     created_at: "datetime"
```

### Comparing `catway-1.0/catway/utils.py` & `catway-1.1/catway/utils.py`

 * *Files identical despite different names*

### Comparing `catway-1.0/catway.egg-info/PKG-INFO` & `catway-1.1/catway.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: catway
-Version: 1.0
+Version: 1.1
 Summary: Create tempmail based on https://mail.catway.org :D
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/catway
 Project-URL: Issues, https://github.com/zaid5o5/catway/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: pydantic
 
 # Install :
 ```commandline
 pip install -U catway
 ```
 
 # How to use :
```

