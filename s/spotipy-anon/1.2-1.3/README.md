# Comparing `tmp/spotipy_anon-1.2.tar.gz` & `tmp/spotipy_anon-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotipy_anon-1.2.tar", last modified: Wed May 10 09:53:12 2023, max compression
+gzip compressed data, was "spotipy_anon-1.3.tar", last modified: Wed May 15 11:40:07 2024, max compression
```

## Comparing `spotipy_anon-1.2.tar` & `spotipy_anon-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/
--rw-rw-rw-   0        0        0     1102 2023-05-10 09:23:29.000000 spotipy_anon-1.2/LICENSE
--rw-rw-rw-   0        0        0     1843 2023-05-10 09:53:12.447143 spotipy_anon-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-05-10 09:23:29.000000 spotipy_anon-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 09:53:12.447143 spotipy_anon-1.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-05-10 09:50:38.000000 spotipy_anon-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/spotipy_anon/
--rw-rw-rw-   0        0        0       56 2023-05-10 09:50:49.000000 spotipy_anon-1.2/spotipy_anon/__init__.py
--rw-rw-rw-   0        0        0     3991 2023-05-10 09:23:29.000000 spotipy_anon-1.2/spotipy_anon/oauth2.py
-drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/spotipy_anon.egg-info/
--rw-rw-rw-   0        0        0     1843 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:40:07.072856 spotipy_anon-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 11:40:04.000000 spotipy_anon-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-15 11:40:07.072856 spotipy_anon-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 11:40:04.000000 spotipy_anon-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:40:07.072856 spotipy_anon-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 11:40:04.000000 spotipy_anon-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:40:07.072856 spotipy_anon-1.3/spotipy_anon/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 11:40:04.000000 spotipy_anon-1.3/spotipy_anon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-15 11:40:04.000000 spotipy_anon-1.3/spotipy_anon/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:40:07.072856 spotipy_anon-1.3/spotipy_anon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-15 11:40:07.000000 spotipy_anon-1.3/spotipy_anon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 11:40:07.000000 spotipy_anon-1.3/spotipy_anon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:40:07.000000 spotipy_anon-1.3/spotipy_anon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 11:40:07.000000 spotipy_anon-1.3/spotipy_anon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 11:40:07.000000 spotipy_anon-1.3/spotipy_anon.egg-info/top_level.txt
```

### Comparing `spotipy_anon-1.2/LICENSE` & `spotipy_anon-1.3/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 dieser-niko (dieserniko)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 dieser-niko (dieserniko)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `spotipy_anon-1.2/setup.py` & `spotipy_anon-1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup
-
-with open("README.md", "r") as f:
-    long_description = f.read()
-
-
-
-setup(
-    name='spotipy_anon',
-    version='1.2',
-    description='An extension to Spotipy for anonymous access to the Spotify Web API',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="@dieserniko",
-    author_email="dieserniko@gmx.de",
-    url='https://github.com/dieser-niko/spotipy-anon',
-    project_urls={
-        'Source': 'https://github.com/dieserniko/spotipy-anon',
-    },
-    install_requires=["spotipy>=2.23.0"],
-    license='MIT',
-    packages=['spotipy_anon'])
+from setuptools import setup
+
+with open("README.md", "r") as f:
+    long_description = f.read()
+
+
+
+setup(
+    name='spotipy_anon',
+    version='1.3',
+    description='An extension to Spotipy for anonymous access to the Spotify Web API',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="@dieserniko",
+    author_email="hello@dieserniko.link",
+    url='https://github.com/dieser-niko/spotipy-anon',
+    project_urls={
+        'Source': 'https://github.com/dieser-niko/spotipy-anon',
+    },
+    install_requires=["spotipy>=2.23.0"],
+    license='MIT',
+    packages=['spotipy_anon'])
```

### Comparing `spotipy_anon-1.2/spotipy_anon/oauth2.py` & `spotipy_anon-1.3/spotipy_anon/oauth2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# -*- coding: utf-8 -*-
-
-__all__ = ["SpotifyAnon"]
-
-
-import warnings
-import logging
-
-import requests
-from spotipy.oauth2 import SpotifyAuthBase
-from spotipy.cache_handler import CacheFileHandler, CacheHandler
-
-logger = logging.getLogger(__name__)
-
-
-class SpotifyAnon(SpotifyAuthBase):
-    """
-    Implements anonymous access to the Spotify API.
-    """
-    client_id: str  # was suggested by PyCharm
-
-    TOKEN_URL = "https://open.spotify.com/get_access_token"
-
-    def __init__(
-            self,
-            proxies=None,
-            requests_session=True,
-            requests_timeout=None,
-            cache_handler=None
-    ):
-        """
-        Creates a SpotifyAnon object
-        
-        Parameters:
-        * proxies: Optional, interpreted as boolean
-        * requests_session: A Requests session
-        * requests_timeout: Optional, tell Requests to stop waiting for a response after
-                            a given number of seconds
-        * cache_handler: An instance of the `CacheHandler` class to handle
-                         getting and saving cached authorization tokens.
-                         Optional, will otherwise use `CacheFileHandler`.
-                         (takes precedence over `cache_path` and `username`)
-        """
-
-        super(SpotifyAnon, self).__init__(requests_session)
-
-        self.proxies = proxies
-        self.requests_session = requests_session
-        self.requests_timeout = requests_timeout
-        self.cache_handler = cache_handler
-
-        if cache_handler:
-            assert issubclass(cache_handler.__class__, CacheHandler), \
-                "cache_handler must be a subclass of CacheHandler: " + str(type(cache_handler)) \
-                + " != " + str(CacheHandler)
-            self.cache_handler = cache_handler
-        else:
-            self.cache_handler = CacheFileHandler()
-
-    def get_access_token(self, as_dict=False, check_cache=True):
-        """
-        If a valid access token is in memory, returns it
-        Else fetches a new token and returns it
-            Parameters:
-            - as_dict - a boolean indicating if returning the access token
-                as a token_info dictionary, otherwise it will be returned
-                as a string.
-        """
-        if as_dict:
-            warnings.warn(
-                "You're using 'as_dict = True'."
-                "get_access_token will return the token string directly in future "
-                "versions. Please adjust your code accordingly, or use "
-                "get_cached_token instead.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-        if check_cache:
-            token_info = self.cache_handler.get_cached_token()
-            if token_info and not self.is_token_expired(token_info):
-                return token_info if as_dict else token_info["access_token"]
-
-        token_info = self._request_access_token()
-        self.cache_handler.save_token_to_cache(token_info)
-        self.client_id = token_info["client_id"]
-        return token_info if as_dict else token_info["access_token"]
-
-    def _request_access_token(self):
-        """Gets client credentials access token """
-        logger.debug("sending GET request to %s", self.TOKEN_URL)
-
-        try:
-            response = self._session.get(
-                self.TOKEN_URL,
-                verify=True,
-                proxies=self.proxies,
-                timeout=self.requests_timeout,
-            )
-            response.raise_for_status()
-            token_info = response.json()
-            return {"client_id": token_info["clientId"],
-                    "access_token": token_info["accessToken"],
-                    "expires_at": int(token_info["accessTokenExpirationTimestampMs"] / 1000)
-                    }
-        except requests.exceptions.HTTPError as http_error:
-            self._handle_oauth_error(http_error)
+# -*- coding: utf-8 -*-
+
+__all__ = ["SpotifyAnon"]
+
+
+import warnings
+import logging
+
+import requests
+from spotipy.oauth2 import SpotifyAuthBase
+from spotipy.cache_handler import MemoryCacheHandler, CacheHandler
+
+logger = logging.getLogger(__name__)
+
+
+class SpotifyAnon(SpotifyAuthBase):
+    """
+    Implements anonymous access to the Spotify API.
+    """
+    client_id: str  # was suggested by PyCharm
+
+    TOKEN_URL = "https://open.spotify.com/get_access_token"
+
+    def __init__(
+            self,
+            proxies=None,
+            requests_session=True,
+            requests_timeout=None,
+            cache_handler=None
+    ):
+        """
+        Creates a SpotifyAnon object
+        
+        Parameters:
+        * proxies: Optional, interpreted as boolean
+        * requests_session: A Requests session
+        * requests_timeout: Optional, tell Requests to stop waiting for a response after
+                            a given number of seconds
+        * cache_handler: An instance of the `CacheHandler` class to handle
+                         getting and saving cached authorization tokens.
+                         Optional, will otherwise use `CacheFileHandler`.
+                         (takes precedence over `cache_path` and `username`)
+        """
+
+        super(SpotifyAnon, self).__init__(requests_session)
+
+        self.proxies = proxies
+        self.requests_session = requests_session
+        self.requests_timeout = requests_timeout
+        self.cache_handler = cache_handler
+
+        if cache_handler:
+            assert issubclass(cache_handler.__class__, CacheHandler), \
+                "cache_handler must be a subclass of CacheHandler: " + str(type(cache_handler)) \
+                + " != " + str(CacheHandler)
+            self.cache_handler = cache_handler
+        else:
+            self.cache_handler = MemoryCacheHandler()
+
+    def get_access_token(self, as_dict=False, check_cache=True):
+        """
+        If a valid access token is in memory, returns it
+        Else fetches a new token and returns it
+            Parameters:
+            - as_dict - a boolean indicating if returning the access token
+                as a token_info dictionary, otherwise it will be returned
+                as a string.
+        """
+        if as_dict:
+            warnings.warn(
+                "You're using 'as_dict = True'."
+                "get_access_token will return the token string directly in future "
+                "versions. Please adjust your code accordingly, or use "
+                "get_cached_token instead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
+        if check_cache:
+            token_info = self.cache_handler.get_cached_token()
+            if token_info and not self.is_token_expired(token_info):
+                return token_info if as_dict else token_info["access_token"]
+
+        token_info = self._request_access_token()
+        self.cache_handler.save_token_to_cache(token_info)
+        self.client_id = token_info["client_id"]
+        return token_info if as_dict else token_info["access_token"]
+
+    def _request_access_token(self):
+        """Gets client credentials access token """
+        logger.debug("sending GET request to %s", self.TOKEN_URL)
+
+        try:
+            response = self._session.get(
+                self.TOKEN_URL,
+                verify=True,
+                proxies=self.proxies,
+                timeout=self.requests_timeout,
+            )
+            response.raise_for_status()
+            token_info = response.json()
+            return {"client_id": token_info["clientId"],
+                    "access_token": token_info["accessToken"],
+                    "expires_at": int(token_info["accessTokenExpirationTimestampMs"] / 1000)
+                    }
+        except requests.exceptions.HTTPError as http_error:
+            self._handle_oauth_error(http_error)
```

