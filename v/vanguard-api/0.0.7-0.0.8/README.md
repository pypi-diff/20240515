# Comparing `tmp/vanguard_api-0.0.7.tar.gz` & `tmp/vanguard_api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.7.tar", last modified: Mon May 13 11:04:32 2024, max compression
+gzip compressed data, was "vanguard_api-0.0.8.tar", last modified: Wed May 15 10:32:21 2024, max compression
```

## Comparing `vanguard_api-0.0.7.tar` & `vanguard_api-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 11:04:28.000000 vanguard_api-0.0.7/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:04:32.444222 vanguard_api-0.0.7/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 11:04:32.000000 vanguard_api-0.0.7/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:21.618747 vanguard_api-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 10:32:21.618747 vanguard_api-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:32:21.618747 vanguard_api-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:21.614747 vanguard_api-0.0.8/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 10:32:17.000000 vanguard_api-0.0.8/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:21.618747 vanguard_api-0.0.8/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 10:32:21.000000 vanguard_api-0.0.8/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 10:32:21.000000 vanguard_api-0.0.8/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:32:21.000000 vanguard_api-0.0.8/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 10:32:21.000000 vanguard_api-0.0.8/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 10:32:21.000000 vanguard_api-0.0.8/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.7/LICENSE` & `vanguard_api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.7/PKG-INFO` & `vanguard_api-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.8.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.0.7/README.md` & `vanguard_api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.7/setup.py` & `vanguard_api-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.7",
+    version="0.0.8",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.8.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.7/vanguard/account.py` & `vanguard_api-0.0.8/vanguard/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,37 @@
                             "dollar_change": dollar_change,
                             "percent_change": percent_change,
                             "quantity": quantity,
                         }
                     )
                     self.accounts_positions[account_id][type] = stocks
 
+    def get_account_ids(self):
+        """
+        Retrieves and sets the account numbers associated with the session.
+
+        This method navigates to the account holdings page, waits for the account numbers to load, and then retrieves the account numbers from the page.
+
+        Returns:
+            bool: True if the account numbers were successfully retrieved, False otherwise.
+        """
+        try:
+            self.session.go_url(holdings_page())
+            self.session.page.wait_for_selector(
+                '//span[contains(text(), "Expand all accounts")]', timeout=120000
+            ).click()
+            self.session.page.wait_for_selector("#overflow-override")
+            all_selectors = self.session.page.query_selector_all("#overflow-override")
+            for _, selector in enumerate(all_selectors):
+                account_id = self._get_account_id(selector)
+                self.account_numbers.append(account_id)
+            return True
+        except PlaywrightTimeoutError:
+            return False
+
     def get_holdings(self):
         """
         Retrieves and sets the holdings information of the account.
 
         This method navigates to the account holdings page, waits for the holdings information to load, and then retrieves the holdings information from the page.
 
         Returns:
@@ -159,15 +182,14 @@
             self.total_value = float(
                 total_element.inner_text().split()[-1].replace(",", "").replace("$", "")
             )
             self.session.page.wait_for_selector("#overflow-override")
             all_selectors = self.session.page.query_selector_all("#overflow-override")
             for i, selector in enumerate(all_selectors):
                 account_id = self._get_account_id(selector)
-                self.account_numbers.append(account_id)
                 table_wrapper = selector.wait_for_selector(f"#self_managed_table_{i}")
                 table_entries = table_wrapper.query_selector_all("tbody")
                 for j, entry in enumerate(table_entries):
                     if j == len(table_entries) - 1:
                         total_row = entry.query_selector_all("tr")
                         for row in total_row:
                             totals = row.inner_text().split()
```

### Comparing `vanguard_api-0.0.7/vanguard/order.py` & `vanguard_api-0.0.8/vanguard/order.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.7/vanguard/session.py` & `vanguard_api-0.0.8/vanguard/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,51 +141,57 @@
 
         Raises:
             Exception: If there is an error during the login process in step one.
         """
         try:
             self.password = password
             self.go_url(landing_page())
-            try:
-                self.page.wait_for_selector(
-                    "#username-password-submit-btn-1", timeout=30000
-                )
-            except PlaywrightTimeoutError:
-                if self.page.url == landing_page():
-                    return False
-                raise Exception("Could not find submit button on login page.")
+            for _ in range(30):
+                try:
+                    if self.page.url == landing_page():
+                        self.page.wait_for_selector(
+                            "//h2[contains(text(), 'Accounts')]",
+                            timeout=1000,
+                        )
+                        return False
+                    self.page.wait_for_selector(
+                        "#username-password-submit-btn-1", timeout=1000
+                    )
+                    break
+                except PlaywrightTimeoutError:
+                    continue
             username_box = self.page.query_selector("#USER")
             username_box.type(username, delay=random.randint(50, 500))
             username_box.press("Tab")
             password_box = self.page.query_selector("#PASSWORD-blocked")
             password_box.type(password, delay=random.randint(50, 500))
             sleep(random.uniform(1, 3))
             self.page.query_selector("#username-password-submit-btn-1").click()
             try:
                 self.page.wait_for_selector(
-                    "button.col-md:nth-child(2) > div:nth-child(1)", timeout=10000
+                    "button.col-md:nth-child(2) > div:nth-child(1)", timeout=5000
                 ).click()
             except PlaywrightTimeoutError:
                 pass
             try:
                 self.page.wait_for_selector(
-                    "xpath=//div[contains(text(), '***-***-')]", timeout=10000
+                    "xpath=//div[contains(text(), '***-***-')]", timeout=5000
                 )
                 otp_cards = self.page.query_selector_all(
                     "xpath=//div[contains(text(), '***-***-')]"
                 )
                 for otp_card in otp_cards:
                     if otp_card.inner_text() == f"***-***-{last_four}":
                         otp_card.click()
                         break
             except PlaywrightTimeoutError:
                 pass
             try:
                 self.page.wait_for_selector(
-                    "xpath=//div[contains(text(), 'Text')]", timeout=10000
+                    "xpath=//div[contains(text(), 'Text')]", timeout=5000
                 ).click()
                 return True
             except PlaywrightTimeoutError:
                 if self.title is not None:
                     self.save_storage_state()
                 return False
         except Exception as e:
@@ -204,25 +210,25 @@
             Exception: Failed to login to chase.
 
         Returns:
             bool: True if login is successful, False otherwise.
         """
         try:
             code = str(code)
-            self.page.wait_for_selector("#CODE", timeout=10000).fill(code)
+            self.page.wait_for_selector("#CODE", timeout=5000).fill(code)
             self.page.query_selector(
                 "c11n-radio.c11n-radio:nth-child(2) > label:nth-child(2)"
             ).click()
             self.page.wait_for_selector(
-                "#security-code-submit-btn", timeout=10000
+                "#security-code-submit-btn", timeout=5000
             ).click()
             sleep(5)
             try:
                 self.page.wait_for_url(
-                    landing_page(), wait_until="domcontentloaded", timeout=10000
+                    landing_page(), wait_until="domcontentloaded", timeout=5000
                 )
                 if self.title is not None:
                     self.save_storage_state()
                 return True
             except TimeoutError:
                 raise Exception("Failed to login to Vanguard")
         except Exception as e:
```

### Comparing `vanguard_api-0.0.7/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.0.8/vanguard_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.7.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.8.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

