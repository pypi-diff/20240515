# Comparing `tmp/openbb_news-1.1.5.tar.gz` & `tmp/openbb_news-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_news-1.1.5.tar", max compression
+gzip compressed data, was "openbb_news-1.2.0.tar", max compression
```

## Comparing `openbb_news-1.1.5.tar` & `openbb_news-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      420 2024-04-17 12:33:20.501645 openbb_news-1.1.5/README.md
--rw-r--r--   0        0        0       29 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_news-1.1.5/openbb_news/py.typed
--rw-r--r--   0        0        0      440 2024-04-19 16:40:26.343120 openbb_news-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 openbb_news-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      293 2024-05-15 14:26:43.333826 openbb_news-1.2.0/README.md
+-rw-r--r--   0        0        0       29 2024-04-23 10:22:39.606101 openbb_news-1.2.0/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-23 10:22:39.606249 openbb_news-1.2.0/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740930 openbb_news-1.2.0/openbb_news/py.typed
+-rw-r--r--   0        0        0      466 2024-05-15 16:04:21.990645 openbb_news-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 openbb_news-1.2.0/PKG-INFO
```

### Comparing `openbb_news-1.1.5/openbb_news/news_router.py` & `openbb_news-1.2.0/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_news-1.1.5/PKG-INFO` & `openbb_news-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-news
-Version: 1.1.5
+Version: 1.2.0
 Summary: News extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB News Extension
 
 This extension provides news for the OpenBB Platform.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-news
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

