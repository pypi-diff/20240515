# Comparing `tmp/aideate_blade-1.0.2.tar.gz` & `tmp/aideate_blade-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.2.tar", last modified: Wed May 15 05:38:02 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.3.tar", last modified: Wed May 15 20:25:40 2024, max compression
```

## Comparing `aideate_blade-1.0.2.tar` & `aideate_blade-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114976 aideate_blade-1.0.2/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 05:38:02.114789 aideate_blade-1.0.2/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.2/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114473 aideate_blade-1.0.2/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      558 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.110535 aideate_blade-1.0.2/aideate_scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.113783 aideate_blade-1.0.2/aideate_scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    12317 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1969 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114261 aideate_blade-1.0.2/aideate_scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      494 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      723 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 05:38:02.115007 aideate_blade-1.0.2/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      884 2024-05-15 05:37:12.000000 aideate_blade-1.0.2/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.986661 aideate_blade-1.0.3/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 20:25:40.986501 aideate_blade-1.0.3/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.3/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.986155 aideate_blade-1.0.3/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      558 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-15 20:25:40.000000 aideate_blade-1.0.3/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.983996 aideate_blade-1.0.3/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.985361 aideate_blade-1.0.3/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    12317 2024-05-15 05:30:34.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1969 2024-05-15 05:30:34.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 20:25:40.985927 aideate_blade-1.0.3/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.3/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 20:24:24.000000 aideate_blade-1.0.3/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-15 20:24:24.000000 aideate_blade-1.0.3/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 20:25:40.986696 aideate_blade-1.0.3/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      884 2024-05-15 20:25:38.000000 aideate_blade-1.0.3/setup.py
```

### Comparing `aideate_blade-1.0.2/LICENSE` & `aideate_blade-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/PKG-INFO` & `aideate_blade-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.2
+Version: 1.0.3
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.2/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.3/aideate_blade.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.2
+Version: 1.0.3
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.2/aideate_blade.egg-info/SOURCES.txt` & `aideate_blade-1.0.3/aideate_blade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/core/image_utils.py` & `aideate_blade-1.0.3/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/core/schemas.py` & `aideate_blade-1.0.3/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/core/scrape.py` & `aideate_blade-1.0.3/aideate_scraper/core/scrape.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/core/scrape_playwright.py` & `aideate_blade-1.0.3/aideate_scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/core/scrape_utils.py` & `aideate_blade-1.0.3/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.2/aideate_scraper/modal/modal_tasks.py` & `aideate_blade-1.0.3/aideate_scraper/modal/modal_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 
 from modal import Function, Image, Mount, Secret, Stub, asgi_app, gpu, method
 
 import proto.gen.message_pb2 as message_pb2
 from modal_functions.tasks.base import image
 
-workers_stub = Stub("web-aideate_scraper", image=image)
+workers_stub = Stub("web-scraper", image=image)
 
 
 @workers_stub.function(secrets=[Secret.from_name("my-aws-secret")])
 async def playwright_web_scrape(url) -> Optional[message_pb2.DocumentMessage]:
     from aideate_scraper.core.scrape_playwright import aget_playwright
 
     result = await aget_playwright(url)
```

### Comparing `aideate_blade-1.0.2/setup.py` & `aideate_blade-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate-blade',
-    version='1.0.2',
+    version='1.0.3',
     description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
```

