# Comparing `tmp/openbb_finviz-1.0.4.tar.gz` & `tmp/openbb_finviz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finviz-1.0.4.tar", max compression
+gzip compressed data, was "openbb_finviz-1.1.0.tar", max compression
```

## Comparing `openbb_finviz-1.0.4.tar` & `openbb_finviz-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      442 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/README.md
--rw-r--r--   0        0        0     1005 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.649645 openbb_finviz-1.0.4/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0      477 2024-04-19 16:41:30.451265 openbb_finviz-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 openbb_finviz-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      315 2024-05-15 14:25:46.006898 openbb_finviz-1.1.0/README.md
+-rw-r--r--   0        0        0     1029 2024-05-14 15:30:05.612881 openbb_finviz-1.1.0/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.665328 openbb_finviz-1.1.0/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9621 2024-05-09 15:04:29.070455 openbb_finviz-1.1.0/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8254 2024-05-10 10:40:27.291294 openbb_finviz-1.1.0/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    11039 2024-05-10 10:40:27.291399 openbb_finviz-1.1.0/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4395 2024-05-15 11:17:30.040928 openbb_finviz-1.1.0/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3932 2024-05-10 10:40:27.291736 openbb_finviz-1.1.0/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630717 openbb_finviz-1.1.0/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630748 openbb_finviz-1.1.0/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-04-23 10:22:39.665571 openbb_finviz-1.1.0/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-08 12:02:16.630850 openbb_finviz-1.1.0/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630874 openbb_finviz-1.1.0/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0      503 2024-05-15 16:05:18.824210 openbb_finviz-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 openbb_finviz-1.1.0/PKG-INFO
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/__init__.py` & `openbb_finviz-1.1.0/openbb_finviz/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,9 @@
         "CompareGroups": FinvizCompareGroupsFetcher,
         "EtfPricePerformance": FinvizPricePerformanceFetcher,
         "EquityInfo": FinvizEquityProfileFetcher,
         "KeyMetrics": FinvizKeyMetricsFetcher,
         "PricePerformance": FinvizPricePerformanceFetcher,
         "PriceTarget": FinvizPriceTargetFetcher,
     },
+    repr_name="FinViz",
 )
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/models/compare_groups.py` & `openbb_finviz-1.1.0/openbb_finviz/models/compare_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,50 +75,50 @@
     market_cap: Optional[ForceInt] = Field(
         default=None,
         description="The market cap of the group.",
     )
     performance_1D: Optional[float] = Field(
         default=None,
         description="The performance in the last day, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_1W: Optional[float] = Field(
         default=None,
         description="The performance in the last week, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_1M: Optional[float] = Field(
         default=None,
         description="The performance in the last month, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_3M: Optional[float] = Field(
         default=None,
         description="The performance in the last quarter, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_6M: Optional[float] = Field(
         default=None,
         description="The performance in the last half year, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_1Y: Optional[float] = Field(
         default=None,
         description="The performance in the last year, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     performance_YTD: Optional[float] = Field(
         default=None,
         description="The performance in the year to date, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     dividend_yield: Optional[float] = Field(
         default=None,
         description="The dividend yield of the group, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     pe: Optional[float] = Field(
         default=None,
         description="The P/E ratio of the group.",
     )
     forward_pe: Optional[float] = Field(
         default=None,
@@ -128,31 +128,31 @@
         default=None,
         description="The PEG ratio of the group.",
         alias="pe_growth",
     )
     eps_growth_past_5_years: Optional[float] = Field(
         default=None,
         description="The EPS growth of the group for the past 5 years, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     eps_growth_next_5_years: Optional[float] = Field(
         default=None,
         description="The estimated EPS growth of the groupo for the next 5 years,"
         + " as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     sales_growth_past_5_years: Optional[float] = Field(
         default=None,
         description="The sales growth of the group for the past 5 years, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     float_short: Optional[float] = Field(
         default=None,
         description="The percent of the float shorted for the group, as a normalized value.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     analyst_recommendation: Optional[float] = Field(
         default=None,
         description="The analyst consensus, on a scale of 1-5 where 1 is a buy and 5 is a sell.",
     )
     volume: Optional[ForceInt] = Field(
         default=None, description=DATA_DESCRIPTIONS.get("volume", "")
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/models/equity_profile.py` & `openbb_finviz-1.1.0/openbb_finviz/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Finviz Equity Profile Model."""
 
 # pylint: disable=unused-argument
-import warnings
+
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from finvizfinance.quote import finvizfinance
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_info import (
     EquityInfoData,
     EquityInfoQueryParams,
 )
 from pydantic import Field
 
-_warn = warnings.warn
-
 
 class FinvizEquityProfileQueryParams(EquityInfoQueryParams):
     """
     Finviz Equity Profile Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizEquityProfileData(EquityInfoData):
     """Finviz Equity Profile Data."""
 
     __alias_dict__ = {
         "stock_exchange": "exchange",
@@ -55,24 +54,24 @@
     short_interest: Optional[str] = Field(
         default=None,
         description="The last reported number of shares sold short, as an abbreviated string.",
     )
     institutional_ownership: Optional[float] = Field(
         default=None,
         description="The institutional ownership of the stock, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     market_cap: Optional[str] = Field(
         default=None,
         description="The market capitalization of the stock, as an abbreviated string.",
     )
     dividend_yield: Optional[float] = Field(
         default=None,
         description="The dividend yield of the stock, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     earnings_date: Optional[str] = Field(
         default=None,
         description="The last, or next confirmed, earnings date and announcement time, as a string."
         + " The format is Nov 02 AMC - for after market close.",
     )
     beta: Optional[float] = Field(
@@ -95,25 +94,25 @@
     def extract_data(
         query: FinvizEquityProfileQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data from Finviz."""
 
-        results = []
+        results: List = []
 
         def get_one(symbol) -> Dict:
             """Get the data for one symbol."""
-            result = {}
+            result: Dict = {}
             try:
                 data = finvizfinance(symbol)
                 fundament = data.ticker_fundament()
                 description = data.ticker_description()
             except Exception as e:  # pylint: disable=W0718
-                _warn(f"Failed to get data for {symbol} -> {e}")
+                warn(f"Failed to get data for {symbol} -> {e}")
                 return result
             div_yield = (
                 float(str(fundament.get("Dividend %", None)).replace("%", "")) / 100
                 if fundament.get("Dividend %", "-") != "-"
                 else None
             )
             inst_own = (
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/models/key_metrics.py` & `openbb_finviz-1.1.0/openbb_finviz/models/key_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class FinvizKeyMetricsQueryParams(KeyMetricsQueryParams):
     """
     Finviz Key Metrics Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizKeyMetricsData(KeyMetricsData):
     """Finviz Key Metrics Data."""
 
     foward_pe: Optional[float] = Field(
         default=None, description="Forward price-to-earnings ratio (forward P/E)"
@@ -57,50 +57,50 @@
         default=None, description="Long-term debt-to-equity ratio (LT Debt/Eq)"
     )
     quick_ratio: Optional[float] = Field(default=None, description="Quick ratio")
     current_ratio: Optional[float] = Field(default=None, description="Current ratio")
     gross_margin: Optional[float] = Field(
         default=None,
         description="Gross margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     profit_margin: Optional[float] = Field(
         default=None,
         description="Profit margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     operating_margin: Optional[float] = Field(
         default=None,
         description="Operating margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_on_assets: Optional[float] = Field(
         default=None,
         description="Return on assets (ROA), as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_on_investment: Optional[float] = Field(
         default=None,
         description="Return on investment (ROI), as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_on_equity: Optional[float] = Field(
         default=None,
         description="Return on equity (ROE), as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     payout_ratio: Optional[float] = Field(
         default=None,
         description="Payout ratio, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     dividend_yield: Optional[float] = Field(
         default=None,
         description="Dividend yield, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
 
 
 class FinvizKeyMetricsFetcher(
     Fetcher[FinvizKeyMetricsQueryParams, List[FinvizKeyMetricsData]]
 ):
     """Finviz Key Metrics Fetcher."""
@@ -114,19 +114,19 @@
     def extract_data(
         query: FinvizKeyMetricsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data from Finviz."""
 
-        results = []
+        results: List = []
 
         def get_one(symbol) -> Dict:
             """Get the data for one symbol."""
-            result = {}
+            result: Dict = {}
             try:
                 data = finvizfinance(symbol)
                 fundament = data.ticker_fundament()
                 mkt_cap = (
                     fundament.get("Market Cap", None)
                     if fundament.get("Market Cap", "-") != "-"
                     else None
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/models/price_performance.py` & `openbb_finviz-1.1.0/openbb_finviz/models/price_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class FinvizPricePerformanceQueryParams(RecentPerformanceQueryParams):
     """
     Finviz Price Performance Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizPricePerformanceData(RecentPerformanceData):
     """Finviz Price Performance Data."""
 
     __alias_dict__ = {
         "symbol": "Ticker",
@@ -44,20 +44,20 @@
         "relative_volume": "Rel Volume",
         "analyst_score": "Recom",
     }
 
     volatility_week: Optional[float] = Field(
         default=None,
         description="One-week realized volatility, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "fontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     volatility_month: Optional[float] = Field(
         default=None,
         description="One-month realized volatility, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "fontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     price: Optional[float] = Field(
         default=None,
         description="Last Price.",
     )
     volume: Optional[float] = Field(
         default=None,
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/models/price_target.py` & `openbb_finviz-1.1.0/openbb_finviz/models/price_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class FinvizPriceTargetQueryParams(PriceTargetQueryParams):
     """Finviz Price Target Query.
 
     Source: https://finviz.com/quote.ashx?
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizPriceTargetData(PriceTargetData):
     """Finviz Price Target Data."""
 
     __alias_dict__ = {
         "published_date": "Date",
@@ -63,20 +63,20 @@
     def extract_data(
         query: FinvizPriceTargetQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Finviz endpoint."""
 
-        results = []
+        results: List[dict] = []
 
         def get_one(symbol) -> List[Dict]:
             """Get the data for one symbol."""
             price_targets = DataFrame()
-            result = []
+            result: List[dict] = []
             try:
                 data = finvizfinance(symbol)
                 price_targets = data.ticker_outer_ratings()
                 if price_targets is None or len(price_targets) == 0:
                     _warn(f"Failed to get data for {symbol}")
                     return result
                 price_targets["symbol"] = symbol
@@ -96,15 +96,15 @@
                 price_targets = price_targets.replace("", None).drop(columns="Price")
             except Exception as e:  # pylint: disable=W0718
                 _warn(f"Failed to get data for {symbol} -> {e}")
                 return result
             result = price_targets.to_dict(orient="records")
             return result
 
-        symbols = query.symbol.split(",")
+        symbols = query.symbol.split(",") if query.symbol else []
         for symbol in symbols:
             result = get_one(symbol)
             if result is not None and result != []:
                 results.extend(result)
 
         return results
```

### Comparing `openbb_finviz-1.0.4/openbb_finviz/utils/definitions.py` & `openbb_finviz-1.1.0/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.4/PKG-INFO` & `openbb_finviz-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: openbb-finviz
-Version: 1.0.4
+Version: 1.1.0
 Summary: Finviz extension for OpenBB
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
 Requires-Dist: finvizfinance (==0.14.7)
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Finviz Data Provider Extension
 
 This extension integrates the [Finviz](https://finviz.com/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-finviz
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

