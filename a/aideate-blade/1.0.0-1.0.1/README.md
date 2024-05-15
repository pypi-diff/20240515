# Comparing `tmp/aideate_blade-1.0.0.tar.gz` & `tmp/aideate_blade-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.0.tar", last modified: Wed May 15 00:25:50 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.1.tar", last modified: Wed May 15 04:54:19 2024, max compression
```

## Comparing `aideate_blade-1.0.0.tar` & `aideate_blade-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:25:50.034307 aideate_blade-1.0.0/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 00:25:50.034116 aideate_blade-1.0.0/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.0/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:25:50.033491 aideate_blade-1.0.0/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 00:25:50.000000 aideate_blade-1.0.0/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      478 2024-05-15 00:25:50.000000 aideate_blade-1.0.0/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 00:25:50.000000 aideate_blade-1.0.0/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 00:25:50.000000 aideate_blade-1.0.0/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        8 2024-05-15 00:25:50.000000 aideate_blade-1.0.0/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:25:50.029884 aideate_blade-1.0.0/scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:25:50.031692 aideate_blade-1.0.0/scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    12259 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1953 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:25:50.032483 aideate_blade-1.0.0/scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      707 2024-05-15 00:07:08.000000 aideate_blade-1.0.0/scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 00:25:50.034452 aideate_blade-1.0.0/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      876 2024-05-15 00:25:24.000000 aideate_blade-1.0.0/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.321828 aideate_blade-1.0.1/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 04:54:19.321641 aideate_blade-1.0.1/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-14 20:10:32.000000 aideate_blade-1.0.1/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.321369 aideate_blade-1.0.1/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      814 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      478 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      359 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        8 2024-05-15 04:54:19.000000 aideate_blade-1.0.1/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.319089 aideate_blade-1.0.1/scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.320185 aideate_blade-1.0.1/scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      529 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      822 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    12285 2024-05-15 04:53:47.000000 aideate_blade-1.0.1/scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1953 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-15 04:54:19.320769 aideate_blade-1.0.1/scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      707 2024-05-15 00:07:08.000000 aideate_blade-1.0.1/scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-15 04:54:19.321863 aideate_blade-1.0.1/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      876 2024-05-15 04:53:57.000000 aideate_blade-1.0.1/setup.py
```

### Comparing `aideate_blade-1.0.0/LICENSE` & `aideate_blade-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/PKG-INFO` & `aideate_blade-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate_blade
-Version: 1.0.0
+Version: 1.0.1
 Summary: web content scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.0/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.1/aideate_blade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate_blade
-Version: 1.0.0
+Version: 1.0.1
 Summary: web content scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.0/scraper/core/image_utils.py` & `aideate_blade-1.0.1/scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/scraper/core/schemas.py` & `aideate_blade-1.0.1/scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/scraper/core/scrape.py` & `aideate_blade-1.0.1/scraper/core/scrape.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import magic
 import pdfplumber
 from PIL import Image
 from prometheus_client import Counter
 from snakemd import Document as mdDocument
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
-from image_utils import async_http_get_image
+from scraper.core.image_utils import async_http_get_image
+from scraper.core.schemas import WebScrapeContent, WebContentType
 from scraper.modal.modal_client import playwright_web_scrape
 from scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
 from settings import ZENROWS_API_KEY
-from schemas import WebScrapeContent, WebContentType
 
 logger = logging.getLogger(__name__)
 
 LLM_SUMMARIZE_FAIL_COUNTER = Counter(
     "scrape_llm_summarize_fail_request", "Number of llm summarize requests that failed"
 )
```

### Comparing `aideate_blade-1.0.0/scraper/core/scrape_playwright.py` & `aideate_blade-1.0.1/scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/scraper/core/scrape_utils.py` & `aideate_blade-1.0.1/scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/scraper/modal/modal_tasks.py` & `aideate_blade-1.0.1/scraper/modal/modal_tasks.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.0/setup.py` & `aideate_blade-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate_blade',
-    version='1.0.0',
+    version='1.0.1',
     description='web content scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
```

