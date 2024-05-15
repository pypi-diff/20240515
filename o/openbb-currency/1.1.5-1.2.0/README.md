# Comparing `tmp/openbb_currency-1.1.5.tar.gz` & `tmp/openbb_currency-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_currency-1.1.5.tar", max compression
+gzip compressed data, was "openbb_currency-1.2.0.tar", max compression
```

## Comparing `openbb_currency-1.1.5.tar` & `openbb_currency-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      454 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/README.md
--rw-r--r--   0        0        0       32 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.497645 openbb_currency-1.1.5/openbb_currency/py.typed
--rw-r--r--   0        0        0      464 2024-04-19 16:40:14.511095 openbb_currency-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_currency-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-05-15 14:27:34.754626 openbb_currency-1.2.0/README.md
+-rw-r--r--   0        0        0       32 2024-02-29 11:03:36.730878 openbb_currency-1.2.0/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3605 2024-05-09 15:04:29.063333 openbb_currency-1.2.0/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.730995 openbb_currency-1.2.0/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 12:02:16.521653 openbb_currency-1.2.0/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.731082 openbb_currency-1.2.0/openbb_currency/py.typed
+-rw-r--r--   0        0        0      490 2024-05-15 16:04:55.540274 openbb_currency-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 openbb_currency-1.2.0/PKG-INFO
```

### Comparing `openbb_currency-1.1.5/openbb_currency/currency_router.py` & `openbb_currency-1.2.0/openbb_currency/currency_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,22 @@
 router.include_router(price_router)
 
 
 # pylint: disable=unused-argument
 @router.command(
     model="CurrencyPairs",
     examples=[
-        APIEx(parameters={"provider": "intrinio"}),
+        APIEx(parameters={"provider": "fmp"}),
         APIEx(
-            description="Search for 'EURUSD' currency pair using 'intrinio' as provider.",
-            parameters={"provider": "intrinio", "symbol": "EURUSD"},
-        ),
-        APIEx(
-            description="Search for actively traded currency pairs on the queried date using 'polygon' as provider.",
-            parameters={"provider": "polygon", "date": "2024-01-02", "active": True},
+            description="Search for 'EUR' currency pair using 'intrinio' as provider.",
+            parameters={"provider": "intrinio", "query": "EUR"},
         ),
         APIEx(
             description="Search for terms  using 'polygon' as provider.",
-            parameters={"provider": "polygon", "search": "Euro zone"},
+            parameters={"provider": "polygon", "query": "Euro zone"},
         ),
     ],
 )
 async def search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
```

### Comparing `openbb_currency-1.1.5/openbb_currency/price/price_router.py` & `openbb_currency-1.2.0/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_currency-1.1.5/PKG-INFO` & `openbb_currency-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-currency
-Version: 1.1.5
+Version: 1.2.0
 Summary: Currency extension for OpenBB
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
 
 # OpenBB Currency Extension
 
 This extension provides currency exchange related data for the OpenBB Platform.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-currency
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

