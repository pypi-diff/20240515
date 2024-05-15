# Comparing `tmp/temsah-2.1.4.tar.gz` & `tmp/temsah-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temsah-2.1.4.tar", last modified: Thu Apr 18 14:17:21 2024, max compression
+gzip compressed data, was "temsah-2.1.5.tar", last modified: Wed May 15 19:02:05 2024, max compression
```

## Comparing `temsah-2.1.4.tar` & `temsah-2.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.220898 temsah-2.1.4/
--rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2024-04-18 14:17:21.219900 temsah-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1746 2024-04-09 22:22:13.000000 temsah-2.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 14:17:21.220898 temsah-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-04-18 14:15:27.000000 temsah-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.210318 temsah-2.1.4/temsah/
--rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.4/temsah/__init__.py
--rw-rw-rw-   0        0        0     1656 2024-04-09 18:12:37.000000 temsah-2.1.4/temsah/currency.py
--rw-rw-rw-   0        0        0    16801 2024-04-18 14:15:12.000000 temsah-2.1.4/temsah/data_extractor.py
--rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.4/temsah/main.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:17:21.218899 temsah-2.1.4/temsah.egg-info/
--rw-rw-rw-   0        0        0      268 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 14:17:20.000000 temsah-2.1.4/temsah.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.306172 temsah-2.1.5/
+-rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2024-05-15 19:02:05.303699 temsah-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1746 2024-04-09 22:22:13.000000 temsah-2.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:02:05.306172 temsah-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-05-15 18:57:38.000000 temsah-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.273717 temsah-2.1.5/temsah/
+-rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.5/temsah/__init__.py
+-rw-rw-rw-   0        0        0     3257 2024-05-13 14:37:04.000000 temsah-2.1.5/temsah/currency.py
+-rw-rw-rw-   0        0        0    16801 2024-04-18 14:15:12.000000 temsah-2.1.5/temsah/data_extractor.py
+-rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.5/temsah/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.300540 temsah-2.1.5/temsah.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/top_level.txt
```

### Comparing `temsah-2.1.4/LICENSE.txt` & `temsah-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temsah-2.1.4/README.md` & `temsah-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `temsah-2.1.4/temsah/currency.py` & `temsah-2.1.5/temsah/currency.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,89 @@
 from bs4 import BeautifulSoup
 import requests
 import chardet
-# ---------------------------
+
+#-------------------------------------
 class Currency:
     def __init__(self):
-        self.url = 'https://www.tgju.org/profile/price_aed'
+    self.url_aed = 'https://www.tgju.org/profile/price_aed'
+    self.url_dollar = 'https://www.tgju.org/profile/price_dollar_rl'
+    self.currency = {}
+#-------------------------------------
+
+    def scrape(self):
         self.currency = {}
+        self.scrape_aed()
+        self.scrape_dollar()
+        return self.currency
 
+#-------------------------------------
 
-    
-    def scrape(self):
-        url = self.url
+    def scrape_aed(self):
+        url = self.url_aed
+        
         headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
             "Accept-Language": "en-US,en;q=0.5",
         }
         page = requests.get(url, headers=headers)
         if page.status_code == 200:
             encoding = chardet.detect(page.content)["encoding"]
             html = page.content.decode(encoding)
             soup = BeautifulSoup(html, "html.parser")
-            scraper = self.get(soup)
-            # ---------------------------
+            scraper = self.get_aed(soup)
         else:
             print(f"page.status_code:{page.status_code}")
 
         return self.currency
             
-    def get(self, soup):
+    def get_aed(self, soup):
         
         self.currency = {}
-        
-            
+      
         div_tag=soup.find('div',class_='fs-cell fs-xl-5 fs-lg-5 fs-md-12 fs-sm-12 fs-xs-12 top-header-item-block-1')
         if div_tag:
             div_tag=soup.find('div',class_='block-last-change-percentage')
             if div_tag:
                 sp_tag = div_tag.find('span', class_='price')
                 if sp_tag:
                     self.currency["AED_currency"] = sp_tag.text 
                 else:
                     print('span tag not found')
             else:
                 print('div tag not found')
         else:
             print('div tag not found')
+            
+    #--------------------scrape_dollar----------------------
+    
+    def scrape_dollar(self):
+        url = self.url_dollar
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
+            "Accept-Language": "en-US,en;q=0.5",
+        }
+        page = requests.get(url, headers=headers)
+        if page.status_code == 200:
+            encoding = chardet.detect(page.content)["encoding"]
+            html = page.content.decode(encoding)
+            soup = BeautifulSoup(html, "html.parser")
+            self.get_dollar(soup)
+        else:
+            print(f"page.status_code:{page.status_code}")
+    
+    def get_dollar(self, soup):
+    div_tag = soup.find('div', class_='fs-cell fs-xl-5 fs-lg-5 fs-md-12 fs-sm-12 fs-xs-12 top-header-item-block-1')
+    if div_tag:
+        div_tag = soup.find('div', class_='block-last-change-percentage')
+        if div_tag:
+            sp_tag = div_tag.find('span', class_='price')
+            if sp_tag:
+                self.currency["USD_currency"] = sp_tag.text 
+            else:
+                print('span tag not found for USD')
+        else:
+            print('div tag not found for USD')
+    else:
+        print('div tag not found for USD')
+
```

### Comparing `temsah-2.1.4/temsah/data_extractor.py` & `temsah-2.1.5/temsah/data_extractor.py`

 * *Files identical despite different names*

### Comparing `temsah-2.1.4/temsah/main.py` & `temsah-2.1.5/temsah/main.py`

 * *Files identical despite different names*

