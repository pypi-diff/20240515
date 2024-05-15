# Comparing `tmp/openbb_cboe-1.1.5.tar.gz` & `tmp/openbb_cboe-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_cboe-1.1.5.tar", max compression
+gzip compressed data, was "openbb_cboe-1.2.0.tar", max compression
```

## Comparing `openbb_cboe-1.1.5.tar` & `openbb_cboe-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      423 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/README.md
--rw-r--r--   0        0        0     1779 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-04-19 13:10:31.744034 openbb_cboe-1.1.5/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-04-17 12:33:20.553645 openbb_cboe-1.1.5/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      494 2024-04-19 16:41:47.231306 openbb_cboe-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 openbb_cboe-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      296 2024-05-15 14:26:08.941817 openbb_cboe-1.2.0/README.md
+-rw-r--r--   0        0        0     1825 2024-05-14 15:30:05.610928 openbb_cboe-1.2.0/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.758231 openbb_cboe-1.2.0/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-08 12:02:16.581350 openbb_cboe-1.2.0/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8396 2024-05-10 10:40:27.290474 openbb_cboe-1.2.0/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9663 2024-05-10 10:40:27.290627 openbb_cboe-1.2.0/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-04-08 12:02:16.581679 openbb_cboe-1.2.0/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-04-23 10:22:39.655242 openbb_cboe-1.2.0/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-04-08 12:02:16.581852 openbb_cboe-1.2.0/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8420 2024-05-10 10:40:27.290789 openbb_cboe-1.2.0/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-04-08 12:02:16.582064 openbb_cboe-1.2.0/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4831 2024-05-09 13:34:29.201648 openbb_cboe-1.2.0/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     7796 2024-05-09 13:34:29.201967 openbb_cboe-1.2.0/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.759328 openbb_cboe-1.2.0/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-02-29 11:03:36.759398 openbb_cboe-1.2.0/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-04-23 10:22:39.655389 openbb_cboe-1.2.0/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      520 2024-05-15 16:06:48.877617 openbb_cboe-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_cboe-1.2.0/PKG-INFO
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/__init__.py` & `openbb_cboe-1.2.0/openbb_cboe/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from openbb_cboe.models.index_search import CboeIndexSearchFetcher
 from openbb_cboe.models.index_snapshots import CboeIndexSnapshotsFetcher
 from openbb_cboe.models.options_chains import CboeOptionsChainsFetcher
 from openbb_core.provider.abstract.provider import Provider
 
 cboe_provider = Provider(
     name="cboe",
-    website="https://www.cboe.com/",
+    website="https://www.cboe.com",
     description="""Cboe is the world's go-to derivatives and exchange network,
-    delivering cutting-edge trading, clearing and investment solutions to people
-    around the world.""",
+delivering cutting-edge trading, clearing and investment solutions to people
+around the world.""",
     credentials=None,
     fetcher_dict={
         "AvailableIndices": CboeAvailableIndicesFetcher,
         "EquityHistorical": CboeEquityHistoricalFetcher,
         "EquityQuote": CboeEquityQuoteFetcher,
         "EquitySearch": CboeEquitySearchFetcher,
         "EtfHistorical": CboeEquityHistoricalFetcher,
@@ -33,8 +33,9 @@
         "FuturesCurve": CboeFuturesCurveFetcher,
         "IndexHistorical": CboeIndexHistoricalFetcher,
         "IndexSearch": CboeIndexSearchFetcher,
         "IndexSnapshots": CboeIndexSnapshotsFetcher,
         "MarketIndices": CboeIndexHistoricalFetcher,
         "OptionsChains": CboeOptionsChainsFetcher,
     },
+    repr_name="Chicago Board Options Exchange (CBOE)",
 )
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/available_indices.py` & `openbb_cboe-1.2.0/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/equity_historical.py` & `openbb_cboe-1.2.0/openbb_cboe/models/equity_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class CboeEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """
     Cboe Equity Historical Price Query
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "1d"] = Field(
         default="1d",
         description=(
             QUERY_DESCRIPTIONS.get("interval", "")
             + " The most recent trading day is not including in daily historical data."
             + " Intraday data is only available for the most recent trading day at 1 minute intervals."
@@ -137,15 +137,15 @@
                 if symbol.replace("^", "") in TICKER_EXCEPTIONS
                 or symbol.replace("^", "") in INDEXES.index
                 else base_url + f"/{symbol.replace('^', '')}.json"
             )
             return url
 
         urls = [
-            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])
+            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])  # type: ignore[arg-type]
             for symbol in symbols
         ]
         return await amake_requests(urls, **kwargs)
 
     @staticmethod
     def transform_data(
         query: CboeEquityHistoricalQueryParams, data: List[Dict], **kwargs: Any
@@ -195,14 +195,14 @@
         if len(query.symbol.split(",")) == 1:
             output = output.drop(columns="symbol")
         # Finally, we apply the user-specified date range because it is not filtered at the source.
         output = output[
             (to_datetime(output["date"]) >= to_datetime(query.start_date))
             & (
                 to_datetime(output["date"])
-                <= to_datetime(query.end_date + timedelta(days=1))
+                <= to_datetime(query.end_date + timedelta(days=1))  # type: ignore[operator]
             )
         ]
         return [
             CboeEquityHistoricalData.model_validate(d)
             for d in output.to_dict("records")
         ]
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/equity_quote.py` & `openbb_cboe-1.2.0/openbb_cboe/models/equity_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class CboeEquityQuoteQueryParams(EquityQuoteQueryParams):
     """CBOE Equity Quote Query.
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="When True, the company directories will be cached for"
         + " 24 hours and are used to validate symbols."
         + " The results of the function are not cached. Set as False to bypass.",
     )
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/equity_search.py` & `openbb_cboe-1.2.0/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/futures_curve.py` & `openbb_cboe-1.2.0/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/index_constituents.py` & `openbb_cboe-1.2.0/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/index_historical.py` & `openbb_cboe-1.2.0/openbb_cboe/models/index_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class CboeIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """CBOE Market Indices Query.
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "1d"] = Field(
         default="1d",
         description=(
             QUERY_DESCRIPTIONS.get("interval", "")
             + " The most recent trading day is not including in daily historical data."
             + " Intraday data is only available for the most recent trading day at 1 minute intervals."
@@ -135,28 +135,28 @@
                 url = (
                     base_url + "index_history/"
                     if interval_type == "historical"
                     else base_url + "intraday_chart_data/"
                 )
                 url += f"{symbol.replace('^', '')}.json"
             else:
-                base_url: str = (
+                base_url: str = (  # type: ignore[no-redef]
                     f"https://cdn.cboe.com/api/global/delayed_quotes/charts/{interval_type}"
                 )
                 url = (
                     base_url + f"/_{symbol.replace('^', '')}.json"
                     if symbol.replace("^", "") in TICKER_EXCEPTIONS
                     or symbol.replace("^", "") in INDEXES.index
                     else base_url + f"/{symbol.replace('^', '')}.json"
                 )
 
             return url
 
         urls = [
-            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])
+            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])  # type: ignore[arg-type]
             for symbol in symbols
         ]
 
         return await amake_requests(urls, **kwargs)
 
     # pylint: disable=unused-argument
     @staticmethod
@@ -201,13 +201,13 @@
         if len(query.symbol.split(",")) == 1:
             output = output.drop(columns="symbol")
         # Finally, we apply the user-specified date range because it is not filtered at the source.
         output = output[
             (to_datetime(output["date"]) >= to_datetime(query.start_date))
             & (
                 to_datetime(output["date"])
-                <= to_datetime(query.end_date + timedelta(days=1))
+                <= to_datetime(query.end_date + timedelta(days=1))  # type: ignore[operator]
             )
         ]
         return [
             CboeIndexHistoricalData.model_validate(d) for d in output.to_dict("records")
         ]
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/index_search.py` & `openbb_cboe-1.2.0/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/index_snapshots.py` & `openbb_cboe-1.2.0/openbb_cboe/models/index_snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class CboeIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """CBOE Index Snapshots Query.
 
     Source: https://www.cboe.com/
     """
 
-    region: Literal[None, "us", "eu"] = Field(
+    region: Optional[Literal["us", "eu"]] = Field(
         default="us",
     )
 
     @field_validator("region", mode="after", check_fields=False)
     @classmethod
     def validate_region(cls, v: str):
         """Validate region."""
@@ -85,59 +85,61 @@
     def transform_query(params: Dict[str, Any]) -> CboeIndexSnapshotsQueryParams:
         """Transform the query."""
         return CboeIndexSnapshotsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeIndexSnapshotsQueryParams,
-        credentials: Optional[Dict[str, str]],
+        credentials: Optional[Dict[str, str]],  # pylint: disable=unused-argument
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Cboe endpoint"""
 
         if query.region == "us":
             url = "https://cdn.cboe.com/api/global/delayed_quotes/quotes/all_us_indices.json"
         if query.region == "eu":
             url = "https://cdn.cboe.com/api/global/european_indices/index_quotes/all-indices.json"
 
         data = await amake_request(url, **kwargs)
         return data.get("data")
 
     @staticmethod
     def transform_data(
-        query: CboeIndexSnapshotsQueryParams, data: dict, **kwargs: Any
+        query: CboeIndexSnapshotsQueryParams,  # pylint: disable=unused-argument
+        data: dict,
+        **kwargs: Any,  # pylint: disable=unused-argument
     ) -> List[CboeIndexSnapshotsData]:
         """Transform the data to the standard format"""
         if not data:
             raise EmptyDataError()
-        data = DataFrame(data)
+        df = DataFrame(data)
         percent_cols = [
             "price_change_percent",
             "iv30",
             "iv30_change",
             "iv30_change_percent",
         ]
         for col in percent_cols:
-            if col in data.columns:
-                data[col] = round(data[col] / 100, 6)
-        data = (
-            data.replace(0, None)
+            if col in df.columns:
+                df[col] = round(df[col] / 100, 6)
+        df = (
+            df.replace(0, None)
             .replace("", None)
             .dropna(how="all", axis=1)
             .fillna("N/A")
             .replace("N/A", None)
         )
         drop_cols = [
             "exchange_id",
             "seqno",
             "index",
             "security_type",
             "ask_size",
             "bid_size",
         ]
         for col in drop_cols:
-            if col in data.columns:
-                data = data.drop(columns=col)
+            if col in df.columns:
+                df = df.drop(columns=col)
         return [
             CboeIndexSnapshotsData.model_validate(d)
-            for d in data.to_dict(orient="records")
+            for d in df.to_dict(orient="records")
         ]
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/models/options_chains.py` & `openbb_cboe-1.2.0/openbb_cboe/models/options_chains.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, Optional
 
 from openbb_cboe.utils.helpers import (
     TICKER_EXCEPTIONS,
     get_company_directory,
     get_index_directory,
 )
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.options_chains import (
     OptionsChainsData,
     OptionsChainsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
@@ -58,45 +59,80 @@
         return CboeOptionsChainsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeOptionsChainsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
-    ) -> List[Dict]:
-        """Return the raw data from the Cboe endpoint"""
-
-        symbol = query.symbol.replace("^", "").split(",")[0]
+    ) -> Dict:
+        """Return the raw data from the Cboe endpoint."""
+        symbol = query.symbol.replace("^", "").split(",")[0].upper()
         INDEXES = await get_index_directory(use_cache=query.use_cache)
         SYMBOLS = await get_company_directory(use_cache=query.use_cache)
         INDEXES = INDEXES.set_index("index_symbol")
 
         if symbol not in SYMBOLS.index:
             raise RuntimeError(f"{symbol} was not found in the Cboe options directory.")
 
         quotes_url = (
             f"https://cdn.cboe.com/api/global/delayed_quotes/options/_{symbol}.json"
             if symbol in TICKER_EXCEPTIONS or symbol in INDEXES.index
             else f"https://cdn.cboe.com/api/global/delayed_quotes/options/{symbol}.json"
         )
-
-        return await amake_request(quotes_url)
+        results = await amake_request(quotes_url)
+        return results  # type: ignore
 
     @staticmethod
     def transform_data(
         query: CboeOptionsChainsQueryParams,
-        data: List[Dict],
+        data: Dict,
         **kwargs: Any,
-    ) -> List[CboeOptionsChainsData]:
-        """Transform the data to the standard format"""
-
+    ) -> AnnotatedResult[List[CboeOptionsChainsData]]:
+        """Transform the data to the standard format."""
         if not data:
             raise EmptyDataError()
+        results_metadata = {}
+        options = data.get("data", {}).pop("options", [])
+        change_percent = data["data"].get("percent_change", None)
+        iv30_percent = data["data"].get("iv30_change_percent", None)
+        if change_percent:
+            change_percent = change_percent / 100
+        if iv30_percent:
+            iv30_percent = iv30_percent / 100
+        last_timestamp = data["data"].get("last_trade_time", None)
+        if last_timestamp:
+            last_timestamp = to_datetime(
+                last_timestamp, format="%Y-%m-%dT%H:%M:%S"
+            ).strftime("%Y-%m-%d %H:%M:%S")
+        results_metadata.update(
+            {
+                "symbol": data["data"].get("symbol"),
+                "security_type": data["data"].get("security_type", None),
+                "bid": data["data"].get("bid", None),
+                "bid_size": data["data"].get("bid_size", None),
+                "ask": data["data"].get("ask", None),
+                "ask_size": data["data"].get("ask_size", None),
+                "open": data["data"].get("open", None),
+                "high": data["data"].get("high", None),
+                "low": data["data"].get("low", None),
+                "close": data["data"].get("close", None),
+                "volume": data["data"].get("volume", None),
+                "current_price": data["data"].get("current_price", None),
+                "prev_close": data["data"].get("prev_day_close", None),
+                "change": data["data"].get("price_change", None),
+                "change_percent": change_percent,
+                "iv30": data["data"].get("iv30", None),
+                "iv30_change": data["data"].get("iv30_change", None),
+                "iv30_change_percent": iv30_percent,
+                "last_tick": data["data"].get("tick", None),
+                "last_trade_timestamp": last_timestamp,
+            }
+        )
 
-        options_df = DataFrame.from_records(data["data"]["options"])
+        options_df = DataFrame.from_records(options)
 
         options_df = options_df.rename(
             columns={
                 "option": "contract_symbol",
                 "iv": "implied_volatility",
                 "theo": "theoretical_price",
                 "percent_change": "change_percent",
@@ -148,11 +184,14 @@
         quotes["open_interest"] = quotes["open_interest"].astype("int64")
         quotes["volume"] = quotes["volume"].astype("int64")
         quotes["bid_size"] = quotes["bid_size"].astype("int64")
         quotes["ask_size"] = quotes["ask_size"].astype("int64")
         quotes["prev_close"] = round(quotes["prev_close"], 2)
         quotes["change_percent"] = round(quotes["change_percent"] / 100, 4)
 
-        return [
-            CboeOptionsChainsData.model_validate(d)
-            for d in quotes.reset_index().to_dict("records")
-        ]
+        return AnnotatedResult(
+            result=[
+                CboeOptionsChainsData.model_validate(d)
+                for d in quotes.reset_index().to_dict("records")
+            ],
+            metadata=results_metadata,
+        )
```

### Comparing `openbb_cboe-1.1.5/openbb_cboe/utils/helpers.py` & `openbb_cboe-1.2.0/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

