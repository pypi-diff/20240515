# Comparing `tmp/openbb_tmx-1.0.2.tar.gz` & `tmp/openbb_tmx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tmx-1.0.2.tar", max compression
+gzip compressed data, was "openbb_tmx-1.1.0.tar", max compression
```

## Comparing `openbb_tmx-1.0.2.tar` & `openbb_tmx-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2369 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/README.md
--rw-r--r--   0        0        0     3319 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5162 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8843 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12451 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10325 2024-04-19 13:10:31.748034 openbb_tmx-1.0.2/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-04-17 12:33:20.781645 openbb_tmx-1.0.2/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0      636 2024-04-19 16:41:11.435221 openbb_tmx-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openbb_tmx-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2637 2024-05-15 14:32:00.047970 openbb_tmx-1.1.0/README.md
+-rw-r--r--   0        0        0     3325 2024-05-14 15:30:05.619866 openbb_tmx-1.1.0/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-23 10:22:39.794265 openbb_tmx-1.1.0/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-04-08 12:02:16.691753 openbb_tmx-1.1.0/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6306 2024-05-09 15:04:29.073848 openbb_tmx-1.1.0/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5166 2024-05-09 15:04:29.073990 openbb_tmx-1.1.0/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-04-08 12:02:16.691957 openbb_tmx-1.1.0/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4653 2024-05-10 10:40:27.302449 openbb_tmx-1.1.0/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8853 2024-05-10 10:40:27.302575 openbb_tmx-1.1.0/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5461 2024-05-10 10:40:27.302741 openbb_tmx-1.1.0/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12481 2024-05-10 10:40:27.302886 openbb_tmx-1.1.0/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-04-08 12:02:16.692386 openbb_tmx-1.1.0/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3644 2024-05-10 10:40:27.303031 openbb_tmx-1.1.0/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5093 2024-05-09 15:04:29.074766 openbb_tmx-1.1.0/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8463 2024-05-10 10:40:27.303171 openbb_tmx-1.1.0/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9711 2024-05-09 15:04:29.075187 openbb_tmx-1.1.0/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-04-08 12:02:16.692727 openbb_tmx-1.1.0/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-04-23 10:22:39.794929 openbb_tmx-1.1.0/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-04-08 12:02:16.692861 openbb_tmx-1.1.0/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-04-23 10:22:39.795036 openbb_tmx-1.1.0/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-04-08 12:02:16.692990 openbb_tmx-1.1.0/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10349 2024-05-09 15:04:29.075380 openbb_tmx-1.1.0/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-04-23 10:22:39.795263 openbb_tmx-1.1.0/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-04-08 12:02:16.693188 openbb_tmx-1.1.0/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5996 2024-05-10 10:40:27.303285 openbb_tmx-1.1.0/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5132 2024-05-09 13:34:29.362361 openbb_tmx-1.1.0/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:02:16.693325 openbb_tmx-1.1.0/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-04-23 10:22:39.795468 openbb_tmx-1.1.0/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-04-08 12:02:16.693456 openbb_tmx-1.1.0/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-04-23 10:22:39.795669 openbb_tmx-1.1.0/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0      662 2024-05-15 16:07:21.293855 openbb_tmx-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 openbb_tmx-1.1.0/PKG-INFO
```

### Comparing `openbb_tmx-1.0.2/README.md` & `openbb_tmx-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# openbb-tmx: A Community Data Provider Extension
+# OpenBB TMX Provider
+
+This extension integrates the [TMX](https://www.tmx.com) data provider into the OpenBB Platform.
+
+## Installation
+
+To install the extension:
+
+```bash
+pip install openbb-tmx
+```
+
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
+
+## Additional information
 
 `openbb-tmx` is an unofficial, community, data provider extension for the OpenBB Platform.
 
 Install with `pip install openbb-tmx`, or from the local directory, `pip install -e .`
 
 ## Command Coverage
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/__init__.py` & `openbb_tmx-1.1.0/openbb_tmx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 from openbb_tmx.models.insider_trading import TmxInsiderTradingFetcher
 from openbb_tmx.models.options_chains import TmxOptionsChainsFetcher
 from openbb_tmx.models.price_target_consensus import TmxPriceTargetConsensusFetcher
 from openbb_tmx.models.treasury_prices import TmxTreasuryPricesFetcher
 
 tmx_provider = Provider(
     name="tmx",
-    website="https://www.tmx.com/",
+    website="https://www.tmx.com",
     description="""Unofficial TMX Data Provider Extension
-        TMX Group Companies
-         - Toronto Stock Exchange
-         - TSX Venture Exchange
-         - TSX Trust
-         - Montréal Exchange
-         - TSX Alpha Exchange
-         - Shorcan
-         - CDCC
-         - CDS
-         - TMX Datalinx
-         - Trayport
+    TMX Group Companies
+        - Toronto Stock Exchange
+        - TSX Venture Exchange
+        - TSX Trust
+        - Montréal Exchange
+        - TSX Alpha Exchange
+        - Shorcan
+        - CDCC
+        - CDS
+        - TMX Datalinx
+        - Trayport
     """,
     fetcher_dict={
         "AvailableIndices": TmxAvailableIndicesFetcher,
         "BondPrices": TmxBondPricesFetcher,
         "CalendarEarnings": TmxCalendarEarningsFetcher,
         "CompanyFilings": TmxCompanyFilingsFetcher,
         "CompanyNews": TmxCompanyNewsFetcher,
@@ -63,8 +63,9 @@
         "IndexSectors": TmxIndexSectorsFetcher,
         "IndexSnapshots": TmxIndexSnapshotsFetcher,
         "InsiderTrading": TmxInsiderTradingFetcher,
         "OptionsChains": TmxOptionsChainsFetcher,
         "PriceTargetConsensus": TmxPriceTargetConsensusFetcher,
         "TreasuryPrices": TmxTreasuryPricesFetcher,
     },
+    repr_name="TMX",
 )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/available_indices.py` & `openbb_tmx-1.1.0/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/bond_prices.py` & `openbb_tmx-1.1.0/openbb_tmx/models/bond_prices.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         default=None,
         description="Yield to maturity (YTM) is the rate of return anticipated on a bond"
         + " if it is held until the maturity date. It takes into account"
         + " the current market price, par value, coupon rate and time to maturity. It is assumed that all"
         + " coupons are reinvested at the same rate."
         + " Values are returned as a normalized percent.",
         alias="lastYield",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     price: Optional[float] = Field(
         default=None,
         description="The last price for the bond.",
         alias="lastPrice",
     )
     highest_price: Optional[float] = Field(
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/calendar_earnings.py` & `openbb_tmx-1.1.0/openbb_tmx/models/calendar_earnings.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     )
     eps_surprise: Optional[float] = Field(
         default=None, description="The EPS surprise in dollars."
     )
     surprise_percent: Optional[float] = Field(
         default=None,
         description="The EPS surprise as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     reporting_time: Optional[str] = Field(
         default=None,
         description="The time of the report - i.e., before or after market.",
     )
 
     @field_validator("surprise_percent", mode="before", check_fields=False)
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/company_filings.py` & `openbb_tmx-1.1.0/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/company_news.py` & `openbb_tmx-1.1.0/openbb_tmx/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxCompanyNewsQueryParams(CompanyNewsQueryParams):
     """TMX Stock News query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=1, description="The page number to start from. Use with limit."
     )
 
     @field_validator("symbol", mode="before")
     @classmethod
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/equity_historical.py` & `openbb_tmx-1.1.0/openbb_tmx/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Canadian Depositary Receipts (CDRs) are: "AAPL:AQL"
 
     CDRs are the underlying asset for CAD-hedged assets.
 
     source: https://money.tmx.com
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Union[
         Literal["1m", "2m", "5m", "15m", "30m", "60m", "1h", "1d", "1W", "1M"], str, int
     ] = Field(  # type: ignore
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " Or, any integer (entered as a string) representing the number of minutes."
         + " Default is daily data."
@@ -96,15 +96,15 @@
     vwap: Optional[float] = Field(
         description="Volume weighted average price for the day.", default=None
     )
     change: Optional[float] = Field(description="Change in price.", default=None)
     change_percent: Optional[float] = Field(
         description="Change in price, as a normalized percentage.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     transactions: Optional[int] = Field(
         description="Total number of transactions recorded.", default=None
     )
     transactions_value: Optional[float] = Field(
         description="Nominal value of recorded transactions.", default=None
     )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/equity_profile.py` & `openbb_tmx-1.1.0/openbb_tmx/models/equity_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, model_validator
 
 
 class TmxEquityProfileQueryParams(EquityInfoQueryParams):
     """TMX Equity Profile query params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TmxEquityProfileData(EquityInfoData):
     """TMX Equity Profile Data."""
 
     __alias_dict__ = {
         "short_description": "shortDescription",
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/equity_quote.py` & `openbb_tmx-1.1.0/openbb_tmx/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 _warn = warnings.warn
 
 
 class TmxEquityQuoteQueryParams(EquityQuoteQueryParams):
     """TMX Equity Profile query params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TmxEquityQuoteData(EquityQuoteData):
     """TMX Equity Profile Data."""
 
     __alias_dict__ = {
         "last_price": "price",
@@ -95,15 +95,15 @@
     change: Optional[float] = Field(
         default=None,
         description="The change in price.",
     )
     change_percent: Optional[float] = Field(
         default=None,
         description="The change in price as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     year_high: Optional[float] = Field(
         description="Fifty-two week high.", default=None, alias="weeks52high"
     )
     year_low: Optional[float] = Field(
         description="Fifty-two week low.", default=None, alias="weeks52low"
     )
@@ -147,15 +147,15 @@
         default=None,
         alias="dividendCurrency",
     )
     div_yield: Optional[float] = Field(
         description="The dividend yield as a normalized percentage.",
         default=None,
         alias="dividendYield",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     div_freq: Optional[str] = Field(
         description="The frequency of dividend payments.",
         default=None,
         alias="dividendFrequency",
     )
     div_ex_date: Optional[dateType] = Field(
@@ -166,21 +166,21 @@
         default=None,
         alias="dividendPayDate",
     )
     div_growth_3y: Optional[Union[float, str]] = Field(
         description="The three year dividend growth as a normalized percentage.",
         default=None,
         alias="dividend3Years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     div_growth_5y: Optional[Union[float, str]] = Field(
         description="The five year dividend growth as a normalized percentage.",
         default=None,
         alias="dividend5Years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     pe: Optional[Union[float, str]] = Field(
         description="The price to earnings ratio.", default=None, alias="peRatio"
     )
     eps: Optional[Union[float, str]] = Field(
         description="The earnings per share.", default=None
     )
@@ -195,21 +195,21 @@
         default=None,
         alias="priceToCashFlow",
     )
     return_on_equity: Optional[Union[float, str]] = Field(
         description="The return on equity, as a normalized percentage.",
         default=None,
         alias="returnOnEquity",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_on_assets: Optional[Union[float, str]] = Field(
         description="The return on assets, as a normalized percentage.",
         default=None,
         alias="returnOnAssets",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     beta: Optional[Union[float, str]] = Field(
         description="The beta relative to the TSX Composite.", default=None
     )
     alpha: Optional[Union[float, str]] = Field(
         description="The alpha relative to the TSX Composite.", default=None
     )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/equity_search.py` & `openbb_tmx-1.1.0/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/etf_countries.py` & `openbb_tmx-1.1.0/openbb_tmx/models/etf_countries.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 _warn = warnings.warn
 
 
 class TmxEtfCountriesQueryParams(EtfCountriesQueryParams):
     """TMX ETF Countries Query Params"""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request. All ETF data comes from a single JSON file that is updated daily."
         + " To bypass, set to False. If True, the data will be cached for 4 hours.",
     )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/etf_holdings.py` & `openbb_tmx-1.1.0/openbb_tmx/models/etf_holdings.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,29 +32,29 @@
     symbol: Optional[str] = Field(
         description="The ticker symbol of the asset.", default=None
     )
     name: Optional[str] = Field(description="The name of the asset.", default=None)
     weight: Optional[float] = Field(
         description="The weight of the asset in the portfolio, as a normalized percentage.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     shares: Optional[Union[int, str]] = Field(
         description="The value of the assets under management.",
         alias="number_of_shares",
         default=None,
     )
     market_value: Optional[Union[float, str]] = Field(
         description="The market value of the holding.", default=None
     )
     currency: Optional[str] = Field(description="The currency of the holding.")
     share_percentage: Optional[float] = Field(
         description="The share percentage of the holding, as a normalized percentage.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     share_change: Optional[Union[float, str]] = Field(
         description="The change in shares of the holding.", default=None
     )
     country: Optional[str] = Field(
         description="The country of the holding.", default=None
     )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/etf_info.py` & `openbb_tmx-1.1.0/openbb_tmx/models/etf_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from openbb_tmx.utils.helpers import get_all_etfs
 from pydantic import Field, field_validator
 
 
 class TmxEtfInfoQueryParams(EtfInfoQueryParams):
     """TMX ETF Info Query Params"""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request. All ETF data comes from a single JSON file that is updated daily."
         + " To bypass, set to False. If True, the data will be cached for 4 hours.",
     )
 
@@ -44,55 +44,55 @@
     close: Optional[float] = Field(description="The closing price of the ETF.")
     prev_close: Optional[float] = Field(
         description="The previous closing price of the ETF.", default=None
     )
     return_1m: Optional[float] = Field(
         description="The one-month return of the ETF, as a normalized percent",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_3m: Optional[float] = Field(
         description="The three-month return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_6m: Optional[float] = Field(
         description="The six-month return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_ytd: Optional[float] = Field(
         description="The year-to-date return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_1y: Optional[float] = Field(
         description="The one-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_3y: Optional[float] = Field(
         description="The three-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_5y: Optional[float] = Field(
         description="The five-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_10y: Optional[float] = Field(
         description="The ten-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_from_inception: Optional[float] = Field(
         description="The return from inception of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     avg_volume: Optional[int] = Field(
         description="The average daily volume of the ETF.",
         alias="volume_avg_daily",
         default=None,
     )
     avg_volume_30d: Optional[int] = Field(
@@ -106,25 +106,25 @@
     )
     pb_ratio: Optional[float] = Field(
         description="The price-to-book ratio of the ETF.", default=None
     )
     management_fee: Optional[float] = Field(
         description="The management fee of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     mer: Optional[float] = Field(
         description="The management expense ratio of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     distribution_yield: Optional[float] = Field(
         description="The distribution yield of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     dividend_frequency: Optional[str] = Field(
         description="The dividend payment frequency of the ETF.", default=None
     )
     website: Optional[str] = Field(description="The website of the ETF.", default=None)
     description: Optional[str] = Field(
         description="The description of the ETF.",
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/etf_search.py` & `openbb_tmx-1.1.0/openbb_tmx/models/etf_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,76 +73,76 @@
     close: Optional[float] = Field(description="The closing price of the ETF.")
     prev_close: Optional[float] = Field(
         description="The previous closing price of the ETF.", default=None
     )
     return_1m: Optional[float] = Field(
         description="The one-month return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_3m: Optional[float] = Field(
         description="The three-month return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_6m: Optional[float] = Field(
         description="The six-month return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_ytd: Optional[float] = Field(
         description="The year-to-date return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_1y: Optional[float] = Field(
         description="The one-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     beta_1y: Optional[float] = Field(
         description="The one-year beta of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_3y: Optional[float] = Field(
         description="The three-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     beta_3y: Optional[float] = Field(
         description="The three-year beta of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_5y: Optional[float] = Field(
         description="The five-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     beta_5y: Optional[float] = Field(
         description="The five-year beta of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_10y: Optional[float] = Field(
         description="The ten-year return of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     beta_10y: Optional[float] = Field(
         description="The ten-year beta of the ETF.", default=None
     )
     beta_15y: Optional[float] = Field(
         description="The fifteen-year beta of the ETF.", default=None
     )
     return_from_inception: Optional[float] = Field(
         description="The return from inception of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     avg_volume: Optional[int] = Field(
         description="The average daily volume of the ETF.",
         alias="volume_avg_daily",
         default=None,
     )
     avg_volume_30d: Optional[int] = Field(
@@ -156,25 +156,25 @@
     )
     pb_ratio: Optional[float] = Field(
         description="The price-to-book ratio of the ETF.", default=None
     )
     management_fee: Optional[float] = Field(
         description="The management fee of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     mer: Optional[float] = Field(
         description="The management expense ratio of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     distribution_yield: Optional[float] = Field(
         description="The distribution yield of the ETF, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     dividend_frequency: Optional[str] = Field(
         description="The dividend payment frequency of the ETF.", default=None
     )
 
     @field_validator(
         "distribution_yield",
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/etf_sectors.py` & `openbb_tmx-1.1.0/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/gainers.py` & `openbb_tmx-1.1.0/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/historical_dividends.py` & `openbb_tmx-1.1.0/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/index_constituents.py` & `openbb_tmx-1.1.0/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/index_sectors.py` & `openbb_tmx-1.1.0/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/index_snapshots.py` & `openbb_tmx-1.1.0/openbb_tmx/models/index_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from pydantic import Field, field_validator
 
 
 class TmxIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """TMX Index Snapshots Query Params."""
 
-    region: Literal[None, "ca", "us"] = Field(default="ca")  # type: ignore
+    region: Optional[Literal["ca", "us"]] = Field(default="ca")  # type: ignore
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request."
         + " Index data is from a single JSON file, updated each day after close."
         + " It is cached for one day. To bypass, set to False.",
     )
 
@@ -60,25 +60,25 @@
     )
     year_low: Optional[float] = Field(
         default=None, description="The 52-week low of the index."
     )
     return_mtd: Optional[float] = Field(
         default=None,
         description="The month-to-date return of the index, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_qtd: Optional[float] = Field(
         default=None,
         description="The quarter-to-date return of the index, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     return_ytd: Optional[float] = Field(
         default=None,
         description="The year-to-date return of the index, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     total_market_value: Optional[float] = Field(
         default=None,
         description="The total quoted market value of the index.",
     )
     number_of_constituents: Optional[int] = Field(
         default=None,
@@ -99,24 +99,24 @@
     constituent_largest_market_value: Optional[float] = Field(
         default=None,
         description="The largest quoted market value of the index constituents.",
     )
     constituent_largest_weight: Optional[float] = Field(
         default=None,
         description="The largest weight of the index constituents, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     constituent_smallest_market_value: Optional[float] = Field(
         default=None,
         description="The smallest quoted market value of the index constituents.",
     )
     constituent_smallest_weight: Optional[float] = Field(
         default=None,
         description="The smallest weight of the index constituents, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
 
     @field_validator(
         "return_mtd",
         "return_qtd",
         "return_ytd",
         "change_percent",
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/insider_trading.py` & `openbb_tmx-1.1.0/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/options_chains.py` & `openbb_tmx-1.1.0/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/price_target_consensus.py` & `openbb_tmx-1.1.0/openbb_tmx/models/price_target_consensus.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """TMX Price Target Consensus Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for TMX.")
@@ -38,15 +38,15 @@
         "target_low": "price_target_low",
         "target_upside": "price_target_upside",
     }
 
     target_upside: Optional[float] = Field(
         default=None,
         description="Percent of upside, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     total_analysts: Optional[int] = Field(
         default=None, description="Total number of analyst."
     )
     buy_ratings: Optional[int] = Field(
         default=None, description="Number of buy ratings."
     )
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/models/treasury_prices.py` & `openbb_tmx-1.1.0/openbb_tmx/models/treasury_prices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""TMX Treasury Prices Fetcher"""
+"""TMX Treasury Prices Fetcher."""
 
 # pylint: disable=unused-argument
 from datetime import (
     date as dateType,
-    datetime,
     timedelta,
 )
 from typing import Any, Dict, List, Literal, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.treasury_prices import (
     TreasuryPricesData,
@@ -15,16 +14,15 @@
 )
 from openbb_tmx.utils.helpers import get_all_bonds
 from pandas import DataFrame
 from pydantic import Field, field_validator
 
 
 class TmxTreasuryPricesQueryParams(TreasuryPricesQueryParams):
-    """
-    TMX Treasury Prices Query Params.
+    """TMX Treasury Prices Query Params.
 
     Data will be made available by 5:00 EST on T+1
 
     Source: https://bondtradedata.iiroc.ca/#/
     """
 
     govt_type: Literal["federal", "provincial", "municipal"] = Field(
@@ -95,21 +93,22 @@
 ):
     """Tmx Bond Reference Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxTreasuryPricesQueryParams:
         """Transform query params."""
         transformed_params = params.copy()
-        now = datetime.now()
-        if now.date().weekday() > 4:
-            now = now - timedelta(now.date().weekday() - 4)
+        yesterday = dateType.today() - timedelta(days=1)
+        last_bd = (
+            yesterday - timedelta(yesterday.weekday() - 4)
+            if yesterday.weekday() > 4
+            else yesterday
+        )
         if "maturity_date_min" not in transformed_params:
-            transformed_params["maturity_date_min"] = (
-                now - timedelta(days=1)
-            ).strftime("%Y-%m-%d")
+            transformed_params["maturity_date_min"] = last_bd
         return TmxTreasuryPricesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
         query: TmxTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
```

### Comparing `openbb_tmx-1.0.2/openbb_tmx/utils/gql.py` & `openbb_tmx-1.1.0/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/openbb_tmx/utils/helpers.py` & `openbb_tmx-1.1.0/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.0.2/pyproject.toml` & `openbb_tmx-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "openbb-tmx"
-version = "1.0.2"
+version = "1.1.0"
 description = "Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API."
 authors = ["OpenBB <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_tmx" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-aiohttp-client-cache = "^0.10.0"
-aiosqlite = "^0.19.0"
+aiohttp-client-cache = "^0.11.0"
+aiosqlite = "^0.20.0"
 random-user-agent = "^1.0.1"
 exchange-calendars = "^4.2.8"
-openbb-core = "^1.1.6"
+openbb-core = "^1.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tmx = "openbb_tmx:tmx_provider"
```

### Comparing `openbb_tmx-1.0.2/PKG-INFO` & `openbb_tmx-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 Metadata-Version: 2.1
 Name: openbb-tmx
-Version: 1.0.2
+Version: 1.1.0
 Summary: Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API.
+License: AGPL-3.0-only
 Author: OpenBB
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp-client-cache (>=0.10.0,<0.11.0)
-Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
+Requires-Dist: aiohttp-client-cache (>=0.11.0,<0.12.0)
+Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: exchange-calendars (>=4.2.8,<5.0.0)
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
-# openbb-tmx: A Community Data Provider Extension
+# OpenBB TMX Provider
+
+This extension integrates the [TMX](https://www.tmx.com) data provider into the OpenBB Platform.
+
+## Installation
+
+To install the extension:
+
+```bash
+pip install openbb-tmx
+```
+
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
+
+## Additional information
 
 `openbb-tmx` is an unofficial, community, data provider extension for the OpenBB Platform.
 
 Install with `pip install openbb-tmx`, or from the local directory, `pip install -e .`
 
 ## Command Coverage
```

