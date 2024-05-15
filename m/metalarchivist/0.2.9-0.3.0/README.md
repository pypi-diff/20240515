# Comparing `tmp/metalarchivist-0.2.9.tar.gz` & `tmp/metalarchivist-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.2.9.tar", last modified: Fri Apr 26 14:15:07 2024, max compression
+gzip compressed data, was "metalarchivist-0.3.0.tar", last modified: Wed May 15 16:44:42 2024, max compression
```

## Comparing `metalarchivist-0.2.9.tar` & `metalarchivist-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.668043 metalarchivist-0.2.9/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-26 14:15:07.667043 metalarchivist-0.2.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 14:15:07.668043 metalarchivist-0.2.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.659043 metalarchivist-0.2.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.660043 metalarchivist-0.2.9/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.664043 metalarchivist-0.2.9/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4170 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     4193 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/label.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/user-agents.json
--rwxrwxrwx   0 root         (0) root         (0)     5625 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.666043 metalarchivist-0.2.9/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)      909 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/album.py
--rwxrwxrwx   0 root         (0) root         (0)     8342 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/label.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/page.py
--rwxrwxrwx   0 root         (0) root         (0)      372 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     6386 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3337 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.667043 metalarchivist-0.2.9/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 14:15:07.000000 metalarchivist-0.2.9/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:15:07.666043 metalarchivist-0.2.9/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10014 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5079 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8412 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     3059 2024-04-26 14:14:53.000000 metalarchivist-0.2.9/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.618732 metalarchivist-0.3.0/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 16:44:42.618732 metalarchivist-0.3.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 16:44:42.618732 metalarchivist-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.609732 metalarchivist-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.610732 metalarchivist-0.3.0/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.613732 metalarchivist-0.3.0/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.614732 metalarchivist-0.3.0/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.616732 metalarchivist-0.3.0/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6842 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.616732 metalarchivist-0.3.0/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3092 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8469 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.617732 metalarchivist-0.3.0/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 16:44:42.000000 metalarchivist-0.3.0/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-15 16:44:42.000000 metalarchivist-0.3.0/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 16:44:42.000000 metalarchivist-0.3.0/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 16:44:42.000000 metalarchivist-0.3.0/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-15 16:44:42.000000 metalarchivist-0.3.0/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 16:44:42.617732 metalarchivist-0.3.0/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     4731 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-15 16:44:28.000000 metalarchivist-0.3.0/src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.9/LICENSE` & `metalarchivist-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.9/PKG-INFO` & `metalarchivist-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.9/pyproject.toml` & `metalarchivist-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.2.9"
+version = "0.3.0"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/export/album.py` & `metalarchivist-0.3.0/src/metalarchivist/export/album.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 # standard
-import json
 import time
 import calendar
 import concurrent.futures
 from datetime import datetime
 
 # third-party
 import urllib3
@@ -26,27 +25,28 @@
 
     @staticmethod
     def get_profile(profile_url: str) -> AlbumProfile:
         response = perform_request(MetalArchives.get_page, AlbumError, profile_url)
         return AlbumProfile(profile_url, response.data)
     
     @classmethod
-    def get_profiles(cls, profile_urls: list[str], segment_size=16) -> list[AlbumProfile]:
+    def get_profiles(cls, profile_urls: list[str], segment_size=16, wait=3.) -> list[AlbumProfile]:
         profiles = list()
         profile_urls_len = len(profile_urls)
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
 
             # don't throw them all in at once
             for segment_start in range(0, profile_urls_len + segment_size, segment_size):
                 segment_end = min(segment_start + segment_size, profile_urls_len)
 
                 # feed the beast
                 album_futures = (executor.submit(cls.get_profile, url) 
-                                 for url in profile_urls[segment_start:segment_end])
+                                 for url in profile_urls[segment_start:segment_end] 
+                                 if not time.sleep(wait))
 
                 # examine the remains
                 for future in concurrent.futures.as_completed(album_futures):
                     profile = future.result()
                     profiles.append(profile)
         
         return profiles
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/export/band.py` & `metalarchivist-0.3.0/src/metalarchivist/export/band.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,28 +21,17 @@
     @staticmethod
     def get_profile(profile_url: str, user_agent: str | None = None) -> BandProfile:
         response = perform_request(MetalArchives.get_page, BandError, profile_url, user_agent=user_agent)
         return BandProfile(profile_url, response.data)
     
     @staticmethod
     def get_profile_links(metallum_id: int, user_agent: str | None = None) -> BandExternalLinks:
-        links_url = MetalArchives.links_query(metallum_id)
+        links_url = MetalArchives.band_links_query(metallum_id)
         response = perform_request(MetalArchives.get_page, BandError, links_url, user_agent=user_agent)
         return BandExternalLinks(metallum_id, response.data)
-    
-    @staticmethod
-    def _get_profiles_thread(profile_url: str) -> BandProfile:
-        response = perform_request(MetalArchives.get_page, BandError, profile_url)
-        return BandProfile(profile_url, response.data)
-
-    @staticmethod
-    def _get_links_thread(metallum_id: int) -> BandExternalLinks:
-        links_url = MetalArchives.links_query(metallum_id)
-        response = perform_request(MetalArchives.get_page, BandError, links_url)
-        return BandExternalLinks(metallum_id, response.data)
 
     @classmethod
     def get_profiles(cls, profile_urls: list[str], segment_size=8, wait=3.) -> list[BandProfile]:
 
         profile_urls_len = len(profile_urls)
         profiles = list()
         
@@ -56,28 +45,28 @@
             # don't throw them all in at once
             for segment_start in range(0, profile_urls_len + segment_size, segment_size):
                 segment_end = min(segment_start + segment_size, profile_urls_len)
 
                 band_futures = list()
                 for url in profile_urls[segment_start:segment_end]:
                     if url not in processed_urls:
-                        future = executor.submit(cls._get_profiles_thread, url)
+                        future = executor.submit(cls.get_profile, url)
                         band_futures.append(future)
                         processed_urls.add(url)
                         time.sleep(wait)
 
                 # examine the remains
                 for future in concurrent.futures.as_completed(band_futures):
                     profile = future.result()
                     profiles.append(profile)
 
         return profiles
     
     @classmethod
-    def get_profiles_links(cls, metallum_ids: list[int], segment_size=8, wait=3.) -> list[BandExternalLinks]:
+    def get_external_links(cls, metallum_ids: list[int], segment_size=8, wait=3.) -> list[BandExternalLinks]:
 
         links = list()
         metallum_ids_count = len(metallum_ids)
 
         if metallum_ids_count == 0:
             return links
 
@@ -88,15 +77,15 @@
             # don't throw them all in at once
             for segment_start in range(0, metallum_ids_count + segment_size, segment_size):
                 segment_end = min(segment_start + segment_size, metallum_ids_count)
 
                 band_futures = list()
                 for url in metallum_ids[segment_start:segment_end]:
                     if url not in processed_urls:
-                        future = executor.submit(cls._get_links_thread, url)
+                        future = executor.submit(cls.get_profile_links, url)
                         band_futures.append(future)
                         processed_urls.add(url)
                         time.sleep(wait)
 
                 # examine the remains
                 for future in concurrent.futures.as_completed(band_futures):
                     profile = future.result()
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/export/genre.py` & `metalarchivist-0.3.0/src/metalarchivist/export/genre.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 if attempt == MAX_ATTEMPTS:
                     raise MetalArchivesInternalError(**kwargs)
                 else:
                     time.sleep(30)
                     attempt += 1
                     continue
 
-            genre_bands = GenrePage(metadata=genre_page_metadata, **kwargs)
+            genre_bands = GenrePage(**kwargs, metadata=genre_page_metadata)
             
             data.append(genre_bands)
 
             record_cursor += genre_bands.count
             echo += 1
             
             if genre_bands.total_records == record_cursor:
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/export/user-agents.json` & `metalarchivist-0.3.0/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.2.9/src/metalarchivist/export/util.py` & `metalarchivist-0.3.0/src/metalarchivist/export/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import random
 import warnings
 from datetime import datetime
 from urllib.parse import urlencode
 from typing import Callable
 
 import urllib3
+from urllib3 import BaseHTTPResponse
 
 
 MAX_ATTEMPTS = 3
+ERROR_SLEEP_SECS = 30
 
 
 def normalize_keyword_casing(dictionary: dict):
     def normalize_to_snakecase(match: re.Match):
         preceding_text = match.group(1)
         text = match.group(2).lower()
 
@@ -49,15 +51,15 @@
             setattr(self, key, value)
 
 
 class JSONError(MetalArchivesError):
     ...
 
 
-def perform_request(func: Callable[..., urllib3.BaseHTTPResponse], error, *args, **kwargs) -> urllib3.BaseHTTPResponse:
+def perform_request(func: Callable[..., BaseHTTPResponse], error, *args, **kwargs) -> BaseHTTPResponse:
     attempt = 0
     
     while True:
         attempt += 1
         response = func(*args, **kwargs)
         status_code = response.status
 
@@ -98,15 +100,15 @@
 
 
 class Constant:
     ERROR_PLACEHOLDER = '«error»'
 
 
 class UserAgent:
-    user_agent_path = os.path.join(os.path.dirname(__file__), 'user-agents.json')
+    user_agent_path = os.path.join(os.path.dirname(__file__), 'data/user-agents.json')
 
     @classmethod
     def load(cls) -> list[str]:
         with open(cls.user_agent_path, 'r') as ua_file:
             user_agents = json.load(ua_file)
 
         return [record['ua'] for record in user_agents]
@@ -116,18 +118,28 @@
         if randomize:
             return random.choice(cls.load())
         
         return 'metalarchivist'
 
 
 class MetalArchives:
+    ROSTER_CURRENT_PAGE_SIZE = 1000
+    ROSTER_PAST_PAGE_SIZE = 1000
+    LABEL_RELEASES_PAGE_SIZE = 2500
+
     ROOT = 'https://www.metal-archives.com'
-    SEARCH = 'https://www.metal-archives.com/search/advanced/searching/bands'
-    BAND_LINKS = 'https://www.metal-archives.com/link/ajax-list/type/band/id'
-    LABEL = 'https://www.metal-archives.com/label/ajax-list/json/1/l/'
+    SEARCH = f'{ROOT}/search/advanced/searching/bands'
+    
+    BAND_LINKS = f'{ROOT}/link/ajax-list/type/band/id'
+    
+    LABEL = f'{ROOT}/label/ajax-list/json/1/l/'
+    LABEL_LINKS = f'{ROOT}/link/ajax-list/type/label/id/'
+    ROSTER_CURRENT = f'{ROOT}/label/ajax-bands/nbrPerPage/{ROSTER_CURRENT_PAGE_SIZE}/id/'
+    ROSTER_PAST = f'{ROOT}/label/ajax-bands-past/nbrPerPage/{ROSTER_PAST_PAGE_SIZE}/id/'
+    LABEL_RELEASES = f'{ROOT}/label/ajax-albums/nbrPerPage/{LABEL_RELEASES_PAGE_SIZE}/id/'
 
     @classmethod
     def get_page(cls, url: str, user_agent: str | None = None, 
                  retries: int | None = None, 
                  timeout: urllib3.Timeout | None = None):
         
         if user_agent is None:
@@ -168,9 +180,28 @@
                         'yearCreationFrom': year_from, 'yearCreationTo': year_to}
         
         query_str = urlencode({k: v for k, v in query_params.items() if v is not None})
 
         return query_str
     
     @classmethod
-    def links_query(cls, metallum_id: int) -> str:
-        return os.path.join(cls.BAND_LINKS, str(metallum_id))
+    def band_links_query(cls, metallum_id: int) -> str:
+        return os.path.join(cls.BAND_LINKS, str(metallum_id))
+    
+    @classmethod
+    def label_links_query(cls, metallum_id: int) -> str:
+        return os.path.join(cls.LABEL_LINKS, str(metallum_id))
+    
+    @classmethod
+    def roster_current_query(cls, metallum_id: int, echo=0, display_start=0, display_length=100) -> str:
+        return (f'{os.path.join(cls.ROSTER_CURRENT, str(metallum_id))}'
+                f'?sEcho={echo}&iDisplayStart={display_start}&iDisplayLength={display_length}')
+    
+    @classmethod
+    def roster_past_query(cls, metallum_id: int, echo=0, display_start=0, display_length=100) -> str:
+        return (f'{os.path.join(cls.ROSTER_PAST, str(metallum_id))}'
+                f'?sEcho={echo}&iDisplayStart={display_start}&iDisplayLength={display_length}')
+    
+    @classmethod
+    def label_releases_query(cls, metallum_id: int, echo=0, display_start=0, display_length=100) -> str:
+        return (f'{os.path.join(cls.LABEL_RELEASES, str(metallum_id))}'
+                f'?sEcho={echo}&iDisplayStart={display_start}&iDisplayLength={display_length}')
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/interface/album.py` & `metalarchivist-0.3.0/src/metalarchivist/interface/album.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from dataclasses import dataclass, field, InitVar, asdict
 
 import lxml.etree
 import lxml.html
 
 from .band import BandLink
-
+from .genre import Subgenres
 
 
 class ParseError(Exception):
     ...
 
 
 def _parse_release_date(release_date) -> str:
@@ -52,14 +52,38 @@
     def __init__(self, html: str):
         html_anchor = lxml.html.fragment_fromstring(html)
         self.name = html_anchor.text
         self.link = html_anchor.attrib['href']
 
 
 @dataclass
+class AlbumRelease:    
+    band: BandLink
+    album: AlbumLink
+
+    release_type: str
+    genres: Subgenres
+    release_date_display: InitVar[str]
+    added_date_display: InitVar[str | None] = field(default=None)
+
+    release_date: str = field(init=False)
+    added_date: str | None = field(init=False)
+
+    def __post_init__(self, release_date_display, added_date_display):
+        self.release_date = _parse_release_date(release_date_display)
+
+        if added_date_display == 'N/A' or added_date_display is None:
+            self.added_date = None
+        else:
+            added_date = re.sub(r'\/(\d)\/', '/0\1/', added_date_display)
+            self.added_date = datetime.strptime(added_date, '%Y-%m-%d %H:%M:%S') \
+                                      .strftime('%Y-%m-%dT%H:%M:%SZ')
+
+
+@dataclass
 class AlbumTrackLength:
     """ Numerically defines the length of an album track """
     length_text: InitVar[str]
     hours: int = field(init=False, default=0)
     minutes: int = field(init=False, default=0)
     seconds: int = field(init=False)
 
@@ -176,10 +200,9 @@
 
         return key
     
     @property
     def release_date(self):
         return _parse_release_date(self.description.release_date)
     
-    
-    def to_json(self):
+    def to_dict(self):
         return asdict(self)
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/interface/band.py` & `metalarchivist-0.3.0/src/metalarchivist/interface/band.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 
 import re
-import struct
 
 from dataclasses import dataclass, field, asdict, InitVar
 from urllib.parse import unquote
 
 import lxml.html
 import lxml.etree
 
-from Crypto.Hash import BLAKE2s
-
 from .genre import Subgenres
 from .theme import Themes
+from .api.base import create_key
 
 
 
 class InvalidAttributeError(Exception):
     ...
 
 
 class InvalidPageError(Exception):
     ...
 
 
-def create_band_key(metallum_id: int, band_name: str) -> str:
-    metallum_id_bytes = struct.pack('>Q', metallum_id)
-    hash_obj = BLAKE2s.new(data=band_name.encode('utf-8'), digest_bytes=12, key=metallum_id_bytes)
-    return hash_obj.hexdigest()
-
-
 @dataclass
 class BandLink:
     """ An HTML anchor tag pointing to a unique band profile """
     name: str = field(init=False)
     link: str = field(init=False)
     metallum_id: int = field(init=False)
     band_key: str = field(init=False)
 
     def __init__(self, html: str):
         html_anchor = lxml.html.fragment_fromstring(html)
         self.name = name = html_anchor.text
         self.link = link = html_anchor.attrib['href']
         self.metallum_id = metallum_id = int(link.split('/')[-1])
 
-        self.band_key = create_band_key(metallum_id, name)
+        self.band_key = create_key(metallum_id, name)
+
+
+@dataclass
+class BandGenre:
+    profile_url: InitVar[str]
+    band_key: str = field(init=False)
+    metallum_id: int = field(init=False)
+    band: str
+    subgenre: Subgenres
+    genre: str
+
+    def __post_init__(self, profile_url: str):
+        metallum_id = profile_url.split('/')[-1]
+        self.metallum_id = int(metallum_id)
+        self.band_key = create_key(self.metallum_id, self.band)
 
 
 @dataclass(frozen=True)
 class BandMember:
     """ A member of a band """
+
     alias: str
     role: str
     profile: str = field(hash=True)
 
 
 @dataclass(frozen=True)
 class BandDescription:
     """ Additional information pertaining to a unique band """
+
     country_of_origin: str = field(kw_only=True)
     location: str = field(kw_only=True)
     status: str = field(kw_only=True)
     formed_in: str = field(kw_only=True)
     genre: str = field(kw_only=True)
     themes: str | None = field(kw_only=True, default=None)
     lyrical_themes: str | None = field(kw_only=True, default=None)
@@ -69,14 +78,15 @@
     current_label: str | None = field(kw_only=True, default=None)
 
 
 
 @dataclass
 class BandExternalLink:
     """ An HTML anchor tag pointing to a band's profile outside of metal-archives.com """
+
     name: str
     url: str
 
 
 @dataclass
 class BandExternalLinks:
     """ A collection of profiles pertaining to a single band, defined by metallum_id """
@@ -107,14 +117,15 @@
     name: str
     members: list[BandMember]
 
 
 @dataclass
 class BandProfile:
     """ A unique band's profile page """
+
     url: str
     html: InitVar[bytes]
     
     name: str = field(init=False)
     metallum_id: int = field(init=False)
     lineup: list[BandLineupCategory] = field(init=False)
     description: BandDescription = field(init=False)
@@ -136,15 +147,15 @@
                 band_name: list = profile_document.xpath(profile_band_name_xpath)
 
             self.name = name = band_name.pop()
 
         except IndexError:
             raise InvalidPageError(f'unable to parse band name from {self.url}')
         
-        self.band_key = create_band_key(metallum_id, name)
+        self.band_key = create_key(metallum_id, name)
 
         lineup = self._parse_lineup(profile_document)
         if len(lineup) == 0:
             lineup = self._parse_lineup(profile_document, all_members=False)
         
         self.lineup = lineup
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/interface/base.py` & `metalarchivist-0.3.0/src/metalarchivist/interface/api/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 
+import struct
+
 from abc import ABC
 from dataclasses import dataclass, field, InitVar, asdict
-from typing import ClassVar
+from typing import ClassVar, Any
+
+from Crypto.Hash import BLAKE2s
+
+
+def create_key(metallum_id: int, name: str) -> str:
+    metallum_id_bytes = struct.pack('>Q', metallum_id)
+    hash_obj = BLAKE2s.new(data=name.encode('utf-8'), digest_bytes=12, key=metallum_id_bytes)
+    return hash_obj.hexdigest()
 
 
 @dataclass
 class PageDataType(ABC):
     ...
 
 
@@ -16,15 +26,15 @@
     i_total_records: InitVar[int] = field(kw_only=True)
     i_total_display_records: InitVar[int] = field(kw_only=True)
     s_echo: InitVar[int] = field(kw_only=True)
     aa_data: InitVar[list] = field(kw_only=True)
     
     error: str | None = field(kw_only=True, default=None)
 
-    metadata: dict = field(default_factory=dict, kw_only=True)
+    metadata: dict[str, Any] = field(default_factory=dict, kw_only=True)
 
     total_records: int = field(init=False) 
     total_display_records: int = field(init=False)
     echo: int = field(init=False)
     count: int = field(init=False)
     _data: list[PageDataType] = field(init=False)
     _error: str = field(init=False)
@@ -56,27 +66,35 @@
     def _process(self, record: list[str]) -> list[PageDataType]:
         return [self.data_type(record, **self.metadata)]
     
     @property
     def data(self):
         unioned_data = list()
         for page_data in self._data:
-            unioned_data += page_data
+            if isinstance(page_data, list):
+                unioned_data += page_data
+            else:
+                raise ValueError(f'data type {type(page_data)} cannot be combined with list')
 
         return unioned_data
     
     def to_json(self):
         return list(map(asdict, self.data))
 
 
-class Pages(ABC, list):
+class PageCollection(ABC, list):
     data_type = Page
 
-    def combine(self) -> data_type:
+    def combine(self):
+        data_type = self.data_type
+
         first_page, *remaining = self
-        for page in remaining:
-            first_page += page
-        return first_page
+        if isinstance(first_page, data_type):
+            for page in remaining:
+                first_page += page
+            return first_page
+        else:
+            raise ValueError(f'data type {data_type} does not match {type(first_page)}')
     
     def __init_subclass__(cls, /, data_type, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.data_type = data_type
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/interface/genre.py` & `metalarchivist-0.3.0/src/metalarchivist/interface/genre.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
                      r'\bpowerviolence\b': r'Powerviolence Hardcore',
                      r'\bdrum and bass\b': r'Drum-and-Bass Electronic',
                      r'\bprog\b': r'Progressive',
                      r'\bpost-black\b': r'Post-Metal Black',
                      r'\bblackened\b': r'Black',
                      r'\bcore\b': r'Hardcore',
                      r'\brac\b': r'Rock-Against-Communism',
+                     r'\braс\b': r'Rock-Against-Communism',
                      r'\baor\b': r'Arena-Rock'}
 
 
 @dataclass
 class Subgenres:
     """ Handle genres specified in text assuming 
         the conventions applied by metal-archives.com
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/interface/theme.py` & `metalarchivist-0.3.0/src/metalarchivist/interface/theme.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import re
 
 from enum import StrEnum, auto
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, asdict
 
 
 class ThemePeriod(StrEnum):
     EARLY = auto()
     MID = auto()
     LATER = auto()
     ALL = auto()
@@ -18,45 +18,62 @@
     
     @classmethod
     def get(cls, value: str, default):
         try:
             return cls[value]
         except KeyError:
             return default
+        
+
+@dataclass(frozen=True)
+class Subtheme:
+    name: str
+
 
+ThemePhaseWithoutSubthemesType = tuple[str, ThemePeriod]
+ThemePhaseType = tuple[str, list[Subtheme], ThemePeriod]
 
-ThemePhaseType = tuple[str, list[str], ThemePeriod]
 
 @dataclass(frozen=True)
 class ThemePhase:
     name: str
-    subthemes: list[str] = field(default_factory=list)
+    subthemes: list[Subtheme] = field(default_factory=list)
     period: ThemePeriod = field(default=ThemePeriod.ALL)
 
 
 class ThemeRules:
-    subtheme_pattern = re.compile(r'\(([\w+, ]+)\)')
     phase_combos = ['early', 'mid', 'later', 'early/mid', 'early/later', 'mid/later']
 
-    junk = {r'\)[\/\b\w]': '), ',
+    subtheme_pattern = re.compile(r'\(([\w+,\/\. ]+)\)\s?')
+    subtheme_delimiter_pattern = re.compile(r'(?:,\s|\s\/\s)')
+    phase_pattern = re.compile(fr'^(?P<name>.*?)(\((?P<period>{"(" + "|".join(phase_combos) + ")"})\))?$')
+
+    not_inside_parenthes_str = r'(?!(?:[^(]*\([^)]*\))*[^()]*\))\s*'
+
+    junk = {r'\banti\b(\w)': r'anti-\g<1>',
+            r'\)[\/\b\w]': '), ',
             r'\(earlier\)': '(early)',
             r'\(early, later\)': '(early/later)',
             r'\(early\), \b': '(early); ',
-            r'\(first album\),': '(early); ',
+            r'\(first album\), \b': '(early); ',
             r'\(later\), \b': '(later); ',
             r'\);$': ')',
             r'\(deb.\)': '',
             r'themes from ': '',
             r' themes': '',
             r'based on ': '',
             r' \(thematic\)': ''}
 
     substitutions = {r'\bw\.a\.r\.': 'White Aryan Resistance',
                      r'\bnational socialism\b': 'Nazism',
                      r'\bo9a': 'Order of Nine Angles'}
+    
+    @classmethod
+    def not_inside_parenthes_pattern(cls, delimiter: str) -> re.Pattern:
+        return re.compile(fr'{delimiter}' + cls.not_inside_parenthes_str)
 
 
 @dataclass
 class Themes:
     full_theme: str
     clean_theme: str = field(init=False)
     phases: list[ThemePhase] = field(init=False)
@@ -69,38 +86,37 @@
         for pattern, substitution in ThemeRules.substitutions.items():
             clean_theme = re.sub(pattern, substitution, clean_theme, flags=re.IGNORECASE)
 
         del pattern
         del substitution
 
         phases = clean_theme.split(';')
-        phases = list(map(self._parse_phase, map(str.lstrip, phases)))
+        phases = self._parse_phases(phases)
         phases = self._explode_phases_on_delimiter(phases, '/')
-        phases = self._explode_phases_on_delimiter(phases, ',')
-        phases = list(map(lambda n: self._parse_subthemes(*n), phases))
+        phases = self._explode_phases_on_delimiter(phases, ', (?=[A-Z0-9])')
+        phases = self._parse_subthemes(phases)
         phases = self._remove_duplicates(phases)
-        # phases = self._scrub_phases_of_junk(phases)
         self.phases = phases = list(map(lambda n: ThemePhase(*n), phases))
         
         sorted_themes = sorted(phases, key=self._phase_sort_key)
         clean_theme_list = list()
         for phase in sorted_themes:
             theme = phase.name
             if len(phase.subthemes) > 0:
-                theme = theme + f' ({", ".join(phase.subthemes)})'
+                theme = theme + f' ({", ".join(map(lambda n: n.name, phase.subthemes))})'
             try:
                 _ = clean_theme_list.index(theme)
             except ValueError:
                 clean_theme_list.append(theme)
 
         self.clean_theme = ', '.join(clean_theme_list)
 
     @staticmethod
     def _phase_sort_key(phase: ThemePhase):
-        return (ThemePeriod._member_names_.index(phase.period.name), phase.name)
+        return (ThemePeriod._member_names_.index(phase.period.name), phase.name.lower())
 
     @staticmethod
     def _collapse_recurrent_phases(phases: list[ThemePhase]) -> list[ThemePhase]:
         all_phases = set(map(lambda n: n.period, phases))
 
         phase_counts: dict[str, set[ThemePeriod]] = dict()
         for phase in phases:
@@ -112,18 +128,14 @@
         consistent_themes = set(theme for theme, phases in phase_counts.items() 
                                 if phases == all_phases)
         
         collapsed_phases = list(map(lambda n: ThemePhase(n), consistent_themes))
         collapsed_phases += list(filter(lambda p: p.name not in consistent_themes, phases))
 
         return collapsed_phases
-
-    @staticmethod
-    def _scrub_phases_of_junk(phases: list[ThemePhase]) -> list[ThemePhase]:
-        raise NotImplementedError
     
     @staticmethod
     def _remove_duplicates(phases: list[ThemePhaseType]) -> list[ThemePhaseType]:
         unique_phases = list()
         for phase in phases:
             
             phase_exists = False
@@ -141,39 +153,51 @@
 
         return unique_phases
 
     @staticmethod
     def _explode_phases_on_delimiter(phases: list[tuple[str, ThemePeriod]], delimiter: str) -> list[tuple[str, ThemePeriod]]:
         def explode(phase: tuple[str, ThemePeriod]) -> list[tuple[str, ThemePeriod]]:
             name, period = phase
-            return [(n.strip(), period) for n in re.split(fr'{delimiter}(?!(?:[^(]*\([^)]*\))*[^()]*\))\s*', name)]
+            not_inside_parenthes = ThemeRules.not_inside_parenthes_pattern(delimiter)
+            return [(n.strip(), period) for n in not_inside_parenthes.split(name)]
 
         return sum(list(map(explode, phases)), [])
     
     @staticmethod
-    def _parse_subthemes(phase: str, period: ThemePeriod) -> tuple[str, list[str], ThemePeriod]:
-        subtheme_pattern = ThemeRules.subtheme_pattern
-        subthemes_match = subtheme_pattern.search(phase)
-        subthemes = subthemes_match.group(1).split(', ') if subthemes_match else []
-
-        phase = subtheme_pattern.sub('', phase).rstrip()
-        return phase, subthemes, period
-    
-    @staticmethod
-    def _parse_phase(phase: str) -> tuple[str, ThemePeriod]:
-        phase_patterns = '(' + '|'.join(ThemeRules.phase_combos) + ')'
-        phase_match = re.compile(fr'^(?P<name>.*?)(\((?P<period>{phase_patterns})\))?$').match(phase)
-        if phase_match is None:
-            raise ValueError
-
-        period_text = phase_match.group('period')
-        if period_text is not None:
-            period = ThemePeriod.get(period_text.upper(), ThemePeriod.ERROR)
-        else:
-            period = ThemePeriod.ALL
+    def _parse_subthemes(phases: list[ThemePhaseWithoutSubthemesType]) -> list[ThemePhaseType]:
+        def parse(phase: str, period: ThemePeriod):
+            subtheme_pattern = ThemeRules.subtheme_pattern
 
-        phase_name = phase_match.group('name')
-        return phase_name, period
+            subtheme_match = subtheme_pattern.search(phase)
+            subthemes = ThemeRules.subtheme_delimiter_pattern.split(subtheme_match.group(1)) if subtheme_match else []
+
+            phase = subtheme_pattern.sub('', phase).rstrip()
+            return phase, list(map(Subtheme, subthemes)), period
+    
+        return list(map(lambda n: parse(*n), phases))
+    
+    @staticmethod
+    def _parse_phases(phases: list[str]) -> list[tuple[str, ThemePeriod]]:
+        
+        def parse(phase: str):
+            phase_match = ThemeRules.phase_pattern.match(phase)
+            if phase_match is None:
+                raise ValueError
+
+            period_text = phase_match.group('period')
+            if period_text is not None:
+                period = ThemePeriod.get(period_text.upper(), ThemePeriod.ERROR)
+            else:
+                period = ThemePeriod.ALL
+
+            phase_name = phase_match.group('name')
+            return phase_name, period
+        
+        return list(map(parse, map(str.lstrip, phases)))
 
     def to_dict(self) -> dict:
-        phases = [dict(name=p.name.lower(), period=p.period.value) for p in self.phases]
+        phases = [dict(name=p.name.lower(), 
+                       subthemes=[{k: v.lower() for k, v in asdict(s).items()} for s in p.subthemes], 
+                       period=p.period.value) 
+                  for p in self.phases]
+        
         return dict(theme=self.clean_theme.lower(), theme_phases=phases)
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist/report.py` & `metalarchivist-0.3.0/src/metalarchivist/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import string
 from datetime import datetime
 from dataclasses import asdict
 
-from .export import Band, Album, Genre
+from .export import Band, Album, Label
 
 Series = list[str | int | float]
-Record = dict[str, str | float | int | list]
+Record = dict[str, str | float | int | Series]
 Dataset = list[Record]
 
 
 def series(from_list, column) -> Series:
     return [[v for k, v in d.items() if k == column].pop() for d in from_list]
 
 
@@ -39,15 +40,15 @@
     band_profile = list(map(lambda n: n.to_dict(), band_profile))
     
     band_desc = expand(select(band_profile, 'description'), 'description')
     band_desc = drop(band_desc, 'genre', 'themes', 'lyrical_themes')
 
     band_ids = series(band_profile, 'metallum_id')
     band_ids = [int(band_id) for band_id in band_ids]
-    band_links = Band.get_profiles_links(band_ids, wait=wait)
+    band_links = Band.get_external_links(band_ids, wait=wait)
     band_links = list(map(asdict, band_links))
 
     genres = expand(select(band_profile, 'genres'), 'genres')
     themes = expand(select(band_profile, 'themes'), 'themes')
 
     band_profile = drop(band_profile, 'genres', 'themes',  'description')
     band_profile = join(band_profile, band_links, 'metallum_id')
@@ -84,9 +85,20 @@
     album_zip = zip(album, profile_urls, release)
 
     album = [dict(**a, **u, **r) for a, u, r in album_zip]
 
     return join(album, band, 'band_url')
 
 
+def get_labels() -> Dataset:
+    label = Label.get_labels_by_letters(*string.ascii_lowercase, page_size=1000)
+    label = map(lambda n: n.label.url, label.data)
+    label = map(Label.get_full_profile, label)
+    label = map(asdict, label)
+    label = list(label)
+
+    return label
+        
+
+
 def get_genres():
     ...
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.3.0/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.2.9
+Version: 0.3.0
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.2.9/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.3.0/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 src/metalarchivist.egg-info/requires.txt
 src/metalarchivist.egg-info/top_level.txt
 src/metalarchivist/export/__init__.py
 src/metalarchivist/export/album.py
 src/metalarchivist/export/band.py
 src/metalarchivist/export/genre.py
 src/metalarchivist/export/label.py
-src/metalarchivist/export/user-agents.json
 src/metalarchivist/export/util.py
+src/metalarchivist/export/data/user-agents.json
 src/metalarchivist/interface/__init__.py
 src/metalarchivist/interface/album.py
 src/metalarchivist/interface/band.py
-src/metalarchivist/interface/base.py
 src/metalarchivist/interface/genre.py
 src/metalarchivist/interface/label.py
-src/metalarchivist/interface/page.py
 src/metalarchivist/interface/search.py
 src/metalarchivist/interface/theme.py
+src/metalarchivist/interface/api/base.py
+src/metalarchivist/interface/api/page.py
 src/test/test_albums.py
 src/test/test_bands.py
 src/test/test_genres.py
+src/test/test_labels.py
 src/test/test_themes.py
```

### Comparing `metalarchivist-0.2.9/src/test/test_albums.py` & `metalarchivist-0.3.0/src/test/test_albums.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         album_release = data.pop()
         self.assertIsInstance(album_release, self.interface.AlbumRelease)
 
     def test_range(self):
 
         self.assertIn('Album', dir(self.export))
 
-        releases = self.export.Album.get_range(datetime(1990, 1, 1), datetime(1990, 1, 31), timeout_read=90.)
+        releases = self.export.Album.get_range(datetime(1990, 1, 1), datetime(1990, 1, 5), timeout_read=90.)
         self.assertIsNotNone(releases)
         self.assertIsInstance(releases, self.interface.ReleasePage)
 
         total_records = releases.total_records
         total_display_records = releases.total_display_records
         self.assertEqual(total_records, total_display_records)
 
@@ -232,15 +232,15 @@
 
     def test_album_profile(self):
         self.assertIn('Album', dir(self.export))
 
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Urfaust/Untergang/1161736')
         self.assertIsNotNone(album)
 
-        album_json = album.to_json()
+        album_json = album.to_dict()
         album_band_link = album_json['band']
 
         self.assertIn('band_key', album_band_link)
 
     def test_album_profiles(self):
 
         self.assertIn('Album', dir(self.export))
```

### Comparing `metalarchivist-0.2.9/src/test/test_bands.py` & `metalarchivist-0.3.0/src/test/test_bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return metalarchivist, interface, export, config
 
 
 class TestBands(unittest.TestCase):
     metalarchivist, interface, export, config = load_module()
 
     def test_band_hash(self):
-        band_hash = self.interface.create_band_key(1, 'Amorphis')
+        band_hash = self.interface.create_key(1, 'Amorphis')
         self.assertEqual(band_hash, '6bdefdd6445b150526b32308')
 
     def test_band_report(self):
 
         bands = self.metalarchivist.get_bands(['https://www.metal-archives.com/bands/Furia/23765',
                                                'https://www.metal-archives.com/bands/Cult_of_Fire/3540334368',
                                                'https://www.metal-archives.com/bands/Urfaust/19596',
@@ -102,17 +102,14 @@
         self.assertIn('Spotify', link_names)
         self.assertIn('Tidal', link_names)
         self.assertIn('Amazon', link_names)
         self.assertIn('Apple Music', link_names)
         self.assertIn('BigCartel', link_names)
         self.assertIn(b'V\xc3\x83\xc2\xa1n Records'.decode(), link_names)
 
-    def test_band_themes(self):
-        ...
-
     def test_band_dates(self):
         
         band = self.export.Band.get_profile('https://www.metal-archives.com/bands/Moonspell/61')
         self.assertIsNotNone(band)
         self.assertEqual(band.description.years_active, '1989-1992 (as Morbid God), 1992-present')
 
     def test_user_agents(self):
```

### Comparing `metalarchivist-0.2.9/src/test/test_genres.py` & `metalarchivist-0.3.0/src/test/test_genres.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,30 @@
     metalarchivist, interface, export, config = load_module()
 
     def test_genres_pages(self):
         target_genre = self.interface.Genre.POWER
 
         genre_length = self.export.Genre.get_genre_size(target_genre)
 
-        genre_bands = self.export.Genre.get_genre(target_genre)
+        genre_bands = self.export.Genre.get_genre(target_genre, page_size=1000)
         self.assertIsNotNone(genre_bands)
         self.assertIsInstance(genre_bands, self.interface.GenrePage)
         self.assertIsInstance(genre_bands.data, list)
 
         self.assertEqual(genre_length, len(genre_bands.data))
 
         self.assertIsInstance(genre_bands.data[0], self.interface.BandGenre)
         self.assertEqual(genre_bands.data[0].genre, target_genre.value)
 
         genre_json = genre_bands.to_json()
         self.assertIsInstance(genre_json, list)
-        self.assertIsInstance(genre_json[0], dict)
+
+        for record in genre_json:
+            self.assertIsInstance(record, dict)
+            self.assertIn('band_key', record)
 
     def test_genres(self):
 
         genres = self.interface.Subgenres('Black Metal/Black \'n\' Roll')
         self.assertIsNotNone(genres)
         self.assertEqual(len(genres.phases), 2)
         self.assertEqual(genres.clean_genre, 'Black, Black\'n\'Roll')
```

### Comparing `metalarchivist-0.2.9/src/test/test_themes.py` & `metalarchivist-0.3.0/src/test/test_themes.py`

 * *Files 21% similar despite different names*

```diff
@@ -77,7 +77,25 @@
         self.assertEqual(len(themes.phases), 6)
      
         themes = self.interface.Themes('Anime (Lolicon, Hentai), Suicide, Racism')
         self.assertIsNotNone(themes)
         self.assertEqual(themes.clean_theme, 'Anime (Lolicon, Hentai), Racism, Suicide')
         self.assertEqual(len(themes.phases), 3)
         self.assertEqual(len(themes.phases[0].subthemes), 2)
+        
+        themes = self.interface.Themes('Horror stories (Edgar Allan Poe / H.P. Lovecraft)')
+        self.assertIsNotNone(themes)
+        self.assertEqual(themes.clean_theme, 'Horror stories (Edgar Allan Poe, H.P. Lovecraft)')
+        self.assertEqual(len(themes.phases), 1)
+        self.assertEqual(len(themes.phases[0].subthemes), 2)
+        
+        themes = self.interface.Themes('Indigenous (Native American) issues, identity, history and culture')
+        self.assertIsNotNone(themes)
+        self.assertEqual(themes.clean_theme, 'Indigenous issues, identity, history and culture (Native American)')
+        self.assertEqual(len(themes.phases), 1)
+        self.assertEqual(len(themes.phases[0].subthemes), 1)
+        
+        themes = self.interface.Themes('History (first album), Life facts and struggles')
+        self.assertIsNotNone(themes)
+        self.assertEqual(themes.clean_theme, 'History, Life facts and struggles')
+        self.assertEqual(len(themes.phases), 2)
+        self.assertEqual(len(themes.phases[0].subthemes), 0)
```

