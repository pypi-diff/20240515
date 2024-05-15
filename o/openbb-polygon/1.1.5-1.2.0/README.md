# Comparing `tmp/openbb_polygon-1.1.5.tar.gz` & `tmp/openbb_polygon-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_polygon-1.1.5.tar", max compression
+gzip compressed data, was "openbb_polygon-1.2.0.tar", max compression
```

## Comparing `openbb_polygon-1.1.5.tar` & `openbb_polygon-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      430 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/README.md
--rw-r--r--   0        0        0     2100 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6283 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6255 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     7150 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-19 13:10:31.748034 openbb_polygon-1.1.5/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6142 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-04-19 16:31:25.550563 openbb_polygon-1.1.5/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-17 12:33:20.689645 openbb_polygon-1.1.5/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0      457 2024-04-19 16:43:11.675521 openbb_polygon-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 openbb_polygon-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      303 2024-05-15 14:25:08.997475 openbb_polygon-1.2.0/README.md
+-rw-r--r--   0        0        0     2871 2024-05-14 15:30:05.617960 openbb_polygon-1.2.0/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-23 10:22:39.678191 openbb_polygon-1.2.0/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-04-02 11:35:59.508406 openbb_polygon-1.2.0/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     7039 2024-05-09 13:34:29.229455 openbb_polygon-1.2.0/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4606 2024-05-10 10:40:27.300299 openbb_polygon-1.2.0/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6289 2024-05-10 10:40:27.300493 openbb_polygon-1.2.0/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6261 2024-05-10 10:40:27.300668 openbb_polygon-1.2.0/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     5135 2024-05-09 15:04:29.071926 openbb_polygon-1.2.0/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9871 2024-05-10 10:40:27.300830 openbb_polygon-1.2.0/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7156 2024-05-10 10:40:27.301011 openbb_polygon-1.2.0/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-04-08 12:02:16.668848 openbb_polygon-1.2.0/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-04-08 12:02:16.668984 openbb_polygon-1.2.0/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6148 2024-05-10 10:40:27.301163 openbb_polygon-1.2.0/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-04-23 10:22:39.678939 openbb_polygon-1.2.0/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-04-08 12:02:16.669327 openbb_polygon-1.2.0/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887235 openbb_polygon-1.2.0/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-04-23 10:22:39.679023 openbb_polygon-1.2.0/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-04-23 10:22:39.679139 openbb_polygon-1.2.0/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0      483 2024-05-15 16:06:03.353141 openbb_polygon-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 openbb_polygon-1.2.0/PKG-INFO
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/__init__.py` & `openbb_polygon-1.2.0/openbb_polygon/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,43 @@
 from openbb_core.provider.abstract.provider import Provider
 from openbb_polygon.models.balance_sheet import PolygonBalanceSheetFetcher
 from openbb_polygon.models.cash_flow import PolygonCashFlowStatementFetcher
 from openbb_polygon.models.company_news import PolygonCompanyNewsFetcher
 from openbb_polygon.models.crypto_historical import PolygonCryptoHistoricalFetcher
 from openbb_polygon.models.currency_historical import PolygonCurrencyHistoricalFetcher
 from openbb_polygon.models.currency_pairs import PolygonCurrencyPairsFetcher
+from openbb_polygon.models.currency_snapshots import PolygonCurrencySnapshotsFetcher
 from openbb_polygon.models.equity_historical import PolygonEquityHistoricalFetcher
 from openbb_polygon.models.equity_nbbo import PolygonEquityNBBOFetcher
 from openbb_polygon.models.income_statement import PolygonIncomeStatementFetcher
 from openbb_polygon.models.index_historical import (
     PolygonIndexHistoricalFetcher,
 )
 from openbb_polygon.models.market_snapshots import PolygonMarketSnapshotsFetcher
 
 polygon_provider = Provider(
     name="polygon",
-    website="https://polygon.io/",
+    website="https://polygon.io",
     description="""The Polygon.io Stocks API provides REST endpoints that let you query
-     the latest market data from all US stock exchanges. You can also find data on
-     company financials, stock market holidays, corporate actions, and more.""",
+the latest market data from all US stock exchanges. You can also find data on
+company financials, stock market holidays, corporate actions, and more.""",
     credentials=["api_key"],
     fetcher_dict={
         "BalanceSheet": PolygonBalanceSheetFetcher,
         "CashFlowStatement": PolygonCashFlowStatementFetcher,
         "CompanyNews": PolygonCompanyNewsFetcher,
         "CryptoHistorical": PolygonCryptoHistoricalFetcher,
         "CurrencyHistorical": PolygonCurrencyHistoricalFetcher,
         "CurrencyPairs": PolygonCurrencyPairsFetcher,
+        "CurrencySnapshots": PolygonCurrencySnapshotsFetcher,
         "EquityHistorical": PolygonEquityHistoricalFetcher,
         "EquityNBBO": PolygonEquityNBBOFetcher,
         "EtfHistorical": PolygonEquityHistoricalFetcher,
         "IncomeStatement": PolygonIncomeStatementFetcher,
         "IndexHistorical": PolygonIndexHistoricalFetcher,
         "MarketIndices": PolygonIndexHistoricalFetcher,
         "MarketSnapshots": PolygonMarketSnapshotsFetcher,
     },
+    repr_name="Polygon.io",
+    v3_credentials=["API_POLYGON_KEY"],
+    instructions='Go to: https://polygon.io\n\n![Polygon](https://user-images.githubusercontent.com/46355364/207825623-fcd7f0a3-131a-4294-808c-754c13e38e2a.png)\n\nClick on, "Get your Free API Key".\n\n![Polygon](https://user-images.githubusercontent.com/46355364/207825952-ca5540ec-6ed2-4cef-a0ed-bb50b813932c.png)\n\nAfter signing up, the API Key is found at the bottom of the account dashboard page.\n\n![Polygon](https://user-images.githubusercontent.com/46355364/207826258-b1f318fa-fd9c-41d9-bf5c-fe16722e6601.png)',  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/balance_sheet.py` & `openbb_polygon-1.2.0/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/cash_flow.py` & `openbb_polygon-1.2.0/openbb_polygon/models/cash_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,18 +60,18 @@
         default=None,
         description="Period of report date greater than or equal to the given date.",
     )
     include_sources: bool = Field(
         default=False,
         description="Whether to include the sources of the financial statement.",
     )
-    order: Literal[None, "asc", "desc"] = Field(
+    order: Optional[Literal["asc", "desc"]] = Field(
         default=None, description="Order of the financial statement."
     )
-    sort: Literal[None, "filing_date", "period_of_report_date"] = Field(
+    sort: Optional[Literal["filing_date", "period_of_report_date"]] = Field(
         default=None, description="Sort of the financial statement."
     )
 
 
 class PolygonCashFlowStatementData(CashFlowStatementData):
     """Polygon Cash Flow Statement Data."""
 
@@ -156,17 +156,17 @@
 
         request_url = f"{base_url}?{query_string}&apiKey={api_key}"
 
         return await get_data_many(request_url, "results", **kwargs)
 
     @staticmethod
     def transform_data(
-        query: PolygonCashFlowStatementQueryParams,
+        query: PolygonCashFlowStatementQueryParams,  # pylint: disable=unused-argument
         data: dict,
-        **kwargs: Any,
+        **kwargs: Any,  # pylint: disable=unused-argument
     ) -> List[PolygonCashFlowStatementData]:
         """Return the transformed data."""
         transformed_data = []
 
         for item in data:
             sub_data = {
                 key: value["value"]
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/company_news.py` & `openbb_polygon-1.2.0/openbb_polygon/models/company_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class PolygonCompanyNewsQueryParams(CompanyNewsQueryParams):
     """Polygon Company News Query.
 
     Source: https://polygon.io/docs/stocks/get_v2_reference_news
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
     __alias_dict__ = {
         "symbol": "ticker",
         "start_date": "published_utc.gte",
         "end_date": "published_utc.lte",
     }
 
     order: Optional[Literal["asc", "desc"]] = Field(
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/crypto_historical.py` & `openbb_polygon-1.2.0/openbb_polygon/models/crypto_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class PolygonCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Polygon Crypto Historical Price Query.
 
     Source: https://polygon.io/docs/crypto/get_v2_aggs_ticker__cryptoticker__range__multiplier___timespan___from___to
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/currency_historical.py` & `openbb_polygon-1.2.0/openbb_polygon/models/currency_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class PolygonCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Polygon Currency Historical Price Query.
 
     Source: https://polygon.io/docs/forex/get_v2_aggs_ticker__forexticker__range__multiplier___timespan___from___to
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/currency_pairs.py` & `openbb_polygon-1.2.0/openbb_polygon/models/currency_pairs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,138 @@
 """Polygon Currency Available Pairs Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_pairs import (
     CurrencyPairsData,
     CurrencyPairsQueryParams,
 )
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_polygon.utils.helpers import get_data
-from pydantic import Field, PositiveInt, field_validator
+from pandas import DataFrame
+from pydantic import Field, field_validator
 
 
 class PolygonCurrencyPairsQueryParams(CurrencyPairsQueryParams):
     """Polygon Currency Available Pairs Query.
 
     Source: https://polygon.io/docs/forex/get_v3_reference_tickers
     """
 
-    symbol: Optional[str] = Field(
-        default=None, description="Symbol of the pair to search."
-    )
-    date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("date", "")
-    )
-    search: Optional[str] = Field(
-        default="",
-        description="Search for terms within the ticker and/or company name.",
-    )
-    active: Optional[bool] = Field(
-        default=True,
-        description="Specify if the tickers returned should be actively traded on the queried date.",
-    )
-    order: Optional[Literal["asc", "desc"]] = Field(
-        default="asc", description="Order data by ascending or descending."
-    )
-    sort: Optional[
-        Literal[
-            "ticker",
-            "name",
-            "market",
-            "locale",
-            "currency_symbol",
-            "currency_name",
-            "base_currency_symbol",
-            "base_currency_name",
-            "last_updated_utc",
-            "delisted_utc",
-        ]
-    ] = Field(default="", description="Sort field used for ordering.")
-    limit: Optional[PositiveInt] = Field(
-        default=1000, description=QUERY_DESCRIPTIONS.get("limit", "")
-    )
-
 
 class PolygonCurrencyPairsData(CurrencyPairsData):
     """Polygon Currency Available Pairs Data."""
 
-    market: str = Field(description="Name of the trading market. Always 'fx'.")
-    locale: str = Field(description="Locale of the currency pair.")
+    __alias_dict__ = {
+        "last_updated": "last_updated_utc",
+        "delisted": "delisted_utc",
+        "name": "currency_name",
+        "symbol": "ticker",
+    }
     currency_symbol: Optional[str] = Field(
         default=None, description="The symbol of the quote currency."
     )
-    currency_name: Optional[str] = Field(
-        default=None, description="Name of the quote currency."
-    )
     base_currency_symbol: Optional[str] = Field(
         default=None, description="The symbol of the base currency."
     )
     base_currency_name: Optional[str] = Field(
         default=None, description="Name of the base currency."
     )
-    last_updated_utc: datetime = Field(description="The last updated timestamp in UTC.")
-    delisted_utc: Optional[datetime] = Field(
-        default=None, description="The delisted timestamp in UTC."
+    market: str = Field(description="Name of the trading market. Always 'fx'.")
+    locale: str = Field(description="Locale of the currency pair.")
+    last_updated: Optional[dateType] = Field(
+        default=None, description="The date the reference data was last updated."
+    )
+    delisted: Optional[dateType] = Field(
+        default=None, description="The date the item was delisted."
     )
 
-    @field_validator("last_updated_utc", mode="before", check_fields=False)
+    @field_validator("last_updated", "delisted", mode="before", check_fields=False)
     @classmethod
     def last_updated_utc_validate(cls, v):  # pylint: disable=E0213
         """Return the parsed last updated timestamp in UTC."""
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ")
-
-    @field_validator("delisted_utc", mode="before", check_fields=False)
-    @classmethod
-    def delisted_utc_validate(cls, v):  # pylint: disable=E0213
-        """Return the parsed delisted timestamp in UTC."""
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ")
+        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ").date() if v else None
 
 
 class PolygonCurrencyPairsFetcher(
     Fetcher[
         PolygonCurrencyPairsQueryParams,
         List[PolygonCurrencyPairsData],
     ]
 ):
-    """Transform the query, extract and transform the data from the Polygon endpoints."""
+    """Polygon Currency Pairs Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> PolygonCurrencyPairsQueryParams:
-        """Transform the query parameters. Ticker is set if symbol is provided."""
-        transform_params = params
-        now = datetime.now().date().isoformat()
-        transform_params["symbol"] = (
-            f"ticker=C:{params.get('symbol').upper()}" if params.get("symbol") else ""
-        )
-        if params.get("date") is None:
-            transform_params["date"] = now
-
-        return PolygonCurrencyPairsQueryParams(**transform_params)
+        """Transform the query parameters."""
+        return PolygonCurrencyPairsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: PolygonCurrencyPairsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
-    ) -> List[dict]:
+    ) -> List[Dict]:
         """Extract the data from the Polygon API."""
         api_key = credentials.get("polygon_api_key") if credentials else ""
-
         request_url = (
             f"https://api.polygon.io/v3/reference/"
-            f"tickers?{query.symbol}&market=fx&date={query.date}&"
-            f"search={query.search}&active={query.active}&order={query.order}&"
-            f"limit={query.limit}&sort={query.sort}&apiKey={api_key}"
+            f"tickers?&market=fx&limit=1000"
+            f"&apiKey={api_key}"
         )
-
         data = {"next_url": request_url}
         all_data: List[Dict] = []
-
         while "next_url" in data:
             data = await get_data(request_url, **kwargs)
-
             if isinstance(data, list):
                 raise ValueError("Expected a dict, got a list")
-
             if len(data["results"]) == 0:
                 raise RuntimeError(
                     "No results found. Please change your query parameters."
                 )
-
             if data["status"] == "OK":
                 results = data.get("results")
                 if not isinstance(results, list):
                     raise ValueError(
                         "Expected 'results' to be a list, got something else."
                     )
                 all_data.extend(results)
             elif data["status"] == "ERROR":
                 raise UserWarning(data["error"])
-
             if "next_url" in data:
                 request_url = f"{data['next_url']}&apiKey={api_key}"
-
         return all_data
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: PolygonCurrencyPairsQueryParams,
-        data: List[dict],
+        data: List[Dict],
         **kwargs: Any,
     ) -> List[PolygonCurrencyPairsData]:
-        """Transform the data into a list of PolygonCurrencyPairsData."""
-        return [PolygonCurrencyPairsData.model_validate(d) for d in data]
+        """Filter data by search query and validate the model."""
+        if not data:
+            raise EmptyDataError("The request was returned empty.")
+        df = DataFrame(data)
+        df["ticker"] = df["ticker"].str.replace("C:", "")
+        if query.query:
+            df = df[
+                df["name"].str.contains(query.query, case=False)
+                | df["base_currency_name"].str.contains(query.query, case=False)
+                | df["currency_name"].str.contains(query.query, case=False)
+                | df["base_currency_symbol"].str.contains(query.query, case=False)
+                | df["currency_symbol"].str.contains(query.query, case=False)
+                | df["ticker"].str.contains(query.query, case=False)
+            ]
+        if len(df) == 0:
+            raise EmptyDataError(
+                f"No results were found with the query supplied. -> {query.query}"
+            )
+        return [
+            PolygonCurrencyPairsData.model_validate(d) for d in df.to_dict("records")
+        ]
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/equity_historical.py` & `openbb_polygon-1.2.0/openbb_polygon/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class PolygonEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Polygon Equity Historical Price Query.
 
     Source: https://polygon.io/docs/stocks/getting-started
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/equity_nbbo.py` & `openbb_polygon-1.2.0/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/income_statement.py` & `openbb_polygon-1.2.0/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/index_historical.py` & `openbb_polygon-1.2.0/openbb_polygon/models/index_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class PolygonIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """Polygon Index Historical Query.
 
     Source: https://polygon.io/docs/indices/getting-started
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/market_indices.py` & `openbb_polygon-1.2.0/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/openbb_polygon/models/market_snapshots.py` & `openbb_polygon-1.2.0/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/openbb_polygon/utils/helpers.py` & `openbb_polygon-1.2.0/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.1.5/PKG-INFO` & `openbb_polygon-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-polygon
-Version: 1.1.5
+Version: 1.2.0
 Summary: Polygon extension for OpenBB
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
 
 # OpenBB Polygon Provider
 
 This extension integrates the [Polygon](https://polygon.io/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-polygon
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

