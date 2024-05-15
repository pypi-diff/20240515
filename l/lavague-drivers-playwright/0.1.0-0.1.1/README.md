# Comparing `tmp/lavague_drivers_playwright-0.1.0.tar.gz` & `tmp/lavague_drivers_playwright-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_playwright-0.1.0.tar", max compression
+gzip compressed data, was "lavague_drivers_playwright-0.1.1.tar", max compression
```

## Comparing `lavague_drivers_playwright-0.1.0.tar` & `lavague_drivers_playwright-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       36 2024-05-07 15:53:35.163891 lavague_drivers_playwright-0.1.0/README.md
--rw-r--r--   0        0        0       60 2024-05-07 15:52:56.168258 lavague_drivers_playwright-0.1.0/lavague/drivers/playwright/__init__.py
--rw-r--r--   0        0        0     6892 2024-05-08 00:19:38.337622 lavague_drivers_playwright-0.1.0/lavague/drivers/playwright/base.py
--rw-r--r--   0        0        0      981 2024-05-07 15:56:22.074270 lavague_drivers_playwright-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 lavague_drivers_playwright-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/README.md
+-rw-r--r--   0        0        0       61 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/__init__.py
+-rw-r--r--   0        0        0     7063 2024-05-15 19:17:05.222186 lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/base.py
+-rw-r--r--   0        0        0      984 2024-05-15 21:18:20.756384 lavague_drivers_playwright-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 lavague_drivers_playwright-0.1.1/PKG-INFO
```

### Comparing `lavague_drivers_playwright-0.1.0/lavague/drivers/playwright/base.py` & `lavague_drivers_playwright-0.1.1/lavague/drivers/playwright/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from typing import Callable, Optional
 from playwright.sync_api import Page
 from lavague.core.base_driver import BaseDriver
 
+
 class PlaywrightDriver(BaseDriver):
-    def __init__(self, url: Optional[str] = None, get_sync_playwright_page: Optional[Callable[[], Page]] = None):
+    driver: Page
+
+    def __init__(
+        self,
+        url: Optional[str] = None,
+        get_sync_playwright_page: Optional[Callable[[], Page]] = None,
+    ):
         super().__init__(url, get_sync_playwright_page)
-    
+
     def default_init_code(self) -> Page:
         # these imports are necessary as they will be pasted to the output
         try:
             from playwright.sync_api import sync_playwright
         except (ImportError, ModuleNotFoundError) as error:
             raise ImportError(
                 "Please install playwright using `pip install playwright` and then `playwright install` to install the necessary browser drivers"
@@ -18,50 +25,53 @@
         browser = p.chromium.launch()
         page = browser.new_page()
         return page
 
     def get_driver(self) -> Page:
         return self.driver
 
+    def resize_driver(self, width, height) -> None:
+        self.driver.set_viewport_size({"width": width, "height": height})
+
     def get_url(self) -> Optional[str]:
         if self.driver.url == "about:blank":
             return None
         return self.driver.url
 
     def go_to_url_code(self, url: str) -> str:
         return f'page.goto("{url}")'
 
     def goto(self, url: str) -> None:
         return self.driver.goto(url)
 
     def get_html(self) -> str:
         return self.driver.content()
 
-    def get_screenshot(self, filename: str) -> None:
+    def save_screenshot(self, filename: str) -> None:
         return self.driver.screenshot(path=filename)
 
     def get_dummy_code(self) -> str:
         return "page.mouse.wheel(delta_x=0, delta_y=500)"
 
     def destroy(self) -> None:
         self.driver.close()
 
     def check_visibility(self, xpath: str) -> bool:
         try:
-            return self.driver.locator(f'xpath={xpath}').is_visible()
+            return self.driver.locator(f"xpath={xpath}").is_visible()
         except:
             return False
 
     def exec_code(self, code: str):
         exec(self.import_lines)
         page = self.driver
         exec(code)
-    
+
     def get_capability(self) -> str:
-        return '''
+        return """
 Your goal is to write Playwright Python code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
 
 In your playwright code, you should only use the page.locator() or page.get_by_text() methods to uniquely locate and interact with the elements on the page. 
 For page.locator(), you must use XPath selectors to uniquely locate elements.
@@ -234,8 +244,8 @@
 action_button = page.get_by_text("Action Button").first
 
 # Then we can click on it
 action_button.click()
 ```
 
 ---
-'''
+"""
```

### Comparing `lavague_drivers_playwright-0.1.0/pyproject.toml` & `lavague_drivers_playwright-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-playwright"
-version = "0.1.0"
+version = "0.1.1"
 description = "Playwright integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -16,14 +16,14 @@
 keywords = ["LAM", "action", "automation", "LLM", "NLP", "RAG", "selenium", "playwright"]
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-lavague-core = "^0.1.0"
+python = "^3.10.0"
+lavague-core = "^0.1.1"
 playwright = "^1.42.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lavague_drivers_playwright-0.1.0/PKG-INFO` & `lavague_drivers_playwright-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-playwright
-Version: 0.1.0
+Version: 0.1.1
 Summary: Playwright integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: lavague-core (>=0.1.0,<0.2.0)
+Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
 Requires-Dist: playwright (>=1.42.0,<2.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
 
 # Playwright integration for lavague
```

