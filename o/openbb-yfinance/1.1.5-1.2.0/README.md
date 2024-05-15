# Comparing `tmp/openbb_yfinance-1.1.5.tar.gz` & `tmp/openbb_yfinance-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_yfinance-1.1.5.tar", max compression
+gzip compressed data, was "openbb_yfinance-1.2.0.tar", max compression
```

## Comparing `openbb_yfinance-1.1.5.tar` & `openbb_yfinance-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      450 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/README.md
--rw-r--r--   0        0        0     4232 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-04-19 16:31:25.550563 openbb_yfinance-1.1.5/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5858 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10102 2024-04-19 16:31:25.550563 openbb_yfinance-1.1.5/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-04-19 13:09:31.739184 openbb_yfinance-1.1.5/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-17 12:33:20.849645 openbb_yfinance-1.1.5/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0      484 2024-04-19 16:42:17.983382 openbb_yfinance-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 openbb_yfinance-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      323 2024-05-15 14:24:24.418114 openbb_yfinance-1.2.0/README.md
+-rw-r--r--   0        0        0     4166 2024-05-14 15:30:05.622090 openbb_yfinance-1.2.0/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.979066 openbb_yfinance-1.2.0/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-23 10:22:39.801074 openbb_yfinance-1.2.0/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-04-08 12:02:16.765334 openbb_yfinance-1.2.0/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-04-23 10:22:39.801195 openbb_yfinance-1.2.0/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-04-08 12:02:16.765440 openbb_yfinance-1.2.0/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-04-08 12:02:16.765519 openbb_yfinance-1.2.0/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2869 2024-05-10 10:40:27.305123 openbb_yfinance-1.2.0/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3456 2024-05-10 10:40:27.305369 openbb_yfinance-1.2.0/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3367 2024-05-10 10:40:27.305501 openbb_yfinance-1.2.0/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6677 2024-05-10 10:40:27.305644 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5868 2024-05-10 10:40:27.305756 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3896 2024-05-10 10:40:27.305887 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-04-02 11:35:59.651682 openbb_yfinance-1.2.0/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10128 2024-05-10 10:40:27.306032 openbb_yfinance-1.2.0/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-04-08 12:02:16.766367 openbb_yfinance-1.2.0/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4717 2024-05-10 10:40:27.306188 openbb_yfinance-1.2.0/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-04-08 12:02:16.766529 openbb_yfinance-1.2.0/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-04-08 12:02:16.766617 openbb_yfinance-1.2.0/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-04-08 12:02:16.766677 openbb_yfinance-1.2.0/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-04-08 12:02:16.766770 openbb_yfinance-1.2.0/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4069 2024-05-10 10:40:27.306306 openbb_yfinance-1.2.0/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-04-08 12:02:16.766930 openbb_yfinance-1.2.0/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10194 2024-05-10 10:40:27.306403 openbb_yfinance-1.2.0/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-04-08 12:02:16.767101 openbb_yfinance-1.2.0/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4682 2024-05-10 10:40:27.308919 openbb_yfinance-1.2.0/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4236 2024-05-10 10:40:27.309704 openbb_yfinance-1.2.0/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6039 2024-05-10 10:40:27.309963 openbb_yfinance-1.2.0/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-04-08 12:02:16.767403 openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-04-08 12:02:16.767490 openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.980652 openbb_yfinance-1.2.0/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-02-29 11:03:36.980745 openbb_yfinance-1.2.0/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-04-02 11:35:59.654237 openbb_yfinance-1.2.0/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-04-23 10:22:39.801794 openbb_yfinance-1.2.0/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-04-08 12:02:16.767762 openbb_yfinance-1.2.0/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0      510 2024-05-15 16:05:12.832912 openbb_yfinance-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 openbb_yfinance-1.2.0/PKG-INFO
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/__init__.py` & `openbb_yfinance-1.2.0/openbb_yfinance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,29 @@
 from openbb_yfinance.models.income_statement import YFinanceIncomeStatementFetcher
 from openbb_yfinance.models.index_historical import (
     YFinanceIndexHistoricalFetcher,
 )
 from openbb_yfinance.models.key_executives import YFinanceKeyExecutivesFetcher
 from openbb_yfinance.models.key_metrics import YFinanceKeyMetricsFetcher
 from openbb_yfinance.models.losers import YFLosersFetcher
-from openbb_yfinance.models.market_indices import (
-    YFinanceMarketIndicesFetcher,
-)
 from openbb_yfinance.models.price_target_consensus import (
     YFinancePriceTargetConsensusFetcher,
 )
 from openbb_yfinance.models.share_statistics import YFinanceShareStatisticsFetcher
 from openbb_yfinance.models.undervalued_growth_equities import (
     YFUndervaluedGrowthEquitiesFetcher,
 )
 from openbb_yfinance.models.undervalued_large_caps import YFUndervaluedLargeCapsFetcher
 
 yfinance_provider = Provider(
     name="yfinance",
-    website="https://finance.yahoo.com/",
+    website="https://finance.yahoo.com",
     description="""Yahoo! Finance is a web-based platform that offers financial news,
-    data, and tools for investors and individuals interested in tracking and analyzing
-    financial markets and assets.""",
+data, and tools for investors and individuals interested in tracking and analyzing
+financial markets and assets.""",
     fetcher_dict={
         "AvailableIndices": YFinanceAvailableIndicesFetcher,
         "BalanceSheet": YFinanceBalanceSheetFetcher,
         "CashFlowStatement": YFinanceCashFlowStatementFetcher,
         "CompanyNews": YFinanceCompanyNewsFetcher,
         "CryptoHistorical": YFinanceCryptoHistoricalFetcher,
         "CurrencyHistorical": YFinanceCurrencyHistoricalFetcher,
@@ -71,8 +68,9 @@
         "IndexHistorical": YFinanceIndexHistoricalFetcher,
         "KeyExecutives": YFinanceKeyExecutivesFetcher,
         "KeyMetrics": YFinanceKeyMetricsFetcher,
         "MarketIndices": YFinanceIndexHistoricalFetcher,
         "PriceTargetConsensus": YFinancePriceTargetConsensusFetcher,
         "ShareStatistics": YFinanceShareStatisticsFetcher,
     },
+    repr_name="Yahoo Finance",
 )
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/active.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/available_indices.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/balance_sheet.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/cash_flow.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/company_news.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/company_news.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class YFinanceCompanyNewsQueryParams(CompanyNewsQueryParams):
     """YFinance Company News Query.
 
     Source: https://finance.yahoo.com/news/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceCompanyNewsData(CompanyNewsData):
     """YFinance Company News Data."""
 
     __alias_dict__ = {
         "symbols": "relatedTickers",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/crypto_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class YFinanceCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Yahoo Finance Crypto Historical Price Query.
 
     Source: https://finance.yahoo.com/crypto/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/currency_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/currency_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class YFinanceCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Yahoo Finance Currency Price Query.
 
     Source: https://finance.yahoo.com/currencies/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class YFinanceEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Yahoo Finance Equity Historical Price Query.
 
     Source: https://finance.yahoo.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_profile.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEquityProfileQueryParams(EquityInfoQueryParams):
     """YFinance Equity Profile Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEquityProfileData(EquityInfoData):
     """YFinance Equity Profile Data."""
 
     __alias_dict__ = {
         "name": "longName",
@@ -87,15 +87,15 @@
         description="The reported number of shares short.",
         default=None,
         alias="sharesShort",
     )
     dividend_yield: Optional[float] = Field(
         description="The dividend yield of the asset, as a normalized percent.",
         default=None,
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="yield",
     )
     beta: Optional[float] = Field(
         description="The beta of the asset relative to the broad market.",
         default=None,
     )
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/equity_quote.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEquityQuoteQueryParams(EquityQuoteQueryParams):
     """YFinance Equity Quote Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEquityQuoteData(EquityQuoteData):
     """YFinance Equity Quote Data."""
 
     __alias_dict__ = {
         "name": "longName",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/etf_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/etf_info.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/etf_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEtfInfoQueryParams(EtfInfoQueryParams):
     """YFinance ETF Info Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEtfInfoData(EtfInfoData):
     """YFinance ETF Info Data."""
 
     __alias_dict__ = {
         "name": "longName",
@@ -74,26 +74,26 @@
         default=None,
         description="The trailing twelve month P/E ratio of the fund's assets.",
         alias="trailingPE",
     )
     dividend_yield: Optional[float] = Field(
         default=None,
         description="The dividend yield of the fund, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="yield",
     )
     dividend_rate_ttm: Optional[float] = Field(
         default=None,
         description="The trailing twelve month annual dividend rate of the fund, in currency units.",
         alias="trailingAnnualDividendRate",
     )
     dividend_yield_ttm: Optional[float] = Field(
         default=None,
         description="The trailing twelve month annual dividend yield of the fund, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="trailingAnnualDividendYield",
     )
     year_high: Optional[float] = Field(
         default=None,
         description="The fifty-two week high price.",
         alias="fiftyTwoWeekHigh",
     )
@@ -111,27 +111,27 @@
         default=None,
         description="200-day moving average price.",
         alias="twoHundredDayAverage",
     )
     return_ytd: Optional[float] = Field(
         default=None,
         description="The year-to-date return of the fund, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="ytdReturn",
     )
     return_3y_avg: Optional[float] = Field(
         default=None,
         description="The three year average return of the fund, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="threeYearAverageReturn",
     )
     return_5y_avg: Optional[float] = Field(
         default=None,
         description="The five year average return of the fund, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="fiveYearAverageReturn",
     )
     beta_3y_avg: Optional[float] = Field(
         default=None,
         description="The three year average beta of the fund.",
         alias="beta3Year",
     )
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/futures_curve.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/futures_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/futures_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class YFinanceFuturesHistoricalQueryParams(FuturesHistoricalQueryParams):
     """Yahoo Finance Futures historical Price Query.
 
     Source: https://finance.yahoo.com/crypto/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/gainers.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/growth_tech_equities.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/historical_dividends.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/income_statement.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/index_historical.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/index_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class YFinanceIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """YFinance Index Historical Query.
 
     Source: https://finance.yahoo.com/world-indices
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/key_executives.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/key_metrics.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/key_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceKeyMetricsQueryParams(KeyMetricsQueryParams):
     """YFinance Key Metrics Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceKeyMetricsData(KeyMetricsData):
     """YFinance Key Metrics Data."""
 
     __alias_dict__ = {
         "market_cap": "marketCap",
@@ -63,26 +63,26 @@
         default=None,
         description="Earnings growth (Year Over Year), as a normalized percent.",
         alias="earningsGrowth",
     )
     earnings_growth_quarterly: Optional[float] = Field(
         default=None,
         description="Quarterly earnings growth (Year Over Year), as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="earningsQuarterlyGrowth",
     )
     revenue_per_share: Optional[float] = Field(
         default=None,
         description="Revenue per share (TTM).",
         alias="revenuePerShare",
     )
     revenue_growth: Optional[float] = Field(
         default=None,
         description="Revenue growth (Year Over Year), as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="revenueGrowth",
     )
     enterprise_to_revenue: Optional[float] = Field(
         default=None,
         description="Enterprise value to revenue ratio.",
         alias="enterpriseToRevenue",
     )
@@ -105,57 +105,57 @@
         default=None,
         description="Debt-to-equity ratio.",
         alias="debtToEquity",
     )
     gross_margin: Optional[float] = Field(
         default=None,
         description="Gross margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="grossMargins",
     )
     operating_margin: Optional[float] = Field(
         default=None,
         description="Operating margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="operatingMargins",
     )
     ebitda_margin: Optional[float] = Field(
         default=None,
         description="EBITDA margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="ebitdaMargins",
     )
     profit_margin: Optional[float] = Field(
         default=None,
         description="Profit margin, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="profitMargins",
     )
     return_on_assets: Optional[float] = Field(
         default=None,
         description="Return on assets, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="returnOnAssets",
     )
     return_on_equity: Optional[float] = Field(
         default=None,
         description="Return on equity, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="returnOnEquity",
     )
     dividend_yield: Optional[float] = Field(
         default=None,
         description="Dividend yield, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="dividendYield",
     )
     dividend_yield_5y_avg: Optional[float] = Field(
         default=None,
         description="5-year average dividend yield, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="fiveYearAvgDividendYield",
     )
     payout_ratio: Optional[float] = Field(
         default=None,
         description="Payout ratio.",
     )
     book_value: Optional[float] = Field(
@@ -201,15 +201,15 @@
     beta: Optional[float] = Field(
         default=None,
         description="Beta relative to the broad market (5-year monthly).",
     )
     price_return_1y: Optional[float] = Field(
         default=None,
         description="One-year price return, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="52WeekChange",
     )
     currency: Optional[str] = Field(
         default=None,
         description="Currency in which the data is presented.",
         alias="financialCurrency",
     )
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/losers.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/market_indices.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/market_indices.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class YFinanceMarketIndicesQueryParams(MarketIndicesQueryParams):
     """YFinance Market Indices Query.
 
     Source: https://finance.yahoo.com/world-indices
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Optional[INTERVALS] = Field(default="1d", description="Data granularity.")
     period: Optional[PERIODS] = Field(
         default="max", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     prepost: bool = Field(default=True, description="Include Pre and Post market data.")
     rounding: bool = Field(default=True, description="Round prices to two decimals?")
@@ -57,15 +57,15 @@
 
         if params.get("start_date") is None:
             transformed_params["start_date"] = now - relativedelta(years=1)
 
         if params.get("end_date") is None:
             transformed_params["end_date"] = now
 
-        tickers = params.get("symbol").lower().split(",")
+        tickers = params.get("symbol", "").lower().split(",")
 
         new_tickers = []
         for ticker in tickers:
             _ticker = ""
             indices = pd.DataFrame(INDICES).transpose().reset_index()
             indices.columns = ["code", "name", "symbol"]
 
@@ -119,15 +119,15 @@
         if query.start_date:
             if "date" in data.columns:
                 data.set_index("date", inplace=True)
                 data.index = to_datetime(data.index)
 
             data = data[
                 (data.index >= to_datetime(query.start_date))
-                & (data.index <= to_datetime(query.end_date + timedelta(days=days)))
+                & (data.index <= to_datetime(query.end_date + timedelta(days=days)))  # type: ignore[operator]
             ]
 
         data.reset_index(inplace=True)
         data.rename(columns={"index": "date"}, inplace=True)
 
         return data.to_dict("records")
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/price_target_consensus.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinancePriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """YFinance Price Target Consensus Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for yFinance.")
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/share_statistics.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/share_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceShareStatisticsQueryParams(ShareStatisticsQueryParams):
     """YFinance Share Statistics Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceShareStatisticsData(ShareStatisticsData):
     """YFinance Share Statistics Data."""
 
     __alias_dict__ = {
         "outstanding_shares": "sharesOutstanding",
@@ -45,15 +45,15 @@
         default=None,
         description="Number of shares that are reported short.",
         alias="sharesShort",
     )
     short_percent_of_float: Optional[float] = Field(
         default=None,
         description="Percentage of shares that are reported short, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="shortPercentOfFloat",
     )
     days_to_cover: Optional[float] = Field(
         default=None,
         description="Number of days to repurchase the shares as a ratio of average daily volume",
         alias="shortRatio",
     )
@@ -66,27 +66,27 @@
         default=None,
         description="Date of the previous month's report.",
         alias="sharesShortPreviousMonthDate",
     )
     insider_ownership: Optional[float] = Field(
         default=None,
         description="Percentage of shares held by insiders, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="heldPercentInsiders",
     )
     institution_ownership: Optional[float] = Field(
         default=None,
         description="Percentage of shares held by institutions, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="heldPercentInstitutions",
     )
     institution_float_ownership: Optional[float] = Field(
         default=None,
         description="Percentage of float held by institutions, as a normalized percent.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="institutionsFloatPercentHeld",
     )
     institutions_count: Optional[int] = Field(
         default=None,
         description="Number of institutions holding shares.",
         alias="institutionsCount",
     )
```

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/utils/futures.csv` & `openbb_yfinance-1.2.0/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/utils/helpers.py` & `openbb_yfinance-1.2.0/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/openbb_yfinance/utils/references.py` & `openbb_yfinance-1.2.0/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.1.5/PKG-INFO` & `openbb_yfinance-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-yfinance
-Version: 1.1.5
+Version: 1.2.0
 Summary: yfinance extension for OpenBB
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
 Requires-Dist: yfinance (>=0.2.27,<0.3.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Yahoo!Finance Provider
 
 This extension integrates the [Yahoo!Finance](https://finance.yahoo.com/) data provider into the OpenBB Platform.
 
@@ -23,11 +25,9 @@
 
 To install the extension:
 
 ```bash
 pip install openbb-yfinance
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

