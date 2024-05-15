# Comparing `tmp/aideate_blade-1.0.3.tar.gz` & `tmp/aideate_blade-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.3.tar", last modified: Wed May 15 20:25:40 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.4.tar", last modified: Wed May 15 21:05:00 2024, max compression
```

## Comparing `aideate_blade-1.0.3.tar` & `aideate_blade-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.986661 aideate_blade-1.0.3/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 20:25:40.986501 aideate_blade-1.0.3/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.3/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.986155 aideate_blade-1.0.3/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      558 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.983996 aideate_blade-1.0.3/aideate_scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.985361 aideate_blade-1.0.3/aideate_scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    12317 2024-05-15 05:30:34.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1969 2024-05-15 05:30:34.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.985927 aideate_blade-1.0.3/aideate_scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 20:24:24.000000 aideate_blade-1.0.3/aideate_scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-15 20:24:24.000000 aideate_blade-1.0.3/aideate_scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 20:25:40.986696 aideate_blade-1.0.3/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      884 2024-05-15 20:25:38.000000 aideate_blade-1.0.3/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 21:05:00.742641 aideate_blade-1.0.4/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 21:05:00.742459 aideate_blade-1.0.4/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.4/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 21:05:00.742150 aideate_blade-1.0.4/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 21:05:00.000000 aideate_blade-1.0.4/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      558 2024-05-15 21:05:00.000000 aideate_blade-1.0.4/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 21:05:00.000000 aideate_blade-1.0.4/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 21:05:00.000000 aideate_blade-1.0.4/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-15 21:05:00.000000 aideate_blade-1.0.4/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 21:05:00.740203 aideate_blade-1.0.4/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 21:05:00.741335 aideate_blade-1.0.4/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    12821 2024-05-15 21:02:57.000000 aideate_blade-1.0.4/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1969 2024-05-15 05:30:34.000000 aideate_blade-1.0.4/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 21:05:00.741778 aideate_blade-1.0.4/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.4/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 20:24:24.000000 aideate_blade-1.0.4/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-15 20:24:24.000000 aideate_blade-1.0.4/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 21:05:00.742678 aideate_blade-1.0.4/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      884 2024-05-15 21:04:01.000000 aideate_blade-1.0.4/setup.py
```

### Comparing `aideate_blade-1.0.3/LICENSE` & `aideate_blade-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/PKG-INFO` & `aideate_blade-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.3
+Version: 1.0.4
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.3/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.4/aideate_blade.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.3
+Version: 1.0.4
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.3/aideate_blade.egg-info/SOURCES.txt` & `aideate_blade-1.0.4/aideate_blade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/aideate_scraper/core/image_utils.py` & `aideate_blade-1.0.4/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/aideate_scraper/core/schemas.py` & `aideate_blade-1.0.4/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/aideate_scraper/core/scrape.py` & `aideate_blade-1.0.4/aideate_scraper/core/scrape.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,14 +244,31 @@
     response = await process_web_content(content, url)
     if response:
         return response
 
     return None
 
 
+async def async_scrape_web_content(url: str) -> Optional[Union[str, bytes]]:
+    # scrape without parsing
+    if not is_instagram_url(url):
+        # instagram doesn't work for these options but in general we want them first
+
+        content = await aget_scrape_api(url)
+        if content:
+            return content
+
+        # fallback to requests
+        content = await aget(url)
+        if content:
+            return content
+
+    return await playwright_web_scrape(url, timeout=int(TIMEOUT_SEC))
+
+
 class ContentExceedMaxLimit(Exception):
     pass
 
 
 def make_default_headers(user_agent: str) -> dict:
     return {
         "accept": "*/*",
```

### Comparing `aideate_blade-1.0.3/aideate_scraper/core/scrape_playwright.py` & `aideate_blade-1.0.4/aideate_scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/aideate_scraper/core/scrape_utils.py` & `aideate_blade-1.0.4/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/aideate_scraper/modal/modal_tasks.py` & `aideate_blade-1.0.4/aideate_scraper/modal/modal_tasks.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.3/setup.py` & `aideate_blade-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate-blade',
-    version='1.0.3',
+    version='1.0.4',
     description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
```

