# Comparing `tmp/duckduckgo_search-5.3.1b1.tar.gz` & `tmp/duckduckgo_search-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.3.1b1.tar", last modified: Wed May  8 22:26:37 2024, max compression
+gzip compressed data, was "duckduckgo_search-6.0.0.tar", last modified: Tue May 14 17:07:33 2024, max compression
```

## Comparing `duckduckgo_search-5.3.1b1.tar` & `duckduckgo_search-6.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      765 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    42757 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 22:26:37.000000 duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:26:37.980471 duckduckgo_search-5.3.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:26:37.976471 duckduckgo_search-5.3.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 22:26:28.000000 duckduckgo_search-5.3.1b1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:33.353969 duckduckgo_search-6.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-05-14 17:07:33.353969 duckduckgo_search-6.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16623 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:33.349969 duckduckgo_search-6.0.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40878 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:33.353969 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 17:07:33.000000 duckduckgo_search-6.0.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:07:33.353969 duckduckgo_search-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:07:33.353969 duckduckgo_search-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/tests/test_duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-14 17:07:21.000000 duckduckgo_search-6.0.0/tests/test_duckduckgo_search_async.py
```

### Comparing `duckduckgo_search-5.3.1b1/LICENSE.md` & `duckduckgo_search-6.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.1b1/PKG-INFO` & `duckduckgo_search-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.1b1
+Version: 6.0.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,32 +19,29 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
+Requires-Dist: pyreqwest_impersonate>=0.4.5
+Requires-Dist: orjson>=3.10.3
 Provides-Extra: lxml
-Requires-Dist: lxml>=5.2.1; extra == "lxml"
-Provides-Extra: orjson
-Requires-Dist: orjson>=3.10.3; extra == "orjson"
+Requires-Dist: lxml>=5.2.2; extra == "lxml"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
-Requires-Dist: ruff>=0.4.3; extra == "dev"
+Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
+Requires-Dist: ruff>=0.4.4; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
-⚠️ Warning: it is better to use AsyncDDGS in asynchronous code</br>
-:bangbang: v5.0 brings breaking changes: all functions are now not generators, but return a list of dictionaries.
-
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
 * [Regions](#regions)
 * [DDGS and AsyncDDGS classes](#ddgs-and-asyncddgs-classes)
 * [Proxy](#proxy)
@@ -58,14 +55,18 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
+There is also a beta release that uses the `httpx` library:
+```python
+pip install -U duckduckgo_search==5.3.1b1
+```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
@@ -206,30 +207,28 @@
 
 results = DDGS().text("python programming", max_results=5)
 print(results)
 ```
 Here is an example of initializing the AsyncDDGS class:
 ```python3
 import asyncio
-import logging
 
 from duckduckgo_search import AsyncDDGS
 
 async def aget_results(word):
-    results = await AsyncDDGS(proxy=None).text(word, max_results=100)
+    results = await AsyncDDGS(proxy=None).atext(word, max_results=100)
     return results
 
 async def main():
     words = ["sun", "earth", "moon"]
     tasks = [aget_results(w) for w in words]
     results = await asyncio.gather(*tasks)
     print(results)
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main())
 ```
 
 [Go To TOP](#TOP)
 
 ## Proxy
 
@@ -290,15 +289,15 @@
 ***Example***
 ```python
 results = DDGS().text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 # Searching for pdf files
 results = DDGS().text('russia filetype:pdf', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 
 # async
-results = await AsyncDDGS().text('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().atext('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
@@ -313,15 +312,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().answers("sun")
 
 # async
-results = await AsyncDDGS().answers("sun")
+results = await AsyncDDGS().aanswers("sun")
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -371,15 +370,15 @@
     type_image=None,
     layout=None,
     license_image=None,
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().images('sun', region='wt-wt', safesearch='off', max_results=20)
+results = await AsyncDDGS().aimages('sun', region='wt-wt', safesearch='off', max_results=20)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -418,15 +417,15 @@
     timelimit="w",
     resolution="high",
     duration="medium",
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().videos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().avideos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
 ```python
@@ -451,15 +450,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().news(keywords="sun", region="wt-wt", safesearch="off", timelimit="m", max_results=20)
 
 # async
-results = await AsyncDDGS().news('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
+results = await AsyncDDGS().anews('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -499,15 +498,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().maps("school", place="Uganda", max_results=50)
 
 # async
-results = await AsyncDDGS().maps('shop', place="Baltimor", max_results=10)
+results = await AsyncDDGS().amaps('shop', place="Baltimor", max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -532,15 +531,15 @@
 ```python
 keywords = 'school'
 # also valid
 keywords = ['school', 'cat']
 results = DDGS().translate(keywords, to="de")
 
 # async
-results = await AsyncDDGS().translate('sun', to="de")
+results = await AsyncDDGS().atranslate('sun', to="de")
 ```
 
 [Go To TOP](#TOP)
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
@@ -559,11 +558,11 @@
     """
 ```
 ***Example***
 ```python3
 results = DDGS().suggestions("fly")
 
 # async
-results = await AsyncDDGS().suggestions('sun')
+results = await AsyncDDGS().asuggestions('sun')
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-5.3.1b1/README.md` & `duckduckgo_search-6.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
-⚠️ Warning: it is better to use AsyncDDGS in asynchronous code</br>
-:bangbang: v5.0 brings breaking changes: all functions are now not generators, but return a list of dictionaries.
-
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
 * [Regions](#regions)
 * [DDGS and AsyncDDGS classes](#ddgs-and-asyncddgs-classes)
 * [Proxy](#proxy)
@@ -23,14 +20,18 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
+There is also a beta release that uses the `httpx` library:
+```python
+pip install -U duckduckgo_search==5.3.1b1
+```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
@@ -171,30 +172,28 @@
 
 results = DDGS().text("python programming", max_results=5)
 print(results)
 ```
 Here is an example of initializing the AsyncDDGS class:
 ```python3
 import asyncio
-import logging
 
 from duckduckgo_search import AsyncDDGS
 
 async def aget_results(word):
-    results = await AsyncDDGS(proxy=None).text(word, max_results=100)
+    results = await AsyncDDGS(proxy=None).atext(word, max_results=100)
     return results
 
 async def main():
     words = ["sun", "earth", "moon"]
     tasks = [aget_results(w) for w in words]
     results = await asyncio.gather(*tasks)
     print(results)
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main())
 ```
 
 [Go To TOP](#TOP)
 
 ## Proxy
 
@@ -255,15 +254,15 @@
 ***Example***
 ```python
 results = DDGS().text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 # Searching for pdf files
 results = DDGS().text('russia filetype:pdf', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 
 # async
-results = await AsyncDDGS().text('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().atext('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
@@ -278,15 +277,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().answers("sun")
 
 # async
-results = await AsyncDDGS().answers("sun")
+results = await AsyncDDGS().aanswers("sun")
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -336,15 +335,15 @@
     type_image=None,
     layout=None,
     license_image=None,
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().images('sun', region='wt-wt', safesearch='off', max_results=20)
+results = await AsyncDDGS().aimages('sun', region='wt-wt', safesearch='off', max_results=20)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -383,15 +382,15 @@
     timelimit="w",
     resolution="high",
     duration="medium",
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().videos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().avideos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
 ```python
@@ -416,15 +415,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().news(keywords="sun", region="wt-wt", safesearch="off", timelimit="m", max_results=20)
 
 # async
-results = await AsyncDDGS().news('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
+results = await AsyncDDGS().anews('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -464,15 +463,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().maps("school", place="Uganda", max_results=50)
 
 # async
-results = await AsyncDDGS().maps('shop', place="Baltimor", max_results=10)
+results = await AsyncDDGS().amaps('shop', place="Baltimor", max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -497,15 +496,15 @@
 ```python
 keywords = 'school'
 # also valid
 keywords = ['school', 'cat']
 results = DDGS().translate(keywords, to="de")
 
 # async
-results = await AsyncDDGS().translate('sun', to="de")
+results = await AsyncDDGS().atranslate('sun', to="de")
 ```
 
 [Go To TOP](#TOP)
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
@@ -524,11 +523,11 @@
     """
 ```
 ***Example***
 ```python3
 results = DDGS().suggestions("fly")
 
 # async
-results = await AsyncDDGS().suggestions('sun')
+results = await AsyncDDGS().asuggestions('sun')
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-5.3.1b1/duckduckgo_search/cli.py` & `duckduckgo_search-6.0.0/duckduckgo_search/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from urllib.parse import unquote
 
 import click
-import httpx
+import pyreqwest_impersonate as pri
 
 from .duckduckgo_search import DDGS
-from .utils import _get_ssl_context, json_dumps
+from .utils import json_dumps
 from .version import __version__
 
 logger = logging.getLogger(__name__)
 
 COLORS = {
     0: "black",
     1: "red",
@@ -77,20 +77,20 @@
         .replace(" ", "")
     )
     return keywords
 
 
 def _download_file(url, dir_path, filename, proxy):
     try:
-        resp = httpx.get(url, proxy=proxy, timeout=10, follow_redirects=True, verify=_get_ssl_context())
-        resp.raise_for_status()
-        with open(os.path.join(dir_path, filename[:200]), "wb") as file:
-            file.write(resp.content)
+        resp = pri.Client(proxy=proxy, impersonate="chrome_124", timeout=10, verify=False).get(url)
+        if resp.status_code == 200:
+            with open(os.path.join(dir_path, filename[:200]), "wb") as file:
+                file.write(resp.content)
     except Exception as ex:
-        logger.info(f"download_file url={url} {type(ex).__name__} {ex}")
+        logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
 def _download_results(keywords, results, images=False, proxy=None, threads=None):
     path_type = "images" if images else "text"
     path = f"{path_type}_{keywords}_{datetime.now():%Y%m%d_%H%M%S}"
     os.makedirs(path, exist_ok=True)
```

### Comparing `duckduckgo_search-5.3.1b1/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-6.0.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,137 @@
-import asyncio
 import logging
 import warnings
 from concurrent.futures import ThreadPoolExecutor
-from contextlib import suppress
 from datetime import datetime, timezone
 from decimal import Decimal
-from functools import cached_property, partial
+from functools import cached_property
 from itertools import cycle, islice
+from threading import Event
 from types import TracebackType
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Dict, List, Optional, Tuple, Type, Union, cast
 
-import httpx
+import pyreqwest_impersonate as pri  # type: ignore
 
 try:
-    from lxml.html import Element, document_fromstring
+    from lxml.etree import _Element
     from lxml.html import HTMLParser as LHTMLParser
+    from lxml.html import document_fromstring
 
     LXML_AVAILABLE = True
 except ImportError:
     LXML_AVAILABLE = False
 
 from .exceptions import DuckDuckGoSearchException, RatelimitException, TimeoutException
 from .utils import (
     _calculate_distance,
     _extract_vqd,
-    _get_headers,
-    _get_ssl_context,
     _normalize,
     _normalize_url,
     _text_extract_json,
     json_loads,
 )
 
-logger = logging.getLogger("duckduckgo_search.AsyncDDGS")
+logger = logging.getLogger("duckduckgo_search.DDGS")
 
 
-class AsyncDDGS:
-    """DuckDuckgo_search async class to get search results from duckduckgo.com."""
+class DDGS:
+    """DuckDuckgo_search class to get search results from duckduckgo.com."""
 
-    _executor: Optional[ThreadPoolExecutor] = None
+    _executor: ThreadPoolExecutor = ThreadPoolExecutor()
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxy: Optional[str] = None,
         proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
-        """Initialize the AsyncDDGS object.
+        """Initialize the DDGS object.
 
         Args:
             headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
             proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
                 example: "http://user:pass@example.com:3128". Defaults to None.
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
         self.proxy: Optional[str] = proxy
         assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
         if not proxy and proxies:
             warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
             self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
-        self._aclient = httpx.AsyncClient(
-            headers=_get_headers() if headers is None else headers,
+        self.headers = headers if headers else {}
+        self.headers["Referer"] = "https://duckduckgo.com/"
+        self.client = pri.Client(
+            headers=self.headers,
             proxy=self.proxy,
             timeout=timeout,
+            cookie_store=True,
+            referer=True,
+            impersonate="chrome_124",
             follow_redirects=False,
-            http2=True,
-            verify=_get_ssl_context(),
+            verify=False,
         )
-        self._aclient.headers["Referer"] = "https://duckduckgo.com/"
-        self._exception_event = asyncio.Event()
+        self._exception_event = Event()
 
-    async def __aenter__(self) -> "AsyncDDGS":
+    def __enter__(self) -> "DDGS":
         return self
 
-    async def __aexit__(
+    def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._aclient.__aexit__(exc_type, exc_val, exc_tb)
-
-    def __del__(self) -> None:
-        if hasattr(self, "_aclient") and self._aclient.is_closed is False:
-            with suppress(RuntimeError, RuntimeWarning):
-                asyncio.create_task(self._aclient.aclose())
+        pass
 
     @cached_property
     def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
         return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
-    @classmethod
-    def _get_executor(cls, max_workers: int = 1) -> ThreadPoolExecutor:
-        """Get ThreadPoolExecutor. Default max_workers=1, because >=2 leads to a big overhead"""
-        if cls._executor is None:
-            cls._executor = ThreadPoolExecutor(max_workers=max_workers)
-        return cls._executor
-
-    @property
-    def executor(cls) -> ThreadPoolExecutor:
-        return cls._get_executor()
-
-    async def _aget_url(
+    def _get_url(
         self,
         method: str,
         url: str,
-        content: Optional[Union[str, bytes]] = None,
-        data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, str]] = None,
+        content: Optional[bytes] = None,
+        data: Optional[Union[Dict[str, str], bytes]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise DuckDuckGoSearchException("Exception occurred in previous call.")
         try:
-            resp = await self._aclient.request(method, url, content=content, data=data, params=params)
-        except httpx.TimeoutException as ex:
-            self._exception_event.set()
-            raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
+            resp = self.client.request(method, url, params=params, content=content, data=data)
         except Exception as ex:
             self._exception_event.set()
+            if "time" in str(ex).lower():
+                raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
             raise DuckDuckGoSearchException(f"{url} {type(ex).__name__}: {ex}") from ex
+        logger.debug(f"_get_url() {resp.url} {resp.status_code} {len(resp.content)}")
         if resp.status_code == 200:
-            return resp.content
+            return cast(bytes, resp.content)
         self._exception_event.set()
         if resp.status_code in (202, 301, 403):
             raise RatelimitException(f"{resp.url} {resp.status_code} Ratelimit")
-        raise DuckDuckGoSearchException(f"{resp.url} return None. {params=} {data=}")
+        raise DuckDuckGoSearchException(f"{resp.url} return None. {params=} {content=} {data=}")
 
-    async def _aget_vqd(self, keywords: str) -> str:
+    def _get_vqd(self, keywords: str) -> str:
         """Get vqd value for a search query."""
-        resp_content = await self._aget_url("POST", "https://duckduckgo.com", data={"q": keywords})
+        resp_content = self._get_url("POST", "https://duckduckgo.com", data={"q": keywords})
         return _extract_vqd(resp_content, keywords)
 
-    async def text(
+    def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         backend: str = "api",
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params.
+        """DuckDuckGo text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             backend: api, html, lite. Defaults to api.
@@ -164,30 +149,30 @@
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         if LXML_AVAILABLE is False and backend != "api":
             backend = "api"
             warnings.warn("lxml is not installed. Using backend='api'.", stacklevel=2)
 
         if backend == "api":
-            results = await self._text_api(keywords, region, safesearch, timelimit, max_results)
+            results = self._text_api(keywords, region, safesearch, timelimit, max_results)
         elif backend == "html":
-            results = await self._text_html(keywords, region, safesearch, timelimit, max_results)
+            results = self._text_html(keywords, region, safesearch, timelimit, max_results)
         elif backend == "lite":
-            results = await self._text_lite(keywords, region, timelimit, max_results)
+            results = self._text_lite(keywords, region, timelimit, max_results)
         return results
 
-    async def _text_api(
+    def _text_api(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params.
+        """DuckDuckGo text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
@@ -198,15 +183,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         payload = {
             "q": keywords,
             "kl": region,
             "l": region,
             "p": "",
             "s": "0",
@@ -221,61 +206,56 @@
             payload["ex"] = "-2"
         elif safesearch == "on":  # strict
             payload["p"] = "1"
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_api_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_api_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://links.duckduckgo.com/d.js", params=payload)
+            resp_content = self._get_url("GET", "https://links.duckduckgo.com/d.js", params=payload)
             page_data = _text_extract_json(resp_content, keywords)
-
+            page_results = []
             for row in page_data:
                 href = row.get("u", None)
                 if href and href not in cache and href != f"http://www.google.com/search?q={keywords}":
                     cache.add(href)
                     body = _normalize(row["a"])
                     if body:
-                        priority += 1
                         result = {
                             "title": _normalize(row["t"]),
                             "href": _normalize_url(href),
                             "body": body,
                         }
-                        results[priority] = result
+                        page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_api_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_api_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_api_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def _text_html(
+    def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params.
+        """DuckDuckGo text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
@@ -286,89 +266,86 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._aclient.headers["Referer"] = "https://html.duckduckgo.com/"
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "q": keywords,
             "kl": region,
             "p": safesearch_base[safesearch.lower()],
             "o": "json",
             "api": "d.js",
         }
         if timelimit:
             payload["df"] = timelimit
         if max_results and max_results > 20:
-            vqd = await self._aget_vqd(keywords)
+            vqd = self._get_vqd(keywords)
             payload["vqd"] = vqd
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_html_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_html_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("POST", "https://html.duckduckgo.com/html", data=payload)
+            resp_content = self._get_url("POST", "https://html.duckduckgo.com/html", data=payload)
             if b"No  results." in resp_content:
-                return
-
-            tree: Element = await asyncio.get_running_loop().run_in_executor(
-                self.executor, partial(document_fromstring, resp_content, self.parser)
-            )
+                return []
 
-            for e in tree.xpath("//div[h2]"):
-                href = e.xpath("./a/@href")
-                href = href[0] if href else None
-                if (
-                    href
-                    and href not in cache
-                    and not href.startswith(
-                        ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
-                    )
-                ):
-                    cache.add(href)
-                    title = e.xpath("./h2/a/text()")
-                    body = e.xpath("./a//text()")
-
-                    priority += 1
-                    result = {
-                        "title": _normalize(title[0]),
-                        "href": _normalize_url(href),
-                        "body": _normalize("".join(body)),
-                    }
-                    results[priority] = result
+            page_results = []
+            tree = document_fromstring(resp_content, self.parser)
+            elements = tree.xpath("//div[h2]")
+            if not isinstance(elements, List):
+                return []
+            for e in elements:
+                if isinstance(e, _Element):
+                    hrefxpath = e.xpath("./a/@href")
+                    href = str(hrefxpath[0]) if isinstance(hrefxpath, List) else None
+                    if (
+                        href
+                        and href not in cache
+                        and not href.startswith(
+                            ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
+                        )
+                    ):
+                        cache.add(href)
+                        titlexpath = e.xpath("./h2/a/text()")
+                        title = str(titlexpath[0]) if isinstance(titlexpath, List) else ""
+                        bodyxpath = e.xpath("./a//text()")
+                        body = "".join(str(x) for x in bodyxpath) if isinstance(bodyxpath, List) else ""
+                        result = {
+                            "title": _normalize(title),
+                            "href": _normalize_url(href),
+                            "body": _normalize(body),
+                        }
+                        page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_html_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_html_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_html_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def _text_lite(
+    def _text_lite(
         self,
         keywords: str,
         region: str = "wt-wt",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params.
+        """DuckDuckGo text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
@@ -378,81 +355,81 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._aclient.headers["Referer"] = "https://lite.duckduckgo.com/"
         payload = {
             "q": keywords,
             "o": "json",
             "api": "d.js",
             "kl": region,
         }
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_lite_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_lite_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
+            resp_content = self._get_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
             if b"No more results." in resp_content:
-                return
+                return []
 
-            tree: Element = await asyncio.get_running_loop().run_in_executor(
-                self.executor, partial(document_fromstring, resp_content, self.parser)
-            )
+            page_results = []
+            tree = document_fromstring(resp_content, self.parser)
+            elements = tree.xpath("//table[last()]//tr")
+            if not isinstance(elements, List):
+                return []
 
-            data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
+            data = zip(cycle(range(1, 5)), elements)
             for i, e in data:
-                if i == 1:
-                    href = e.xpath(".//a//@href")
-                    href = href[0] if href else None
-                    if (
-                        href is None
-                        or href in cache
-                        or href.startswith(("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain"))
-                    ):
-                        [next(data, None) for _ in range(3)]  # skip block(i=1,2,3,4)
-                    else:
-                        cache.add(href)
-                        title = e.xpath(".//a//text()")[0]
-                elif i == 2:
-                    body = e.xpath(".//td[@class='result-snippet']//text()")
-                    body = "".join(body).strip()
-                elif i == 3:
-                    priority += 1
-                    result = {
-                        "title": _normalize(title),
-                        "href": _normalize_url(href),
-                        "body": _normalize(body),
-                    }
-                    results[priority] = result
+                if isinstance(e, _Element):
+                    if i == 1:
+                        hrefxpath = e.xpath(".//a//@href")
+                        href = str(hrefxpath[0]) if hrefxpath and isinstance(hrefxpath, List) else None
+                        if (
+                            href is None
+                            or href in cache
+                            or href.startswith(
+                                ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
+                            )
+                        ):
+                            [next(data, None) for _ in range(3)]  # skip block(i=1,2,3,4)
+                        else:
+                            cache.add(href)
+                            titlexpath = e.xpath(".//a//text()")
+                            title = str(titlexpath[0]) if isinstance(titlexpath, List) else ""
+                    elif i == 2:
+                        bodyxpath = e.xpath(".//td[@class='result-snippet']//text()")
+                        body = "".join(str(x) for x in bodyxpath) if isinstance(bodyxpath, List) else ""
+                        if href:
+                            result = {
+                                "title": _normalize(title),
+                                "href": _normalize_url(href),
+                                "body": _normalize(body),
+                            }
+                            page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_lite_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_lite_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_lite_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def images(
+    def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         size: Optional[str] = None,
         color: Optional[str] = None,
@@ -486,15 +463,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "1", "off": "-1"}
         timelimit = f"time:{timelimit}" if timelimit else ""
         size = f"size:{size}" if size else ""
         color = f"color:{color}" if color else ""
         type_image = f"type:{type_image}" if type_image else ""
         layout = f"layout:{layout}" if layout else ""
@@ -505,57 +482,52 @@
             "q": keywords,
             "vqd": vqd,
             "f": f"{timelimit},{size},{color},{type_image},{layout},{license_image}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 600
+        results: List[Dict[str, str]] = []
 
-        async def _images_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _images_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/i.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/i.js", params=payload)
             resp_json = json_loads(resp_content)
 
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 image_url = row.get("image")
                 if image_url and image_url not in cache:
                     cache.add(image_url)
-                    priority += 1
                     result = {
                         "title": row["title"],
                         "image": _normalize_url(image_url),
                         "thumbnail": _normalize_url(row["thumbnail"]),
                         "url": _normalize_url(row["url"]),
                         "height": row["height"],
                         "width": row["width"],
                         "source": row["source"],
                     }
-                    results[priority] = result
+                    page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_images_page(0, page=0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_images_page(s, i)) for i, s in enumerate(range(100, max_results, 100), start=1)
-            )
+            slist.extend(range(100, max_results, 100))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_images_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def videos(
+    def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         resolution: Optional[str] = None,
         duration: Optional[str] = None,
@@ -580,15 +552,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         timelimit = f"publishedAfter:{timelimit}" if timelimit else ""
         resolution = f"videoDefinition:{resolution}" if resolution else ""
         duration = f"videoDuration:{duration}" if duration else ""
         license_videos = f"videoLicense:{license_videos}" if license_videos else ""
         payload = {
@@ -597,47 +569,42 @@
             "q": keywords,
             "vqd": vqd,
             "f": f"{timelimit},{resolution},{duration},{license_videos}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 700
+        results: List[Dict[str, str]] = []
 
-        async def _videos_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _videos_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/v.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/v.js", params=payload)
             resp_json = json_loads(resp_content)
 
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 if row["content"] not in cache:
                     cache.add(row["content"])
-                    priority += 1
-                    results[priority] = row
+                    page_results.append(row)
+            return page_results
 
-        tasks = [asyncio.create_task(_videos_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 400)
-            tasks.extend(
-                asyncio.create_task(_videos_page(s, i)) for i, s in enumerate(range(59, max_results, 59), start=1)
-            )
+            slist.extend(range(59, max_results, 59))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_videos_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def news(
+    def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
@@ -656,70 +623,65 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "l": region,
             "o": "json",
             "noamp": "1",
             "q": keywords,
             "vqd": vqd,
             "p": safesearch_base[safesearch.lower()],
         }
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 700
+        results: List[Dict[str, str]] = []
 
-        async def _news_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _news_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/news.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/news.js", params=payload)
             resp_json = json_loads(resp_content)
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 if row["url"] not in cache:
                     cache.add(row["url"])
                     image_url = row.get("image", None)
-                    priority += 1
                     result = {
                         "date": datetime.fromtimestamp(row["date"], timezone.utc).isoformat(),
                         "title": row["title"],
                         "body": _normalize(row["excerpt"]),
                         "url": _normalize_url(row["url"]),
                         "image": _normalize_url(image_url),
                         "source": row["source"],
                     }
-                    results[priority] = result
+                    page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_news_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 200)
-            tasks.extend(
-                asyncio.create_task(_news_page(s, i)) for i, s in enumerate(range(29, max_results, 29), start=1)
-            )
+            slist.extend(range(29, max_results, 29))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_news_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def answers(self, keywords: str) -> List[Dict[str, str]]:
+    def answers(self, keywords: str) -> List[Dict[str, str]]:
         """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query,
 
         Returns:
             List of dictionaries with instant answers results.
@@ -731,15 +693,15 @@
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": f"what is {keywords}",
             "format": "json",
         }
-        resp_content = await self._aget_url("GET", "https://api.duckduckgo.com/", params=payload)
+        resp_content = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         page_data = json_loads(resp_content)
 
         results = []
         answer = page_data.get("AbstractText")
         url = page_data.get("AbstractURL")
         if answer:
             results.append(
@@ -752,15 +714,15 @@
             )
 
         # related
         payload = {
             "q": f"{keywords}",
             "format": "json",
         }
-        resp_content = await self._aget_url("GET", "https://api.duckduckgo.com/", params=payload)
+        resp_content = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         resp_json = json_loads(resp_content)
         page_data = resp_json.get("RelatedTopics", [])
 
         for row in page_data:
             topic = row.get("Name")
             if not topic:
                 icon = row["Icon"].get("URL")
@@ -782,15 +744,15 @@
                             "topic": topic,
                             "url": subrow["FirstURL"],
                         }
                     )
 
         return results
 
-    async def suggestions(self, keywords: str, region: str = "wt-wt") -> List[Dict[str, str]]:
+    def suggestions(self, keywords: str, region: str = "wt-wt") -> List[Dict[str, str]]:
         """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
         Returns:
@@ -803,19 +765,19 @@
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
             "kl": region,
         }
-        resp_content = await self._aget_url("GET", "https://duckduckgo.com/ac/", params=payload)
+        resp_content = self._get_url("GET", "https://duckduckgo.com/ac/", params=payload)
         page_data = json_loads(resp_content)
         return [r for r in page_data]
 
-    async def maps(
+    def maps(
         self,
         keywords: str,
         place: Optional[str] = None,
         street: Optional[str] = None,
         city: Optional[str] = None,
         county: Optional[str] = None,
         state: Optional[str] = None,
@@ -849,15 +811,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         # if longitude and latitude are specified, skip the request about bbox to the nominatim api
         if latitude and longitude:
             lat_t = Decimal(latitude.replace(",", "."))
             lat_b = Decimal(latitude.replace(",", "."))
             lon_l = Decimal(longitude.replace(",", "."))
             lon_r = Decimal(longitude.replace(",", "."))
@@ -885,37 +847,37 @@
                 if state:
                     params["state"] = state
                 if country:
                     params["country"] = country
                 if postalcode:
                     params["postalcode"] = postalcode
             # request nominatim api to get coordinates box
-            resp_content = await self._aget_url(
+            resp_content = self._get_url(
                 "GET",
                 "https://nominatim.openstreetmap.org/search.php",
                 params=params,
             )
             if resp_content == b"[]":
-                raise DuckDuckGoSearchException("maps() Сoordinates are not found, check function parameters.")
+                raise DuckDuckGoSearchException("maps() Coordinates are not found, check function parameters.")
             resp_json = json_loads(resp_content)
             coordinates = resp_json[0]["boundingbox"]
             lat_t, lon_l = Decimal(coordinates[1]), Decimal(coordinates[2])
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
 
         # if a radius is specified, expand the search square
         lat_t += Decimal(radius) * Decimal(0.008983)
         lat_b -= Decimal(radius) * Decimal(0.008983)
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
-        logger.info(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
+        logger.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         cache = set()
         results: List[Dict[str, str]] = []
 
-        async def _maps_page(
+        def _maps_page(
             bbox: Tuple[Decimal, Decimal, Decimal, Decimal],
         ) -> Optional[List[Dict[str, str]]]:
             if max_results and len(results) >= max_results:
                 return None
             lat_t, lon_l, lat_b, lon_r = bbox
             params = {
                 "q": keywords,
@@ -925,15 +887,15 @@
                 "mkexp": "b",
                 "wiki_info": "1",
                 "is_requery": "1",
                 "bbox_tl": f"{lat_t},{lon_l}",
                 "bbox_br": f"{lat_b},{lon_r}",
                 "strict_bbox": "1",
             }
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/local.js", params=params)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/local.js", params=params)
             resp_json = json_loads(resp_content)
             page_data = resp_json.get("results", [])
 
             page_results = []
             for res in page_data:
                 r_name = f'{res["name"]} {res["address"]}'
                 if r_name in cache:
@@ -954,53 +916,57 @@
                         "hours": res["hours"] or "",
                         "category": res["ddg_category"] or "",
                         "facebook": f"www.facebook.com/profile.php?id={x}" if (x := res["facebook_id"]) else "",
                         "instagram": f"https://www.instagram.com/{x}" if (x := res["instagram_id"]) else "",
                         "twitter": f"https://twitter.com/{x}" if (x := res["twitter_id"]) else "",
                     }
                     page_results.append(result)
-
             return page_results
 
         # search squares (bboxes)
         start_bbox = (lat_t, lon_l, lat_b, lon_r)
         work_bboxes = [start_bbox]
         while work_bboxes:
             queue_bboxes = []  # for next iteration, at the end of the iteration work_bboxes = queue_bboxes
             tasks = []
             for bbox in work_bboxes:
-                tasks.append(asyncio.create_task(_maps_page(bbox)))
+                tasks.append(bbox)
                 # if distance between coordinates > 1, divide the square into 4 parts and save them in queue_bboxes
                 if _calculate_distance(lat_t, lon_l, lat_b, lon_r) > 1:
                     lat_t, lon_l, lat_b, lon_r = bbox
                     lat_middle = (lat_t + lat_b) / 2
                     lon_middle = (lon_l + lon_r) / 2
                     bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
                     bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
                     bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
                     bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
                     queue_bboxes.extend([bbox1, bbox2, bbox3, bbox4])
 
             # gather tasks using asyncio.wait_for and timeout
-            with suppress(Exception):
-                work_bboxes_results = await asyncio.gather(*[asyncio.wait_for(task, timeout=10) for task in tasks])
+            work_bboxes_results = []
+            try:
+                for r in self._executor.map(_maps_page, tasks):
+                    if r:
+                        work_bboxes_results.extend(r)
+            except Exception as e:
+                raise e
 
             for x in work_bboxes_results:
                 if isinstance(x, list):
                     results.extend(x)
                 elif isinstance(x, dict):
                     results.append(x)
 
             work_bboxes = queue_bboxes
             if not max_results or len(results) >= max_results or len(work_bboxes_results) == 0:
                 break
 
         return list(islice(results, max_results))
 
-    async def translate(
+    def translate(
         self, keywords: Union[List[str], str], from_: Optional[str] = None, to: str = "en"
     ) -> List[Dict[str, str]]:
         """DuckDuckGo translate.
 
         Args:
             keywords: string or list of strings to translate.
             from_: translate from (defaults automatically). Defaults to None.
@@ -1012,42 +978,39 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd("translate")
+        vqd = self._get_vqd("translate")
 
         payload = {
             "vqd": vqd,
             "query": "translate",
             "to": to,
         }
         if from_:
             payload["from"] = from_
 
-        results = []
-
-        async def _translate_keyword(keyword: str) -> None:
-            resp_content = await self._aget_url(
+        def _translate_keyword(keyword: str) -> Dict[str, str]:
+            resp_content = self._get_url(
                 "POST",
                 "https://duckduckgo.com/translation.js",
                 params=payload,
-                content=keyword,
+                content=keyword.encode(),
             )
-            page_data = json_loads(resp_content)
+            page_data: Dict[str, str] = json_loads(resp_content)
             page_data["original"] = keyword
-            results.append(page_data)
+            return page_data
 
         if isinstance(keywords, str):
             keywords = [keywords]
-        tasks = [asyncio.create_task(_translate_keyword(keyword)) for keyword in keywords]
+
+        results = []
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_translate_keyword, keywords):
+                results.append(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
         return results
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-6.0.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.1b1
+Version: 6.0.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -19,32 +19,29 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
-Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
+Requires-Dist: pyreqwest_impersonate>=0.4.5
+Requires-Dist: orjson>=3.10.3
 Provides-Extra: lxml
-Requires-Dist: lxml>=5.2.1; extra == "lxml"
-Provides-Extra: orjson
-Requires-Dist: orjson>=3.10.3; extra == "orjson"
+Requires-Dist: lxml>=5.2.2; extra == "lxml"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: pytest>=8.2.0; extra == "dev"
-Requires-Dist: ruff>=0.4.3; extra == "dev"
+Requires-Dist: pytest-asyncio>=0.23.6; extra == "dev"
+Requires-Dist: ruff>=0.4.4; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive.
 
-⚠️ Warning: it is better to use AsyncDDGS in asynchronous code</br>
-:bangbang: v5.0 brings breaking changes: all functions are now not generators, but return a list of dictionaries.
-
 ## Table of Contents
 * [Install](#install)
 * [CLI version](#cli-version)
 * [Duckduckgo search operators](#duckduckgo-search-operators)
 * [Regions](#regions)
 * [DDGS and AsyncDDGS classes](#ddgs-and-asyncddgs-classes)
 * [Proxy](#proxy)
@@ -58,14 +55,18 @@
 * [7. translate() - translation](#7-translate---translation-by-duckduckgocom)
 * [8. suggestions() - suggestions](#8-suggestions---suggestions-by-duckduckgocom)
 
 ## Install
 ```python
 pip install -U duckduckgo_search
 ```
+There is also a beta release that uses the `httpx` library:
+```python
+pip install -U duckduckgo_search==5.3.1b1
+```
 > [!NOTE]
 > you can install lxml to use the `text` function with `backend='html'` or `backend='lite'` (size ≈ 12Mb)</br>
 > `pip install -U duckduckgo_search[lxml]`
 
 ## CLI version
 
 ```python3
@@ -206,30 +207,28 @@
 
 results = DDGS().text("python programming", max_results=5)
 print(results)
 ```
 Here is an example of initializing the AsyncDDGS class:
 ```python3
 import asyncio
-import logging
 
 from duckduckgo_search import AsyncDDGS
 
 async def aget_results(word):
-    results = await AsyncDDGS(proxy=None).text(word, max_results=100)
+    results = await AsyncDDGS(proxy=None).atext(word, max_results=100)
     return results
 
 async def main():
     words = ["sun", "earth", "moon"]
     tasks = [aget_results(w) for w in words]
     results = await asyncio.gather(*tasks)
     print(results)
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main())
 ```
 
 [Go To TOP](#TOP)
 
 ## Proxy
 
@@ -290,15 +289,15 @@
 ***Example***
 ```python
 results = DDGS().text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 # Searching for pdf files
 results = DDGS().text('russia filetype:pdf', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 
 # async
-results = await AsyncDDGS().text('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().atext('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
@@ -313,15 +312,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().answers("sun")
 
 # async
-results = await AsyncDDGS().answers("sun")
+results = await AsyncDDGS().aanswers("sun")
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -371,15 +370,15 @@
     type_image=None,
     layout=None,
     license_image=None,
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().images('sun', region='wt-wt', safesearch='off', max_results=20)
+results = await AsyncDDGS().aimages('sun', region='wt-wt', safesearch='off', max_results=20)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -418,15 +417,15 @@
     timelimit="w",
     resolution="high",
     duration="medium",
     max_results=100,
 )
 
 # async
-results = await AsyncDDGS().videos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
+results = await AsyncDDGS().avideos('sun', region='wt-wt', safesearch='off', timelimit='y', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
 ```python
@@ -451,15 +450,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().news(keywords="sun", region="wt-wt", safesearch="off", timelimit="m", max_results=20)
 
 # async
-results = await AsyncDDGS().news('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
+results = await AsyncDDGS().anews('sun', region='wt-wt', safesearch='off', timelimit='d', max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -499,15 +498,15 @@
     """
 ```
 ***Example***
 ```python
 results = DDGS().maps("school", place="Uganda", max_results=50)
 
 # async
-results = await AsyncDDGS().maps('shop', place="Baltimor", max_results=10)
+results = await AsyncDDGS().amaps('shop', place="Baltimor", max_results=10)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -532,15 +531,15 @@
 ```python
 keywords = 'school'
 # also valid
 keywords = ['school', 'cat']
 results = DDGS().translate(keywords, to="de")
 
 # async
-results = await AsyncDDGS().translate('sun', to="de")
+results = await AsyncDDGS().atranslate('sun', to="de")
 ```
 
 [Go To TOP](#TOP)
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
@@ -559,11 +558,11 @@
     """
 ```
 ***Example***
 ```python3
 results = DDGS().suggestions("fly")
 
 # async
-results = await AsyncDDGS().suggestions('sun')
+results = await AsyncDDGS().asuggestions('sun')
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-5.3.1b1/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-6.0.0/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 duckduckgo_search.egg-info/PKG-INFO
 duckduckgo_search.egg-info/SOURCES.txt
 duckduckgo_search.egg-info/dependency_links.txt
 duckduckgo_search.egg-info/entry_points.txt
 duckduckgo_search.egg-info/requires.txt
 duckduckgo_search.egg-info/top_level.txt
 tests/test_cli.py
-tests/test_duckduckgo_search.py
+tests/test_duckduckgo_search.py
+tests/test_duckduckgo_search_async.py
```

### Comparing `duckduckgo_search-5.3.1b1/pyproject.toml` & `duckduckgo_search-6.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -24,39 +24,38 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "click>=8.1.7",  
-    "httpx[brotli, http2, socks]>=0.27.0",
+    "click>=8.1.7",
+    "pyreqwest_impersonate>=0.4.5",
+    "orjson>=3.10.3",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
 ddgs = "duckduckgo_search.cli:safe_entry_point"
 
 [tool.setuptools.dynamic]
 version = {attr = "duckduckgo_search.version.__version__"}
 
 [project.optional-dependencies]
 lxml = [
-    "lxml>=5.2.1",
-]
-orjson = [
-    "orjson>=3.10.3",
+    "lxml>=5.2.2",
 ]
 dev = [
     "mypy>=1.10.0",
     "pytest>=8.2.0",
-    "ruff>=0.4.3",
+    "pytest-asyncio>=0.23.6",
+    "ruff>=0.4.4",
 ]
 
 [tool.ruff]
 line-length = 120
 exclude = ["tests"]
 
 [tool.ruff.lint]
@@ -66,15 +65,15 @@
     "UP",  # pyupgrade
     "B",  # flake8-bugbear
     "SIM",  # flake8-simplify
     "I",  # isort
 ]
 ignore = ["D100"]
 
-[tool.ruff.per-file-ignores]
-"utils.py" = ["E501"]
-
 [tool.mypy]
 python_version = "3.8"
 strict = true
 exclude = ['cli\.py$', '__main__\.py$', "tests/", "build/"]
 
+[[tool.mypy.overrides]]
+module = "curl_cffi"
+ignore_missing_imports = true
```

### Comparing `duckduckgo_search-5.3.1b1/tests/test_cli.py` & `duckduckgo_search-6.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.1b1/tests/test_duckduckgo_search.py` & `duckduckgo_search-6.0.0/tests/test_duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 def test_context_manager():
     with DDGS() as ddgs:
         results = ddgs.news("cars", max_results=30)
         assert 27 <= len(results) <= 30
 
 
 def test_text():
-    results = DDGS().text("cat", max_results=30)
-    assert 27 <= len(results) <= 30
-
-
-def test_text_params():
     results = DDGS().text("cat", safesearch="off", timelimit="m", max_results=30)
     assert 27 <= len(results) <= 30
 
 
 def test_text_html():
     results = DDGS().text("eagle", backend="html", max_results=30)
     assert 27 <= len(results) <= 30
```

