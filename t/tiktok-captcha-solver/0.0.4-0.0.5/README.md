# Comparing `tmp/tiktok_captcha_solver-0.0.4.tar.gz` & `tmp/tiktok_captcha_solver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok_captcha_solver-0.0.4.tar", last modified: Tue May 14 04:00:52 2024, max compression
+gzip compressed data, was "tiktok_captcha_solver-0.0.5.tar", last modified: Wed May 15 13:09:38 2024, max compression
```

## Comparing `tiktok_captcha_solver-0.0.4.tar` & `tiktok_captcha_solver-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2529 2024-05-14 04:00:19.000000 tiktok_captcha_solver-0.0.4/README.md
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1087 2024-05-14 04:00:39.000000 tiktok_captcha_solver-0.0.4/pyproject.toml
--rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-14 04:00:52.974847 tiktok_captcha_solver-0.0.4/setup.cfg
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.969847 tiktok_captcha_solver-0.0.4/src/
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.971847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/
--rw-r--r--   0 gregb     (1000) gregb     (1000)      120 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-12 21:58:21.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/models.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7982 2024-05-14 03:53:36.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     7865 2024-05-14 03:54:51.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/seleniumsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1688 2024-05-14 03:54:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/solver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.973847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/
--rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/__init__.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_api.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_downloader.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     1608 2024-05-14 03:57:25.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
--rw-r--r--   0 gregb     (1000) gregb     (1000)     2356 2024-05-14 03:57:24.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
-drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-14 04:00:52.973847 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/
--rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/PKG-INFO
--rw-r--r--   0 gregb     (1000) gregb     (1000)      792 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/SOURCES.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/dependency_links.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)      106 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/requires.txt
--rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-14 04:00:52.000000 tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/top_level.txt
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2529 2024-05-14 04:00:19.000000 tiktok_captcha_solver-0.0.5/README.md
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1087 2024-05-15 13:09:24.000000 tiktok_captcha_solver-0.0.5/pyproject.toml
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       38 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/setup.cfg
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.962226 tiktok_captcha_solver-0.0.5/src/
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.964226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      120 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1895 2024-05-12 21:58:21.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      350 2024-05-11 04:30:20.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      335 2024-05-05 06:12:30.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/models.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     8164 2024-05-15 12:47:17.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     7977 2024-05-15 13:01:27.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/seleniumsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2196 2024-05-15 13:03:24.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/solver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.965226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        0 2024-05-05 16:49:30.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/__init__.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1264 2024-05-05 17:22:04.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_api.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      189 2024-05-05 17:34:44.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_downloader.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     1608 2024-05-15 13:09:16.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_playwrightsolver.py
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     2356 2024-05-15 13:09:26.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_seleniumsolver.py
+drwxr-xr-x   0 gregb     (1000) gregb     (1000)        0 2024-05-15 13:09:38.966226 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/
+-rw-r--r--   0 gregb     (1000) gregb     (1000)     3533 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/PKG-INFO
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      792 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)        1 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)      106 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/requires.txt
+-rw-r--r--   0 gregb     (1000) gregb     (1000)       22 2024-05-15 13:09:38.000000 tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/top_level.txt
```

### Comparing `tiktok_captcha_solver-0.0.4/PKG-INFO` & `tiktok_captcha_solver-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tiktok_captcha_solver-0.0.4/README.md` & `tiktok_captcha_solver-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.4/pyproject.toml` & `tiktok_captcha_solver-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
 [project]
 name = "tiktok-captcha-solver"
-version = "0.0.4"
+version = "0.0.5"
 
 description = "This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code."
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["tiktok", "captcha", "solver", "selenium", "rotate", "puzzle", "3d"]
```

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/api.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/playwrightsolver.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/playwrightsolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This class handles the captcha solving for playwright users"""
 
 import random
 import time
 from typing import Literal
-from playwright.sync_api import FloatRect, Locator, Page
+from playwright.sync_api import FloatRect, Page
 from undetected_chromedriver import logging
 
 from .solver import Solver
 
 from .api import ApiClient
 from .downloader import download_image_b64
 
@@ -18,32 +18,28 @@
 
     def __init__(self, page: Page, sadcaptcha_api_key: str) -> None:
         self.page = page
         self.client = ApiClient(sadcaptcha_api_key)
 
     def captcha_is_present(self, timeout: int = 15) -> bool:
         for _ in range(timeout):
-            for wrapper in self.captcha_wrappers:
-                if len(self.page.locator(wrapper).all()) > 0:
-                    logging.debug("Detected captcha with wrapper: " + wrapper)
-                    return True
+            if self._any_selector_in_list_present(self.captcha_wrappers):
+                logging.debug("Captcha detected")
+                return True
             time.sleep(1)
         logging.debug("Did not detect captcha")
         return False
 
     def identify_captcha(self) -> Literal["puzzle", "shapes", "rotate"]:
-        rotate_selector = "[data-testid=whirl-inner-img]"
-        puzzle_selector = "img.captcha_verify_img_slide"
-        shapes_selector = "#verify-points"
         for _ in range(15):
-            if len(self.page.locator(puzzle_selector).all()) > 0:
+            if self._any_selector_in_list_present(self.puzzle_selectors):
                 return "puzzle"
-            elif len(self.page.locator(rotate_selector).all()) > 0:
+            elif self._any_selector_in_list_present(self.rotate_selectors):
                 return "rotate"
-            elif len(self.page.locator(shapes_selector).all()) > 0:
+            if self._any_selector_in_list_present(self.shapes_selectors):
                 return "shapes"
             else:
                 time.sleep(2)
         raise ValueError("Neither puzzle, shapes, or rotate captcha was present.")
 
     def solve_shapes(self, retries: int = 3) -> None:
         for _ in range(retries):
@@ -187,7 +183,15 @@
         self.page.mouse.move(start_x, start_y)
         time.sleep(random.randint(1, 10) / 11)
         self.page.mouse.down()
         time.sleep(random.randint(1, 10) / 11)
         self.page.mouse.move(start_x + x, start_y, steps=100)
         time.sleep(0.001)
         self.page.mouse.up()
+
+    def _any_selector_in_list_present(self, selectors: list[str]) -> bool:
+        for selector in selectors:
+            if len(self.page.locator(selector).all()) > 0:
+                logging.debug("Detected selector: " + selector + " from list " + ", ".join(selectors))
+                return True
+        logging.debug("No selector in list found: " + ", ".join(selectors))
+        return False
```

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/seleniumsolver.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/seleniumsolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,32 +21,28 @@
 
     def __init__(self, chromedriver: Chrome, sadcaptcha_api_key: str) -> None:
         self.chromedriver = chromedriver
         self.client = ApiClient(sadcaptcha_api_key)
 
     def captcha_is_present(self, timeout: int = 15) -> bool:
         for _ in range(timeout):
-            for wrapper in self.captcha_wrappers:
-                if len(self.chromedriver.find_elements(By.CSS_SELECTOR, wrapper)) > 0:
-                    logging.debug("Found captcha with wrapper: " + wrapper)
-                    return True
+            if self._any_selector_in_list_present(self.captcha_wrappers):
+                print("Captcha detected")
+                return True
             time.sleep(1)
         logging.debug("Captcha not found")
         return False
 
     def identify_captcha(self) -> Literal["puzzle", "shapes", "rotate"]:
-        rotate_selector = "[data-testid=whirl-inner-img]"
-        puzzle_selector = "img.captcha_verify_img_slide"
-        shapes_selector = "#verify-points"
         for _ in range(15):
-            if len(self.chromedriver.find_elements(By.CSS_SELECTOR, puzzle_selector)) > 0:
+            if self._any_selector_in_list_present(self.puzzle_selectors):
                 return "puzzle"
-            elif len(self.chromedriver.find_elements(By.CSS_SELECTOR, rotate_selector)) > 0:
+            elif self._any_selector_in_list_present(self.rotate_selectors):
                 return "rotate"
-            elif len(self.chromedriver.find_elements(By.CSS_SELECTOR, shapes_selector)) > 0:
+            elif self._any_selector_in_list_present(self.shapes_selectors):
                 return "shapes"
             else:
                 time.sleep(2)
         raise ValueError("Neither puzzle, shapes, or rotate captcha was present.")
 
     def solve_shapes(self, retries: int = 3) -> None:
         for _ in range(retries):
@@ -178,7 +174,14 @@
         actions.pause(0.7)
         for _ in range(0, 5):
             actions.move_by_offset(-1, 0)
             actions.pause(0.05)
         actions.pause(0.1)
         actions.release().perform()
 
+    def _any_selector_in_list_present(self, selectors: list[str]) -> bool:
+        for selector in selectors:
+            if len(self.chromedriver.find_elements(By.CSS_SELECTOR, selector)) > 0:
+                logging.debug("Detected selector: " + selector + " from list " + ", ".join(selectors))
+                return True
+        logging.debug("No selector in list found: " + ", ".join(selectors))
+        return False
```

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/solver.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/solver.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,39 @@
 
 class Solver(ABC):
 
     @property
     def captcha_wrappers(self) -> list[str]:
         return [
             "div#captcha_container",
-            "div.captcha_verify_container"
+            "div.captcha_verify_container",
+            "#verify-points",
+            ".captcha_verify_action",
         ]
 
+    @property
+    def rotate_selectors(self) -> list[str]:
+        return [
+            "[data-testid=whirl-inner-img]",
+            "[data-testid=whirl-outer-img]"
+        ]
+
+    @property
+    def puzzle_selectors(self) -> list[str]:
+        return [
+            "img.captcha_verify_img_slide"
+        ]
+
+    @property
+    def shapes_selectors(self) -> list[str]:
+        return [
+            ".verify-captcha-submit-button" 
+        ]
+
+
     def solve_captcha_if_present(self, captcha_detect_timeout: int = 15, retries: int = 3) -> None:
         """Solves any captcha that is present, if one is detected
 
         Args:
             captcha_detect_timeout: return if no captcha is detected in this many seconds
             retries: number of times to retry captcha
         """
```

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_api.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_playwrightsolver.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_playwrightsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver/tests/test_seleniumsolver.py` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver/tests/test_seleniumsolver.py`

 * *Files identical despite different names*

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/PKG-INFO` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktok-captcha-solver
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package integrates with Selenium or Playwright to solve any TikTok captcha in one line of code.
 Author-email: Toughdata LLC <greg@toughdata.net>
 Project-URL: Homepage, https://www.sadcaptcha.com
 Project-URL: Source, https://github.com/gbiz123/tiktok-captcha-solver/
 Keywords: tiktok,captcha,solver,selenium,rotate,puzzle,3d
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tiktok_captcha_solver-0.0.4/src/tiktok_captcha_solver.egg-info/SOURCES.txt` & `tiktok_captcha_solver-0.0.5/src/tiktok_captcha_solver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

