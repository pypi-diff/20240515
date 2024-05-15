# Comparing `tmp/openbb_tiingo-1.1.5.tar.gz` & `tmp/openbb_tiingo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tiingo-1.1.5.tar", max compression
+gzip compressed data, was "openbb_tiingo-1.2.0.tar", max compression
```

## Comparing `openbb_tiingo-1.1.5.tar` & `openbb_tiingo-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      440 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/README.md
--rw-r--r--   0        0        0     1120 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-17 12:33:20.769645 openbb_tiingo-1.1.5/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0      451 2024-04-19 16:41:54.227323 openbb_tiingo-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_tiingo-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      304 2024-05-15 14:29:35.406731 openbb_tiingo-1.2.0/README.md
+-rw-r--r--   0        0        0     1260 2024-05-14 15:30:05.619556 openbb_tiingo-1.2.0/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-29 11:03:36.971894 openbb_tiingo-1.2.0/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3657 2024-05-10 10:40:27.301343 openbb_tiingo-1.2.0/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5313 2024-05-10 10:40:27.301906 openbb_tiingo-1.2.0/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4680 2024-05-10 10:40:27.302091 openbb_tiingo-1.2.0/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5341 2024-05-10 10:40:27.302261 openbb_tiingo-1.2.0/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-04-02 11:35:59.532576 openbb_tiingo-1.2.0/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-04-08 12:02:16.680377 openbb_tiingo-1.2.0/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-02-29 11:03:36.972367 openbb_tiingo-1.2.0/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-02-29 11:03:36.972440 openbb_tiingo-1.2.0/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0      477 2024-05-15 16:06:54.282954 openbb_tiingo-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 openbb_tiingo-1.2.0/PKG-INFO
```

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/company_news.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     offset: Optional[int] = Field(
         default=0, description="Page offset, used in conjunction with limit."
     )
     source: Optional[str] = Field(
         default=None, description="A comma-separated list of the domains requested."
     )
```

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/crypto_historical.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
         "interval": "resampleFreq",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     exchanges: Optional[List[str]] = Field(
         default=None,
         description=(
@@ -121,15 +121,15 @@
         """Return the raw data from the Tiingo endpoint."""
         api_key = credentials.get("tiingo_token") if credentials else ""
 
         base_url = "https://api.tiingo.com/tiingo/crypto/prices"
         query_str = get_querystring(
             query.model_dump(by_alias=False), ["tickers", "resampleFreq"]
         )
-        results = []
+        results: List[dict] = []
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             result = await response.json()
             symbol = response.url.query.get("tickers", "")
             if not result:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
```

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/currency_historical.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/currency_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
         "interval": "resampleFreq",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     _frequency: Literal["daily", "weekly", "monthly", "annually"] = PrivateAttr(
         default=None
     )
@@ -102,15 +102,15 @@
 
         api_key = credentials.get("tiingo_token") if credentials else ""
 
         base_url = "https://api.tiingo.com/tiingo/fx/prices"
         query_str = get_querystring(
             query.model_dump(by_alias=False), ["tickers", "resampleFreq"]
         )
-        results = []
+        results: List[dict] = []
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             result = await response.json()
             symbol = response.url.query.get("tickers", "")
             if not result:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
```

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/equity_historical.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Source: https://www.tiingo.com/documentation/end-of-day
     """
 
     __alias_dict__ = {
         "start_date": "startDate",
         "end_date": "endDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1d", "1W", "1M", "1Y"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     _frequency: Literal["daily", "weekly", "monthly", "annually"] = PrivateAttr(
         default=None
     )
@@ -138,15 +138,15 @@
         query_str = get_querystring(
             query.model_dump(by_alias=True), ["symbol", "interval"]
         )
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             data = await response.json()
             symbol = response.url.parts[-2]
-            results = []
+            results: List[dict] = []
             if not data:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
 
             if isinstance(data, List):
                 results = data
```

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/models/world_news.py` & `openbb_tiingo-1.2.0/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.5/openbb_tiingo/utils/helpers.py` & `openbb_tiingo-1.2.0/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.5/PKG-INFO` & `openbb_tiingo-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-tiingo
-Version: 1.1.5
+Version: 1.2.0
 Summary: Tiingo extension for OpenBB
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
 
 # OpenBB Tiingo Provider
 
 This extension integrates the [Tiingo](https://www.tiingo.com/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-tiingo
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/feature/openbb-sdk-v4/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/sdk).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

