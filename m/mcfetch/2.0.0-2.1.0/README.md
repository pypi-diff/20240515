# Comparing `tmp/mcfetch-2.0.0.tar.gz` & `tmp/mcfetch-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcfetch-2.0.0.tar", last modified: Mon Apr 22 00:40:41 2024, max compression
+gzip compressed data, was "mcfetch-2.1.0.tar", last modified: Wed May 15 02:56:21 2024, max compression
```

## Comparing `mcfetch-2.0.0.tar` & `mcfetch-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.113416 mcfetch-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 00:40:32.000000 mcfetch-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 00:40:41.109416 mcfetch-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-22 00:40:32.000000 mcfetch-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/mcfetch/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/asyncmcfetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/mcfetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/mcfetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:40:41.113416 mcfetch-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-22 00:40:32.000000 mcfetch-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_async_fetch_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_fetch_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:56:21.697809 mcfetch-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 02:56:17.000000 mcfetch-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-15 02:56:21.697809 mcfetch-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-15 02:56:17.000000 mcfetch-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:56:21.693809 mcfetch-2.1.0/mcfetch/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-15 02:56:17.000000 mcfetch-2.1.0/mcfetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-15 02:56:17.000000 mcfetch-2.1.0/mcfetch/asyncmcfetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 02:56:17.000000 mcfetch-2.1.0/mcfetch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-15 02:56:17.000000 mcfetch-2.1.0/mcfetch/mcfetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-15 02:56:17.000000 mcfetch-2.1.0/mcfetch/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:56:21.697809 mcfetch-2.1.0/mcfetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-15 02:56:21.000000 mcfetch-2.1.0/mcfetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-15 02:56:21.000000 mcfetch-2.1.0/mcfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:56:21.000000 mcfetch-2.1.0/mcfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 02:56:21.000000 mcfetch-2.1.0/mcfetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 02:56:21.000000 mcfetch-2.1.0/mcfetch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:56:21.697809 mcfetch-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-15 02:56:17.000000 mcfetch-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:56:21.697809 mcfetch-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:56:17.000000 mcfetch-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-15 02:56:17.000000 mcfetch-2.1.0/tests/test_async_fetch_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-15 02:56:17.000000 mcfetch-2.1.0/tests/test_fetch_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 02:56:17.000000 mcfetch-2.1.0/tests/test_tools.py
```

### Comparing `mcfetch-2.0.0/LICENSE` & `mcfetch-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcfetch-2.0.0/PKG-INFO` & `mcfetch-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mcfetch
-Version: 2.0.0
-Summary: Modified version of mcuuid - fetches Minecraftplayer information from the Mojang API
-Home-page: https://github.com/oDepleted/mcfetch
-Author: oDepleted
-Author-email: contact@statalytics.net
+Version: 2.1.0
+Summary: Modified version of mcuuid - fetches Minecraft player information from the Mojang API
+Home-page: https://github.com/Luciism/mcfetch
+Author: Lucism
+Author-email: contact@lucism.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.0.0
-Requires-Dist: aiohttp>=3.8.5
+Requires-Dist: aiohttp>=3.9.4
 Requires-Dist: aiohttp_client_cache>=0.8.1
 
 # MCFETCH
 
 Fetches Minecraft player information from the Mojang API
 
 ## Installation
```

### Comparing `mcfetch-2.0.0/README.md` & `mcfetch-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mcfetch-2.0.0/mcfetch/__init__.py` & `mcfetch-2.1.0/mcfetch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 that cleans up the code, updates it to be more modern and reliable,
 and fixes KeyErrors by using .get().
 
 To use this package, simply import it and create a
 `FetchPlayer` object with the player's name or UUID:
 
 ```python
-from mcfetch import FetchPlayer
+from mcfetch import Player
 
-player = FetchPlayer(name='Notch')
+player = Player(name='Notch')
 print(player.name)
 print(player.uuid)
 ```
 """
 
 name = "mcfetch"
 
-from .mcfetch import *
-from .asyncmcfetch import *
+from .asyncmcfetch import AsyncPlayer as AsyncPlayer
+from .exceptions import RequestFailedError as RequestFailedError
+from .mcfetch import Player as Player
 from .tools import *
 
 __all__ = [
     'mcfetch',
     'asyncmcfetch'
 ]
```

### Comparing `mcfetch-2.0.0/mcfetch/asyncmcfetch.py` & `mcfetch-2.1.0/mcfetch/asyncmcfetch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,45 @@
+import asyncio
 import json
 from base64 import b64decode
 
-from aiohttp import ClientSession
+from aiohttp import (
+    ClientError,
+    ClientSession,
+    ClientTimeout,
+    ContentTypeError,
+    StreamReader,
+)
 from aiohttp_client_cache import CacheBackend, CachedSession
 
+from .exceptions import RequestFailedError
+
 
 class AsyncPlayer:
     def __init__(
         self,
         player: str,
-        cache_backend: CacheBackend=None
-    ):
+        cache_backend: CacheBackend=None,
+        request_retries: int=3,
+        request_retry_delay: int=3,
+        request_timeout: int=4
+    ) -> None:
         """
         Initializes an AsyncPlayer object with a name or uuid.
 
         Args:
             player (str): The player's username or uuid.
-            cache_backend (class, optional): The backend used for caching
-            responses, if `None`, caching won't be used.
+            cache_backend (class, optional): The backend used for caching \
+                responses, if `None`, caching won't be used.
+            request_retries (int, optional): The amount of times to reattempt the \
+                request if failed.
+            request_retry_delay (int, optional): The delay (in seconds) to wait before \
+                retrying the request
+            request_timeout (int, optional): The amount of time to terminate the request \
+                after if no response is delivered.
 
         Raises:
             AssertionError: If both name and uuid are None or if both are not None.
         """
         self._uuid = None
         self._name = None
 
@@ -32,19 +50,22 @@
 
         self._pretty_name = None
 
         self._skin_url = None
         self._skin_texture = None
 
         self._player_exists = True
-
         self._has_loaded_by_uuid = False
 
         self.cache_backend = cache_backend
 
+        self._request_retries = request_retries
+        self._request_retry_delay = request_retry_delay
+        self._request_timeout = request_timeout
+
 
     @property
     async def name(self) -> str | None:
         """Returns the player's pretty name."""
         if self._pretty_name is None:
             if self._name is None:
                 await self._load_by_uuid()
@@ -73,48 +94,74 @@
     @property
     async def skin_texture(self) -> str | None:
         """Returns the player's skin texture image as bytes."""
         if self._skin_texture is None:
             skin_url = await self.skin_url
             if skin_url is None:
                 return None
-            texture = (await self._make_request(skin_url)).content
+            texture = await self._make_request_with_err_handling(skin_url)
             self._skin_texture = await texture.read()
 
         return self._skin_texture
 
 
     async def _make_request(self, url: str):
+        timeout = ClientTimeout(total=self._request_timeout)
+
         if self.cache_backend is None:
-            async with ClientSession() as session:
+            async with ClientSession(timeout=timeout) as session:
                 data = await session.get(url)
         else:
-            async with CachedSession(cache=self.cache_backend) as session:
+            async with CachedSession(
+                cache=self.cache_backend, timeout=timeout
+            ) as session:
                 data = await session.get(url)
         return data
 
 
+    async def _make_request_with_err_handling(
+        self,
+        url: str,
+        as_json: bool=False,
+        _attempt: int=1
+    ) -> dict | StreamReader:
+        try:
+            res = await self._make_request(url)
+            if as_json:
+                return await res.json()
+            return res.content
+        except (TimeoutError, ClientError, ContentTypeError) as exc:
+            if _attempt > self._request_retries:  # Max retries exceeded
+                raise RequestFailedError(exc) from exc
+
+            await asyncio.sleep(self._request_retry_delay)
+            return await self._make_request_with_err_handling(
+                url, as_json, _attempt=_attempt+1)
+
+
     async def _load_by_name(self):
         if self._uuid is None and self._player_exists:
-            data: dict = await (await self._make_request(
-                f"https://api.mojang.com/users/profiles/minecraft/{self._name}"
-            )).json()
+            data = await self._make_request_with_err_handling(
+                f"https://api.mojang.com/users/profiles/minecraft/{self._name}",
+                as_json=True
+            )
 
             self._uuid = data.get("id")
             self._pretty_name = data.get("name")
 
             if self._pretty_name is None:
                 self._player_exists = False
 
 
     async def _load_by_uuid(self):
         if (not self._has_loaded_by_uuid) and self._player_exists:
-            data: dict = await (await self._make_request(
-                f"https://sessionserver.mojang.com/session/minecraft/profile/{self._uuid}"
-            )).json()
+            data = await self._make_request_with_err_handling(
+                f"https://sessionserver.mojang.com/session/minecraft/profile/{self._uuid}",
+                as_json=True
+            )
 
             name = data.get("name")
 
             # Stops future requests
             if name is None:
                 self._player_exists = False
                 return
@@ -125,8 +172,8 @@
                 if item.get('name') == 'textures':
                     encoded_str = item.get('value', '')
                     textures: dict = json.loads(b64decode(encoded_str) or '{}')
 
                     self._skin_url = textures.get('textures', {}).get('SKIN', {}).get('url')
                     break
 
-            self._has_loaded_by_uuid == True
+            self._has_loaded_by_uuid = True
```

### Comparing `mcfetch-2.0.0/mcfetch/tools.py` & `mcfetch-2.1.0/mcfetch/tools.py`

 * *Files identical despite different names*

### Comparing `mcfetch-2.0.0/mcfetch.egg-info/PKG-INFO` & `mcfetch-2.1.0/mcfetch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mcfetch
-Version: 2.0.0
-Summary: Modified version of mcuuid - fetches Minecraftplayer information from the Mojang API
-Home-page: https://github.com/oDepleted/mcfetch
-Author: oDepleted
-Author-email: contact@statalytics.net
+Version: 2.1.0
+Summary: Modified version of mcuuid - fetches Minecraft player information from the Mojang API
+Home-page: https://github.com/Luciism/mcfetch
+Author: Lucism
+Author-email: contact@lucism.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.0.0
-Requires-Dist: aiohttp>=3.8.5
+Requires-Dist: aiohttp>=3.9.4
 Requires-Dist: aiohttp_client_cache>=0.8.1
 
 # MCFETCH
 
 Fetches Minecraft player information from the Mojang API
 
 ## Installation
```

### Comparing `mcfetch-2.0.0/setup.py` & `mcfetch-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mcfetch",
-    version="2.0.0",
-    author="oDepleted",
-    author_email="contact@statalytics.net",
-    description="Modified version of mcuuid - fetches Minecraft"
+    version="2.1.0",
+    author="Lucism",
+    author_email="contact@lucism.dev",
+    description="Modified version of mcuuid - fetches Minecraft "
                 "player information from the Mojang API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/oDepleted/mcfetch",
+    url="https://github.com/Luciism/mcfetch",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'requests>=2.0.0',
-        'aiohttp>=3.8.5',
+        'aiohttp>=3.9.4',
         'aiohttp_client_cache>=0.8.1'
-    ],
+    ]
 )
```

### Comparing `mcfetch-2.0.0/tests/test_async_fetch_player.py` & `mcfetch-2.1.0/tests/test_async_fetch_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 from aiohttp_client_cache import SQLiteBackend
-from mcfetch import AsyncPlayer
-from requests_cache import CachedSession
+from mcfetch import AsyncPlayer, RequestFailedError
 
 
 class _TestAsyncPlayerBase:
     def setup_method(self):
         self.existing_player: AsyncPlayer = \
             self.get_existing_player_instance()
```

### Comparing `mcfetch-2.0.0/tests/test_fetch_player.py` & `mcfetch-2.1.0/tests/test_fetch_player.py`

 * *Files identical despite different names*

### Comparing `mcfetch-2.0.0/tests/test_tools.py` & `mcfetch-2.1.0/tests/test_tools.py`

 * *Files identical despite different names*

