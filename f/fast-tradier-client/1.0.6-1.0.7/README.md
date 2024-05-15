# Comparing `tmp/fast_tradier_client-1.0.6.tar.gz` & `tmp/fast_tradier_client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-1.0.6.tar", last modified: Sat May 11 18:28:30 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.7.tar", last modified: Tue May 14 15:54:35 2024, max compression
```

## Comparing `fast_tradier_client-1.0.6.tar` & `fast_tradier_client-1.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11018 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10274 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.748004 fast_tradier_client-1.0.6/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16961 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16390 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.748004 fast_tradier_client-1.0.6/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     4096 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11018 2024-05-11 18:28:30.000000 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-11 18:28:30.000000 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 18:28:30.000000 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-11 18:28:30.000000 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-11 18:28:30.000000 fast_tradier_client-1.0.6/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 18:28:30.752004 fast_tradier_client-1.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-11 18:28:02.000000 fast_tradier_client-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.787577 fast_tradier_client-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11018 2024-05-14 15:54:35.787577 fast_tradier_client-1.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10274 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.779576 fast_tradier_client-1.0.7/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16961 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16390 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     4151 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 15:54:35.783576 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11018 2024-05-14 15:54:35.000000 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-14 15:54:35.000000 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 15:54:35.000000 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-14 15:54:35.000000 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-14 15:54:35.000000 fast_tradier_client-1.0.7/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 15:54:35.787577 fast_tradier_client-1.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-14 15:54:09.000000 fast_tradier_client-1.0.7/setup.py
```

### Comparing `fast_tradier_client-1.0.6/LICENSE` & `fast_tradier_client-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/PKG-INFO` & `fast_tradier_client-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.6/README.md` & `fast_tradier_client-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0.7/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0.7/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0.7/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0.7/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0.7/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0.7/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0.7/fast_tradier/models/account/AccountOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/market_data/Hlocv.py` & `fast_tradier_client-1.0.7/fast_tradier/models/market_data/Hlocv.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0.7/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0.7/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/trading/EquityOrder.py` & `fast_tradier_client-1.0.7/fast_tradier/models/trading/EquityOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/trading/OptionOrder.py` & `fast_tradier_client-1.0.7/fast_tradier/models/trading/OptionOrder.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,27 +82,26 @@
         Returns:
             Mapping[str, Any]: _description_
         """
         temp_result = self.model_dump(by_alias=True)
         result: Dict[str, Any] = {}
         for k, v in temp_result.items():
             result[k] = v
-
-        if len(self.option_legs) == 1:
-            result["option_symbol"] = self.option_legs[0].option_symbol
-            result["side"] = self.option_legs[0].side
-            result["quantity"] = self.option_legs[0].quantity
-            result["class"] = OptionOrderClass.SingleLeg
-        elif len(self.option_legs) > 1:
-            result["class"] = OptionOrderClass.MultiLegs
-            for i in range(len(self.option_legs)):
-                opt_item = self.option_legs[i]
-                symbol_key = f"option_symbol[{i}]"
-                result[symbol_key] = opt_item.option_symbol
-                side_key = f"side[{i}]"
-                result[side_key] = f"{opt_item.side}"
-                quant_key = f"quantity[{i}]"
-                result[quant_key] = f"{opt_item.quantity}"
+        if self.option_legs is not None and len(self.option_legs) > 0:
+            result["class"] = self.order_class
+            if len(self.option_legs) == 1:
+                result["option_symbol"] = self.option_legs[0].option_symbol
+                result["side"] = self.option_legs[0].side
+                result["quantity"] = self.option_legs[0].quantity
+            elif len(self.option_legs) > 1:
+                for i in range(len(self.option_legs)):
+                    opt_item = self.option_legs[i]
+                    symbol_key = f"option_symbol[{i}]"
+                    result[symbol_key] = opt_item.option_symbol
+                    side_key = f"side[{i}]"
+                    result[side_key] = f"{opt_item.side}"
+                    quant_key = f"quantity[{i}]"
+                    result[quant_key] = f"{opt_item.quantity}"
         else:
             raise Exception("option legs should not be empty")
 
         return result
```

### Comparing `fast_tradier_client-1.0.6/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0.7/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0.7/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0.7/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0.7/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0.7/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-1.0.6/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0.7/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-1.0.6/pyproject.toml` & `fast_tradier_client-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

