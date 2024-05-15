# Comparing `tmp/openbb_alpha_vantage-1.1.5.tar.gz` & `tmp/openbb_alpha_vantage-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_alpha_vantage-1.1.5.tar", max compression
+gzip compressed data, was "openbb_alpha_vantage-1.2.0.tar", max compression
```

## Comparing `openbb_alpha_vantage-1.1.5.tar` & `openbb_alpha_vantage-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      457 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/README.md
--rw-r--r--   0        0        0     1106 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-17 12:33:20.553645 openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      493 2024-04-19 16:41:41.591292 openbb_alpha_vantage-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      330 2024-05-15 14:26:22.821035 openbb_alpha_vantage-1.2.0/README.md
+-rw-r--r--   0        0        0     1452 2024-05-10 19:27:56.005744 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-23 10:22:39.651445 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-10 10:40:27.289046 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5594 2024-05-14 15:30:05.609782 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752779 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-04-23 10:22:39.651694 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-23 10:22:39.651812 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      519 2024-05-15 16:06:25.928312 openbb_alpha_vantage-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.2.0/PKG-INFO
```

### Comparing `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/equity_historical.py` & `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class AVEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Alpha Vantage Equity Historical Price Query.
 
     Source: https://www.alphavantage.co/documentation/#time-series-data
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "60m", "1d", "1W", "1M"] = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", ""),
     )
     adjustment: Literal["splits_only", "splits_and_dividends", "unadjusted"] = Field(
         description="The adjustment factor to apply. 'splits_only' is not supported for intraday data.",
```

### Comparing `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/models/historical_eps.py` & `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/historical_eps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """AlphaVantage Historical EPS Model."""
 
 # pylint: disable=unused-argument
 
-import warnings
 from datetime import date as dateType
 from typing import Any, Dict, List, Literal, Optional, Union
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.historical_eps import (
     HistoricalEpsData,
     HistoricalEpsQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
@@ -16,25 +16,23 @@
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
     amake_requests,
 )
 from pydantic import Field, field_validator
 
-_warn = warnings.warn
-
 
 class AlphaVantageHistoricalEpsQueryParams(HistoricalEpsQueryParams):
     """
     AlphaVantage Historical EPS Query Params.
 
     Source: https://www.alphavantage.co/documentation/#earnings
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     period: Literal["annual", "quarter"] = Field(
         default="quarter", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     limit: Optional[int] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
@@ -99,55 +97,57 @@
     @staticmethod
     async def aextract_data(
         query: AlphaVantageHistoricalEpsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the AlphaVantage endpoint."""
-
         api_key = credentials.get("alpha_vantage_api_key") if credentials else ""
-
         BASE_URL = "https://www.alphavantage.co/query?function=EARNINGS&"
-
         # We are allowing multiple symbols to be passed in the query, so we need to handle that.
         symbols = query.symbol.split(",")
-
         urls = [f"{BASE_URL}symbol={symbol}&apikey={api_key}" for symbol in symbols]
-
-        results = []
+        results: List = []
+        messages: List = []
 
         # We need to make a custom callback function for this async request.
         async def response_callback(response: ClientResponse, _: ClientSession):
             """Response callback function."""
             symbol = response.url.query.get("symbol", None)
             data = await response.json()
             target = (
                 "annualEarnings" if query.period == "annual" else "quarterlyEarnings"
             )
-            result = []
+            message = data.get("Information", "")
+            if message:
+                messages.append(message)
+                warn(f"Symbol Error for {symbol}: {message}")
+            result: List = []
             # If data is returned, append it to the results list.
             if data:
                 result = [
                     {
                         "symbol": symbol,
                         **d,
                     }
                     for d in data.get(target, [])  # type: ignore
                 ]
                 if query.limit is not None:
                     results.extend(result[: query.limit])
                 else:
                     results.extend(result)
-
             # If no data is returned, raise a warning and move on to the next symbol.
             if not data:
-                _warn(f"Symbol Error: No data found for {symbol}")
+                warn(f"Symbol Error: No data found for {symbol}")
 
         await amake_requests(urls, response_callback, **kwargs)  # type: ignore
 
+        if not results:
+            raise EmptyDataError(f"No data was returned -> \n{messages[-1]}")
+
         return results
 
     @staticmethod
     def transform_data(
         query: AlphaVantageHistoricalEpsQueryParams,
         data: List[Dict],
         **kwargs: Any,
```

### Comparing `openbb_alpha_vantage-1.1.5/openbb_alpha_vantage/utils/helpers.py` & `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

