# Comparing `tmp/crawlist-0.0.9.tar.gz` & `tmp/crawlist-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.9.tar", last modified: Wed May  8 11:10:04 2024, max compression
+gzip compressed data, was "crawlist-0.1.0.tar", last modified: Wed May 15 07:36:31 2024, max compression
```

## Comparing `crawlist-0.0.9.tar` & `crawlist-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 11:09:59.000000 crawlist-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 11:09:59.000000 crawlist-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-08 11:10:04.670817 crawlist-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-08 11:09:59.000000 crawlist-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.666817 crawlist-0.0.9/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.666817 crawlist-0.0.9/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist/analyzers/pager/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/pager/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/analyzers/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-08 11:09:59.000000 crawlist-0.0.9/crawlist/processings/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:10:04.670817 crawlist-0.0.9/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 11:10:04.000000 crawlist-0.0.9/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:10:04.670817 crawlist-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-08 11:09:59.000000 crawlist-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.088747 crawlist-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 07:36:22.000000 crawlist-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 07:36:22.000000 crawlist-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-15 07:36:31.088747 crawlist-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-15 07:36:22.000000 crawlist-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.084747 crawlist-0.1.0/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.084747 crawlist-0.1.0/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.084747 crawlist-0.1.0/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.084747 crawlist-0.1.0/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 07:36:22.000000 crawlist-0.1.0/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:36:31.088747 crawlist-0.1.0/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-15 07:36:31.000000 crawlist-0.1.0/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 07:36:31.000000 crawlist-0.1.0/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:36:31.000000 crawlist-0.1.0/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 07:36:31.000000 crawlist-0.1.0/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 07:36:31.000000 crawlist-0.1.0/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:36:31.088747 crawlist-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-15 07:36:22.000000 crawlist-0.1.0/setup.py
```

### Comparing `crawlist-0.0.9/LICENSE` & `crawlist-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/PKG-INFO` & `crawlist-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.9
+Version: 0.1.0
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,15 +47,15 @@
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.
 
 ## installing
 You can use pip or pip3 to install the crawlist
 
 `pip install crawlist` or `pip3 install crawlist`
 
 If you have already installed crawlist, you may need to update to the latest version
@@ -112,11 +112,11 @@
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the link below.
 
-[English](https://wwydev.gitbook.io/crawlist "English Document")
+[中文](https://wwydev.gitbook.io/crawlist-zh/ "中文文档")|[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crawlist-0.0.9/README.md` & `crawlist-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.
 
 ## installing
 You can use pip or pip3 to install the crawlist
 
 `pip install crawlist` or `pip3 install crawlist`
 
 If you have already installed crawlist, you may need to update to the latest version
@@ -87,11 +87,11 @@
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the link below.
 
-[English](https://wwydev.gitbook.io/crawlist "English Document")
+[中文](https://wwydev.gitbook.io/crawlist-zh/ "中文文档")|[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crawlist-0.0.9/crawlist/analyzers/analyzer.py` & `crawlist-0.1.0/crawlist/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/driver.py` & `crawlist-0.1.0/crawlist/analyzers/driver.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/pager/dynamic_pager.py` & `crawlist-0.1.0/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,31 +51,36 @@
                 self.webdriver.quit()
             except:
                 pass
 
 
 class DynamicRedirectPager(DynamicPager):
     @check
-    def __init__(self, uri: str, uri_split: str, webdriver: Driver | WebDriver = None, start: int = 1, offset: int = 1,
+    def __init__(self, uri_split: str, uri: str = "", webdriver: Driver | WebDriver = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
         Based on dynamic web page analyzer (redirect page flipping)
-        :param uri: First page link
         :param uri_split: Link pagination (using% v proxy) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
+        :param uri: If set, It will be the First page link.
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert '%v' in uri_split
-        assert Valid.is_valid_url(uri) and Valid.is_valid_url(uri_split.replace('%v', str(start)))
+        if uri:
+            assert Valid.is_valid_url(uri)
+        assert Valid.is_valid_url(uri_split.replace('%v', str(start)))
         assert offset >= 1 and start >= 0
         self.index = start
         self.offset = offset
-        self.current_uri = uri
+        if uri:
+            self.current_uri = uri
+        else:
+            self.current_uri = uri_split.replace('%v', str(start))
         self.uri_split = uri_split
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(self.webdriver)
         self.sleep()
 
     def next(self) -> None:
         self.index += self.offset
```

### Comparing `crawlist-0.0.9/crawlist/analyzers/pager/pager.py` & `crawlist-0.1.0/crawlist/analyzers/pager/pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/pager/static_pager.py` & `crawlist-0.1.0/crawlist/analyzers/pager/static_pager.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,37 @@
         else:
             self.request = request
         super().__init__(interval=interval)
 
 
 class StaticRedirectPager(StaticPager):
     @check
-    def __init__(self, uri: str, uri_split: str, request: Request = None, start: int = 1, offset: int = 1,
+    def __init__(self,  uri_split: str, uri: str = "", request: Request = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
         Based on static web page analyzer (redirect page flipping)
-        :param uri: First page link
         :param uri_split: Link pagination (using %v instead) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
+        :param uri: If set, It will be the First page link.
         :param request: Request object
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert '%v' in uri_split
-        assert Valid.is_valid_url(uri) and Valid.is_valid_url(uri_split.replace('%v', str(start)))
+        if uri:
+            assert Valid.is_valid_url(uri)
+        assert Valid.is_valid_url(uri_split.replace('%v', str(start)))
         assert offset >= 1 and start >= 0
         super().__init__(request=request, interval=interval)
         self.index = start
         self.offset = offset
-        self.current_uri = uri
+        if uri:
+            self.current_uri = uri
+        else:
+            self.current_uri = uri_split.replace('%v', str(start))
         self.uri_split = uri_split
 
     def next(self) -> None:
         self.index += self.offset
         self.current_uri = self.uri_split.replace('%v', str(self.index))
         self.sleep()
```

### Comparing `crawlist-0.0.9/crawlist/analyzers/request.py` & `crawlist-0.1.0/crawlist/analyzers/request.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/selector.py` & `crawlist-0.1.0/crawlist/analyzers/selector.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/trie.py` & `crawlist-0.1.0/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/analyzers/valid.py` & `crawlist-0.1.0/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/annotation.py` & `crawlist-0.1.0/crawlist/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/processings/action.py` & `crawlist-0.1.0/crawlist/processings/action.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist/processings/script.py` & `crawlist-0.1.0/crawlist/processings/script.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/crawlist.egg-info/PKG-INFO` & `crawlist-0.1.0/crawlist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.9
+Version: 0.1.0
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,15 +47,15 @@
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.
 
 ## installing
 You can use pip or pip3 to install the crawlist
 
 `pip install crawlist` or `pip3 install crawlist`
 
 If you have already installed crawlist, you may need to update to the latest version
@@ -112,11 +112,11 @@
     pager.webdriver.quit()
 
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the link below.
 
-[English](https://wwydev.gitbook.io/crawlist "English Document")
+[中文](https://wwydev.gitbook.io/crawlist-zh/ "中文文档")|[English](https://wwydev.gitbook.io/crawlist "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crawlist-0.0.9/crawlist.egg-info/SOURCES.txt` & `crawlist-0.1.0/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.9/setup.py` & `crawlist-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
```

