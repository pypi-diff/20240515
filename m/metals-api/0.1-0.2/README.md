# Comparing `tmp/metals_api-0.1.tar.gz` & `tmp/metals_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metals_api-0.1.tar", last modified: Tue May 14 18:42:48 2024, max compression
+gzip compressed data, was "metals_api-0.2.tar", last modified: Tue May 14 20:25:20 2024, max compression
```

## Comparing `metals_api-0.1.tar` & `metals_api-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:42:48.486046 metals_api-0.1/
--rw-rw-rw-   0        0        0     4174 2024-05-14 18:42:48.486046 metals_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3558 2024-05-14 18:39:59.000000 metals_api-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:42:48.462047 metals_api-0.1/metals_api/
--rw-rw-rw-   0        0        0       79 2024-05-14 18:40:20.000000 metals_api-0.1/metals_api/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-13 19:49:31.000000 metals_api-0.1/metals_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:42:48.484049 metals_api-0.1/metals_api.egg-info/
--rw-rw-rw-   0        0        0     4174 2024-05-14 18:42:48.000000 metals_api-0.1/metals_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-14 18:42:48.000000 metals_api-0.1/metals_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:42:48.000000 metals_api-0.1/metals_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:42:48.000000 metals_api-0.1/metals_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:42:48.487046 metals_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      971 2024-05-14 18:42:20.000000 metals_api-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.606725 metals_api-0.2/
+-rw-rw-rw-   0        0        0     4585 2024-05-14 20:25:20.605726 metals_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3969 2024-05-14 20:15:22.000000 metals_api-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.536726 metals_api-0.2/metals_api/
+-rw-rw-rw-   0        0        0       79 2024-05-14 18:40:20.000000 metals_api-0.2/metals_api/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-05-14 20:22:28.000000 metals_api-0.2/metals_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:25:20.603726 metals_api-0.2/metals_api.egg-info/
+-rw-rw-rw-   0        0        0     4585 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 20:25:20.000000 metals_api-0.2/metals_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 20:25:20.607728 metals_api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      971 2024-05-14 20:13:44.000000 metals_api-0.2/setup.py
```

### Comparing `metals_api-0.1/PKG-INFO` & `metals_api-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metals_api
-Version: 0.1
+Version: 0.2
 Summary: A Python package to get the latest metals prices from the Metals-API
 Home-page: https://github.com/Zyla-Labs/pypi-metals-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: metals-api,precious metals api,metals api,metals, precious metals,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -27,19 +27,25 @@
 
 ## Supported Symbols
 
 Explore a wide range of supported symbols, including gold, silver, platinum, palladium, and various others. From LBMA Gold to LME Steel, we cover it all. [View Symbols](https://www.metals-api.com/symbols)
 
 ## Available Endpoints
 
-The Metals-API API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+The Metals-API API comes with multiple endpoints, each providing different functionality. However, in this section, we will focus on the Latest Rates endpoint, Historical Rates and Times Series
 
 1. **Latest Rates Endpoint**
    - Returns real-time exchange rate data for all available or a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
 
+2. **Historical Rates Endpoint**
+   - Returns historical exchange rate data for a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
+
+3. **Time-Series Data Endpoint**
+   - Returns daily historical exchange rate data between two specified dates for all available or a specific set of currencies. (The date limits per API request depend on the acquired plan).
+
 ## Documentation
 
 For detailed information on API endpoints, usage, and integration guidelines, check our [API Documentation](https://www.metals-api.com/documentation).
 
 Start using Metals-API today for unparalleled access to precious metals data. Visit [Metals-API.com](https://metals-api.com) and integrate in just minutes!
```

### Comparing `metals_api-0.1/README.md` & `metals_api-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,25 @@
 
 ## Supported Symbols
 
 Explore a wide range of supported symbols, including gold, silver, platinum, palladium, and various others. From LBMA Gold to LME Steel, we cover it all. [View Symbols](https://www.metals-api.com/symbols)
 
 ## Available Endpoints
 
-The Metals-API API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+The Metals-API API comes with multiple endpoints, each providing different functionality. However, in this section, we will focus on the Latest Rates endpoint, Historical Rates and Times Series
 
 1. **Latest Rates Endpoint**
    - Returns real-time exchange rate data for all available or a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
 
+2. **Historical Rates Endpoint**
+   - Returns historical exchange rate data for a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
+
+3. **Time-Series Data Endpoint**
+   - Returns daily historical exchange rate data between two specified dates for all available or a specific set of currencies. (The date limits per API request depend on the acquired plan).
+
 ## Documentation
 
 For detailed information on API endpoints, usage, and integration guidelines, check our [API Documentation](https://www.metals-api.com/documentation).
 
 Start using Metals-API today for unparalleled access to precious metals data. Visit [Metals-API.com](https://metals-api.com) and integrate in just minutes!
```

### Comparing `metals_api-0.1/metals_api.egg-info/PKG-INFO` & `metals_api-0.2/metals_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metals-api
-Version: 0.1
+Version: 0.2
 Summary: A Python package to get the latest metals prices from the Metals-API
 Home-page: https://github.com/Zyla-Labs/pypi-metals-api
 Author: Zyla Labs
 Author-email: hello@zylalabs.com
 Keywords: metals-api,precious metals api,metals api,metals, precious metals,gold,silver,Platinum,Palladium,Ruthenium,Rhodium,forex data,rates,money,usd,eur,btc,forex api,gbp to usd,gbp to eur,eur to usd,api,currency api,exchange rate api,get currency rates api,currency rates php,usd to eur api,copper,nickel,aluminium,TIN,Zinc
 Description-Content-Type: text/markdown
 
@@ -27,19 +27,25 @@
 
 ## Supported Symbols
 
 Explore a wide range of supported symbols, including gold, silver, platinum, palladium, and various others. From LBMA Gold to LME Steel, we cover it all. [View Symbols](https://www.metals-api.com/symbols)
 
 ## Available Endpoints
 
-The Metals-API API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+The Metals-API API comes with multiple endpoints, each providing different functionality. However, in this section, we will focus on the Latest Rates endpoint, Historical Rates and Times Series
 
 1. **Latest Rates Endpoint**
    - Returns real-time exchange rate data for all available or a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
 
+2. **Historical Rates Endpoint**
+   - Returns historical exchange rate data for a specific set of currencies. (The number of symbols per API request depends on the acquired plan).
+
+3. **Time-Series Data Endpoint**
+   - Returns daily historical exchange rate data between two specified dates for all available or a specific set of currencies. (The date limits per API request depend on the acquired plan).
+
 ## Documentation
 
 For detailed information on API endpoints, usage, and integration guidelines, check our [API Documentation](https://www.metals-api.com/documentation).
 
 Start using Metals-API today for unparalleled access to precious metals data. Visit [Metals-API.com](https://metals-api.com) and integrate in just minutes!
```

### Comparing `metals_api-0.1/setup.py` & `metals_api-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name='metals_api',
-    version='0.1',
+    version='0.2',
     description = 'A Python package to get the latest metals prices from the Metals-API',
     author = 'Zyla Labs',
     author_email = 'hello@zylalabs.com',
     url = 'https://github.com/Zyla-Labs/pypi-metals-api',
     keywords = ['metals-api', 'precious metals api',  'metals api', 'metals, precious metals' , 'gold' , 'silver', 'Platinum', 'Palladium', 'Ruthenium', 'Rhodium', 'forex data', 'rates', 'money', 'usd', 'eur', 'btc', 'forex api', 'gbp to usd', 'gbp to eur', 'eur to usd', 'api', 'currency api', 'exchange rate api', 'get currency rates api', 'currency rates php', 'usd to eur api','copper','nickel','aluminium','TIN', 'Zinc'],
     packages=find_packages(),
     install_requires=[
```

