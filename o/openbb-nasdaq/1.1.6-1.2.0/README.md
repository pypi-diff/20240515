# Comparing `tmp/openbb_nasdaq-1.1.6.tar.gz` & `tmp/openbb_nasdaq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nasdaq-1.1.6.tar", max compression
+gzip compressed data, was "openbb_nasdaq-1.2.0.tar", max compression
```

## Comparing `openbb_nasdaq-1.1.6.tar` & `openbb_nasdaq-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      430 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/README.md
--rw-r--r--   0        0        0     1840 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-04-19 15:17:18.352283 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5109 2024-04-19 15:17:18.352283 openbb_nasdaq-1.1.6/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-19 13:10:31.748034 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-17 12:33:20.681645 openbb_nasdaq-1.1.6/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      508 2024-04-19 16:40:57.859190 openbb_nasdaq-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 openbb_nasdaq-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      303 2024-05-15 14:25:19.879856 openbb_nasdaq-1.2.0/README.md
+-rw-r--r--   0        0        0     2484 2024-05-14 15:30:05.617274 openbb_nasdaq-1.2.0/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-23 10:22:39.674899 openbb_nasdaq-1.2.0/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-04-23 10:22:39.675013 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-04-23 10:22:39.675292 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-04-02 11:35:59.494640 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-04-23 10:22:39.675428 openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-04-23 10:22:39.675550 openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5111 2024-05-10 10:40:27.299762 openbb_nasdaq-1.2.0/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-04-08 12:02:16.661594 openbb_nasdaq-1.2.0/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5163 2024-05-10 10:40:27.300096 openbb_nasdaq-1.2.0/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-04-08 12:02:16.661718 openbb_nasdaq-1.2.0/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-04-08 12:02:16.661815 openbb_nasdaq-1.2.0/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-04-08 12:02:16.661906 openbb_nasdaq-1.2.0/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-04-02 11:35:59.495686 openbb_nasdaq-1.2.0/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-04-23 10:22:39.675762 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-02-29 11:03:36.881453 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-04-08 12:02:16.661991 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-04-08 12:02:16.662176 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      534 2024-05-15 16:05:35.015231 openbb_nasdaq-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 openbb_nasdaq-1.2.0/PKG-INFO
```

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/cot_search.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/economic_calendar.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/economic_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class NasdaqEconomicCalendarQueryParams(EconomicCalendarQueryParams):
     """Nasdaq Economic Calendar Query.
 
     Source: https://www.nasdaq.com/market-activity/economic-calendar
     """
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
     country: Optional[str] = Field(
         default=None,
         description="Country of the event",
     )
 
     @field_validator("country", mode="before", check_fields=False)
```

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/equity_search.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/historical_dividends.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/historical_dividends.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from openbb_nasdaq.utils.helpers import IPO_HEADERS
 from pydantic import Field, field_validator
 
 
 class NasdaqHistoricalDividendsQueryParams(HistoricalDividendsQueryParams):
     """Nasdaq Historical Dividends Query Params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class NasdaqHistoricalDividendsData(HistoricalDividendsData):
     """Nasdaq Historical Dividends Data."""
 
     __alias_dict__ = {
         "ex_dividend_date": "exOrEffDate",
@@ -113,21 +113,21 @@
             asset_class = "stocks"
             url = f"https://api.nasdaq.com/api/quote/{symbol}/dividends?assetclass={asset_class}"
 
             response = await amake_request(
                 url,
                 headers=IPO_HEADERS,
             )
-            if response.get("status").get("rCode") == 400:
+            if response.get("status").get("rCode") == 400:  # type: ignore
                 response = await amake_request(
                     url.replace("stocks", "etf"),
                     headers=IPO_HEADERS,
                 )
-            if response.get("status").get("rCode") == 200:
-                data = response.get("data").get("dividends").get("rows")
+            if response.get("status").get("rCode") == 200:  # type: ignore
+                data = response.get("data").get("dividends").get("rows")  # type: ignore
 
             if data:
                 if len(symbols) > 1:
                     for d in data:
                         d["symbol"] = symbol
                 results.extend(data)
             if not data:
```

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/models/top_retail.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/helpers.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/query_params.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/openbb_nasdaq/utils/series_ids.py` & `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.6/PKG-INFO` & `openbb_nasdaq-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-nasdaq
-Version: 1.1.6
+Version: 1.2.0
 Summary: Nasdaq extension for OpenBB
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
 Requires-Dist: nasdaq-data-link (>=1.0.4,<2.0.0)
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Nasdaq Provider
 
 This extension integrates the [Nasdaq](https://www.nasdaq.com) data provider into the OpenBB Platform.
 
@@ -24,11 +26,9 @@
 
 To install the extension:
 
 ```bash
 pip install openbb-nasdaq
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

