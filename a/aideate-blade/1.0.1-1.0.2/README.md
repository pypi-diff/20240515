# Comparing `tmp/aideate_blade-1.0.1.tar.gz` & `tmp/aideate_blade-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.1.tar", last modified: Wed May 15 04:54:19 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.2.tar", last modified: Wed May 15 05:38:02 2024, max compression
```

## Comparing `aideate_blade-1.0.1.tar` & `aideate_blade-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.321828 aideate_blade-1.0.1/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 04:54:19.321641 aideate_blade-1.0.1/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.1/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.321369 aideate_blade-1.0.1/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      478 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        8 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.319089 aideate_blade-1.0.1/scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.320185 aideate_blade-1.0.1/scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    12285 2024-05-15 04:53:47.000000 aideate_blade-1.0.1/scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1953 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.320769 aideate_blade-1.0.1/scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      707 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 04:54:19.321863 aideate_blade-1.0.1/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      876 2024-05-15 04:53:57.000000 aideate_blade-1.0.1/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114976 aideate_blade-1.0.2/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 05:38:02.114789 aideate_blade-1.0.2/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.2/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114473 aideate_blade-1.0.2/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      558 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-15 05:38:02.000000 aideate_blade-1.0.2/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.110535 aideate_blade-1.0.2/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.113783 aideate_blade-1.0.2/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    12317 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1969 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 05:38:02.114261 aideate_blade-1.0.2/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.2/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      494 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      723 2024-05-15 05:30:34.000000 aideate_blade-1.0.2/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 05:38:02.115007 aideate_blade-1.0.2/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      884 2024-05-15 05:37:12.000000 aideate_blade-1.0.2/setup.py
```

### Comparing `aideate_blade-1.0.1/LICENSE` & `aideate_blade-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.1/PKG-INFO` & `aideate_blade-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: aideate_blade
-Version: 1.0.1
-Summary: web content scraper
+Name: aideate-blade
+Version: 1.0.2
+Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
 Requires-Dist: boto3==1.29.6
```

### Comparing `aideate_blade-1.0.1/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.2/aideate_blade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: aideate_blade
-Version: 1.0.1
-Summary: web content scraper
+Name: aideate-blade
+Version: 1.0.2
+Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
 Requires-Dist: boto3==1.29.6
```

### Comparing `aideate_blade-1.0.1/scraper/core/image_utils.py` & `aideate_blade-1.0.2/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.1/scraper/core/schemas.py` & `aideate_blade-1.0.2/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.1/scraper/core/scrape.py` & `aideate_blade-1.0.2/aideate_scraper/core/scrape.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import magic
 import pdfplumber
 from PIL import Image
 from prometheus_client import Counter
 from snakemd import Document as mdDocument
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
-from scraper.core.image_utils import async_http_get_image
-from scraper.core.schemas import WebScrapeContent, WebContentType
-from scraper.modal.modal_client import playwright_web_scrape
-from scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
+from aideate_scraper.core.image_utils import async_http_get_image
+from aideate_scraper.core.schemas import WebScrapeContent, WebContentType
+from aideate_scraper.modal.modal_client import playwright_web_scrape
+from aideate_scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
 from settings import ZENROWS_API_KEY
 
 logger = logging.getLogger(__name__)
 
 LLM_SUMMARIZE_FAIL_COUNTER = Counter(
     "scrape_llm_summarize_fail_request", "Number of llm summarize requests that failed"
 )
```

### Comparing `aideate_blade-1.0.1/scraper/core/scrape_playwright.py` & `aideate_blade-1.0.2/aideate_scraper/core/scrape_playwright.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import BytesIO
 from typing import Optional
 
 import magic
 from playwright.async_api import async_playwright
 from prometheus_client import Counter
 
-from scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
+from aideate_scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
 
 PLAYWRIGHT_COUNTER = Counter("playwright_request", "Number of api requests")
 
 PLAYWRIGHT_FAIL_COUNTER = Counter(
     "playwright_fail_request", "Number of get requests that failed"
 )
 
@@ -20,15 +20,15 @@
     # https://github.com/Josh-XT/AGiXT/blob/main/agixt/extensions/web_playwright.py
     async with async_playwright() as p:
         browser = await p.chromium.launch(headless=True)
         context = await browser.new_context(
             viewport={"width": 1920, "height": 1080}, user_agent=get_user_agent()
         )
         await context.add_init_script(
-            path="/envision/ml/scraper/core/libs/stealth.min.js"
+            path="/envision/ml/aideate_scraper/core/libs/stealth.min.js"
         )
         page = await context.new_page()
         text = None
         try:
             response = await page.goto(url, timeout=TIMEOUT_SEC * 1_000)
             text = await response.body()
             content_type = magic.from_buffer(BytesIO(text).read(2048), mime=True)
```

### Comparing `aideate_blade-1.0.1/scraper/core/scrape_utils.py` & `aideate_blade-1.0.2/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.1/scraper/modal/modal_tasks.py` & `aideate_blade-1.0.2/aideate_scraper/modal/modal_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Optional
 
 from modal import Function, Image, Mount, Secret, Stub, asgi_app, gpu, method
 
 import proto.gen.message_pb2 as message_pb2
 from modal_functions.tasks.base import image
 
-workers_stub = Stub("web-scraper", image=image)
+workers_stub = Stub("web-aideate_scraper", image=image)
 
 
 @workers_stub.function(secrets=[Secret.from_name("my-aws-secret")])
 async def playwright_web_scrape(url) -> Optional[message_pb2.DocumentMessage]:
-    from scraper.core.scrape_playwright import aget_playwright
+    from aideate_scraper.core.scrape_playwright import aget_playwright
 
     result = await aget_playwright(url)
     return result
 
 
 # Test each method
 @workers_stub.local_entrypoint()
```

### Comparing `aideate_blade-1.0.1/setup.py` & `aideate_blade-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
-    name='aideate_blade',
-    version='1.0.1',
-    description='web content scraper',
+    name='aideate-blade',
+    version='1.0.2',
+    description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
         "ipdb==0.13.11",
```

