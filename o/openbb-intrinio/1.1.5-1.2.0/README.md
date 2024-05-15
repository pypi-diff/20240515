# Comparing `tmp/openbb_intrinio-1.1.5.tar.gz` & `tmp/openbb_intrinio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_intrinio-1.1.5.tar", max compression
+gzip compressed data, was "openbb_intrinio-1.2.0.tar", max compression
```

## Comparing `openbb_intrinio-1.1.5.tar` & `openbb_intrinio-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      435 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/README.md
--rw-r--r--   0        0        0     5393 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-04-17 12:33:20.669645 openbb_intrinio-1.1.5/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22983 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     3273 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     8675 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7321 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-04-19 13:10:31.748034 openbb_intrinio-1.1.5/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-04-19 16:31:25.550563 openbb_intrinio-1.1.5/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     2560 2024-04-19 16:31:25.550563 openbb_intrinio-1.1.5/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-17 12:33:20.673645 openbb_intrinio-1.1.5/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0      489 2024-04-19 16:43:17.507536 openbb_intrinio-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 openbb_intrinio-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      308 2024-05-15 14:25:27.915403 openbb_intrinio-1.2.0/README.md
+-rw-r--r--   0        0        0     5944 2024-05-14 15:30:05.616440 openbb_intrinio-1.2.0/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-02-29 11:03:36.874926 openbb_intrinio-1.2.0/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22763 2024-05-09 13:34:29.221940 openbb_intrinio-1.2.0/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-04-08 12:02:16.650967 openbb_intrinio-1.2.0/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-04-08 12:02:16.651055 openbb_intrinio-1.2.0/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-04-02 11:35:59.478049 openbb_intrinio-1.2.0/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     9166 2024-05-10 10:40:27.297354 openbb_intrinio-1.2.0/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2939 2024-05-09 15:04:29.071560 openbb_intrinio-1.2.0/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     9171 2024-05-09 15:04:29.071762 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2382 2024-05-10 10:40:27.297486 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4980 2024-05-10 10:40:27.297645 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-04-02 11:35:59.478839 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-04-23 10:22:39.671958 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29033 2024-05-10 10:40:27.297866 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8343 2024-05-10 10:40:27.298055 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-04-08 12:02:16.651932 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-04-02 11:35:59.479335 openbb_intrinio-1.2.0/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-04-02 11:35:59.479441 openbb_intrinio-1.2.0/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8423 2024-05-10 10:40:27.298213 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     5005 2024-05-14 15:30:05.616608 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_pe_estimates.py
+-rw-r--r--   0        0        0     9700 2024-05-10 10:40:27.298372 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-04-02 11:35:59.479494 openbb_intrinio-1.2.0/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5102 2024-05-10 10:40:27.298529 openbb_intrinio-1.2.0/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-04-08 12:02:16.652255 openbb_intrinio-1.2.0/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-04-08 12:02:16.652375 openbb_intrinio-1.2.0/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3682 2024-05-10 10:40:27.298668 openbb_intrinio-1.2.0/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-04-08 12:02:16.652664 openbb_intrinio-1.2.0/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-04-02 11:35:59.480067 openbb_intrinio-1.2.0/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12545 2024-05-10 10:40:27.298912 openbb_intrinio-1.2.0/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3369 2024-05-10 10:40:27.299106 openbb_intrinio-1.2.0/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-04-02 11:35:59.480302 openbb_intrinio-1.2.0/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-04-23 10:22:39.672601 openbb_intrinio-1.2.0/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-04-08 12:02:16.653091 openbb_intrinio-1.2.0/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-04-08 12:02:16.653227 openbb_intrinio-1.2.0/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6519 2024-05-10 10:40:27.299281 openbb_intrinio-1.2.0/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-04-02 11:35:59.480930 openbb_intrinio-1.2.0/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-04-02 11:35:59.481011 openbb_intrinio-1.2.0/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-04-02 11:35:59.481085 openbb_intrinio-1.2.0/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     8655 2024-05-09 13:34:29.227363 openbb_intrinio-1.2.0/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.876946 openbb_intrinio-1.2.0/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-02-29 11:03:36.877031 openbb_intrinio-1.2.0/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-23 10:22:39.673143 openbb_intrinio-1.2.0/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-04-08 12:02:16.653631 openbb_intrinio-1.2.0/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0      515 2024-05-15 16:07:06.280254 openbb_intrinio-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_intrinio-1.2.0/PKG-INFO
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/__init__.py` & `openbb_intrinio-1.2.0/openbb_intrinio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     IntrinioEtfPricePerformanceFetcher,
 )
 from openbb_intrinio.models.etf_search import IntrinioEtfSearchFetcher
 from openbb_intrinio.models.financial_ratios import IntrinioFinancialRatiosFetcher
 from openbb_intrinio.models.forward_eps_estimates import (
     IntrinioForwardEpsEstimatesFetcher,
 )
+from openbb_intrinio.models.forward_pe_estimates import (
+    IntrinioForwardPeEstimatesFetcher,
+)
 from openbb_intrinio.models.forward_sales_estimates import (
     IntrinioForwardSalesEstimatesFetcher,
 )
 from openbb_intrinio.models.fred_series import IntrinioFredSeriesFetcher
 from openbb_intrinio.models.historical_attributes import (
     IntrinioHistoricalAttributesFetcher,
 )
@@ -51,17 +54,17 @@
     IntrinioSearchAttributesFetcher,
 )
 from openbb_intrinio.models.share_statistics import IntrinioShareStatisticsFetcher
 from openbb_intrinio.models.world_news import IntrinioWorldNewsFetcher
 
 intrinio_provider = Provider(
     name="intrinio",
-    website="https://intrinio.com/",
+    website="https://intrinio.com",
     description="""Intrinio is a financial data platform that provides real-time and
-    historical financial market data to businesses and developers through an API.""",
+historical financial market data to businesses and developers through an API.""",
     credentials=["api_key"],
     fetcher_dict={
         "BalanceSheet": IntrinioBalanceSheetFetcher,
         "CalendarIpo": IntrinioCalendarIpoFetcher,
         "CashFlowStatement": IntrinioCashFlowStatementFetcher,
         "CompanyFilings": IntrinioCompanyFilingsFetcher,
         "CompanyNews": IntrinioCompanyNewsFetcher,
@@ -73,14 +76,15 @@
         "EtfHistorical": IntrinioEquityHistoricalFetcher,
         "EtfHoldings": IntrinioEtfHoldingsFetcher,
         "EtfInfo": IntrinioEtfInfoFetcher,
         "EtfPricePerformance": IntrinioEtfPricePerformanceFetcher,
         "EtfSearch": IntrinioEtfSearchFetcher,
         "FinancialRatios": IntrinioFinancialRatiosFetcher,
         "ForwardEpsEstimates": IntrinioForwardEpsEstimatesFetcher,
+        "ForwardPeEstimates": IntrinioForwardPeEstimatesFetcher,
         "ForwardSalesEstimates": IntrinioForwardSalesEstimatesFetcher,
         "FredSeries": IntrinioFredSeriesFetcher,
         "HistoricalAttributes": IntrinioHistoricalAttributesFetcher,
         "HistoricalDividends": IntrinioHistoricalDividendsFetcher,
         "IncomeStatement": IntrinioIncomeStatementFetcher,
         "IndexHistorical": IntrinioIndexHistoricalFetcher,
         "InsiderTrading": IntrinioInsiderTradingFetcher,
@@ -93,8 +97,11 @@
         "OptionsUnusual": IntrinioOptionsUnusualFetcher,
         "PriceTargetConsensus": IntrinioPriceTargetConsensusFetcher,
         "ReportedFinancials": IntrinioReportedFinancialsFetcher,
         "SearchAttributes": IntrinioSearchAttributesFetcher,
         "ShareStatistics": IntrinioShareStatisticsFetcher,
         "WorldNews": IntrinioWorldNewsFetcher,
     },
+    repr_name="Intrinio",
+    v3_credentials=["API_INTRINIO_KEY"],
+    instructions="Go to: https://intrinio.com/starter-plan\n\n![Intrinio](https://user-images.githubusercontent.com/85772166/219207556-fcfee614-59f1-46ae-bff4-c63dd2f6991d.png)\n\nAn API key will be issued with a subscription. Find the token value within the account dashboard.",  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/balance_sheet.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/balance_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,14 @@
 
     period: Literal["annual", "quarter"] = Field(default="annual")
     fiscal_year: Optional[int] = Field(
         default=None,
         description="The specific fiscal year.  Reports do not go beyond 2008.",
     )
 
-    @field_validator("period", mode="after", check_fields=False)
-    @classmethod
-    def validate_period(cls, v):
-        """Validate period."""
-        v = "FY" if v == "annual" else "QTR"
-        return v
-
     @field_validator("symbol", mode="after", check_fields=False)
     @classmethod
     def handle_symbol(cls, v) -> str:
         """Handle symbols with a dash and replace it with a dot for Intrinio."""
         return v.replace("-", ".")
 
 
@@ -424,31 +417,30 @@
         query: IntrinioBalanceSheetQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
         statement_code = "balance_sheet_statement"
-        period = "FY" if query.period == "annual" else "QTR"
         fundamentals_data: Dict = {}
         base_url = "https://api-v2.intrinio.com"
+        period = "FY" if query.period == "annual" else "QTR"
         fundamentals_url = (
             f"{base_url}/companies/{query.symbol}/fundamentals?"
             f"statement_code={statement_code}&type={period}"
         )
         if query.fiscal_year is not None:
             if query.fiscal_year < 2008:
                 warn("Financials data is only available from 2008 and later.")
                 query.fiscal_year = 2008
             fundamentals_url = fundamentals_url + f"&fiscal_year={query.fiscal_year}"
         fundamentals_url = fundamentals_url + f"&api_key={api_key}"
         fundamentals_data = (await get_data_one(fundamentals_url, **kwargs)).get(
             "fundamentals", []
         )
-
         fiscal_periods = [
             f"{item['fiscal_year']}-{item['fiscal_period']}"
             for item in fundamentals_data
         ]
         fiscal_periods = fiscal_periods[: query.limit]
 
         async def callback(response: ClientResponse, _: Any) -> Dict:
@@ -458,16 +450,16 @@
                 "period_ending": statement_data["fundamental"]["end_date"],
                 "fiscal_year": statement_data["fundamental"]["fiscal_year"],
                 "fiscal_period": statement_data["fundamental"]["fiscal_period"],
                 "financials": statement_data["standardized_financials"],
             }
 
         urls = [
-            f"{base_url}/fundamentals/{query.symbol}-{statement_code}-{period}/standardized_financials?api_key={api_key}"
-            for period in fiscal_periods
+            f"{base_url}/fundamentals/{query.symbol}-{statement_code}-{p}/standardized_financials?api_key={api_key}"
+            for p in fiscal_periods
         ]
 
         return await amake_requests(urls, callback, **kwargs)
 
     @staticmethod
     def transform_data(
         query: IntrinioBalanceSheetQueryParams, data: List[Dict], **kwargs: Any
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/calendar_ipo.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/cash_flow.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/company_filings.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/company_news.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/index_historical.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,101 @@
-"""Intrinio Company News Model."""
+"""Intrinio Index Historical Model."""
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.company_news import (
-    CompanyNewsData,
-    CompanyNewsQueryParams,
+from openbb_core.provider.standard_models.index_historical import (
+    IndexHistoricalData,
+    IndexHistoricalQueryParams,
 )
-from openbb_core.provider.utils.helpers import (
-    ClientResponse,
-    amake_requests,
-    filter_by_dates,
-    get_querystring,
-)
-from pydantic import Field, field_validator
+from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_requests, get_querystring
+from pydantic import Field
 
 
-class IntrinioCompanyNewsQueryParams(CompanyNewsQueryParams):
-    """Intrinio Company News Query.
+class IntrinioIndexHistoricalQueryParams(IndexHistoricalQueryParams):
+    """Intrinio Index Historical Query.
 
-    Source: https://docs.intrinio.com/documentation/web_api/get_company_news_v2
+    Source:
+    https://docs.intrinio.com/documentation/web_api/get_stock_market_index_historical_data_v2
     """
 
-    __alias_dict__ = {"symbol": "symbols", "limit": "page_size"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
-
+    __alias_dict__ = {"limit": "page_size", "sort": "sort_order"}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
-class IntrinioCompanyNewsData(CompanyNewsData):
-    """Intrinio Company News Data."""
+    limit: Optional[int] = Field(
+        default=10000,
+        description=QUERY_DESCRIPTIONS.get("limit", ""),
+    )
 
-    __alias_dict__ = {
-        "symbols": "symbol",
-        "date": "publication_date",
-        "text": "summary",
-    }
 
-    id: str = Field(description="Article ID.")
+class IntrinioIndexHistoricalData(IndexHistoricalData):
+    """Intrinio Index Historical Data."""
 
-    @field_validator("publication_date", mode="before", check_fields=False)
-    def date_validate(cls, v):  # pylint: disable=E0213
-        """Return the date as a datetime object."""
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.000Z")
+    __alias_dict__ = {"close": "value"}
 
 
-class IntrinioCompanyNewsFetcher(
+class IntrinioIndexHistoricalFetcher(
     Fetcher[
-        IntrinioCompanyNewsQueryParams,
-        List[IntrinioCompanyNewsData],
+        IntrinioIndexHistoricalQueryParams,
+        List[IntrinioIndexHistoricalData],
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> IntrinioCompanyNewsQueryParams:
+    def transform_query(params: Dict[str, Any]) -> IntrinioIndexHistoricalQueryParams:
         """Transform the query params."""
-        return IntrinioCompanyNewsQueryParams(**params)
+        transformed_params = params
+
+        now = datetime.now().date()
+        if params.get("start_date") is None:
+            transformed_params["start_date"] = now - relativedelta(years=1)
+
+        if params.get("end_date") is None:
+            transformed_params["end_date"] = now
+
+        return IntrinioIndexHistoricalQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioCompanyNewsQueryParams,
+        query: IntrinioIndexHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
+        results = []
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-
-        base_url = "https://api-v2.intrinio.com/companies"
-        query_str = get_querystring(
-            query.model_dump(by_alias=True), ["symbols", "page"]
-        )
-
-        async def callback(response: ClientResponse, _: Any) -> List[Dict]:
-            """Return the response."""
-            if response.status != 200:
-                return []
-
-            symbol = response.url.parts[-2]
-            data = await response.json()
-
-            if isinstance(data, dict):
-                return [{**d, "symbol": symbol} for d in data.get("news", [])]
-            return []
-
+        symbols = query.symbol.replace("$", "").replace("^", "").split(",")
+        base_url = "https://api-v2.intrinio.com/indices/stock_market"
+        query_str = get_querystring(query.model_dump(by_alias=True), ["symbol"])
         urls = [
-            f"{base_url}/{symbol}/news?{query_str}&api_key={api_key}"
-            for symbol in [s.strip() for s in getattr(query, "symbol", "").split(",")]
+            f"{base_url}/${symbol}/historical_data/level?{query_str}&api_key={api_key}"
+            for symbol in symbols
         ]
 
-        return await amake_requests(urls, callback, **kwargs)
+        async def callback(response, _) -> List[Dict]:
+            """Response callback."""
+            _response = await response.json()
+            data = _response.get("historical_data")
+            symbol = _response["index"].get("symbol").replace("$", "")
+            data = [d for d in data if d.get("value") is not None]
+            data = [{"symbol": symbol, **d} for d in data] if len(symbols) > 1 else data
+            return results.extend(data) if len(data) > 0 else results  # type: ignore
+
+        await amake_requests(urls, callback, **kwargs)
+
+        if len(results) == 0:
+            raise EmptyDataError()
+        return results
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
-        query: IntrinioCompanyNewsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[IntrinioCompanyNewsData]:
+        query: IntrinioIndexHistoricalQueryParams,  # pylint: disable=unused-argument
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[IntrinioIndexHistoricalData]:
         """Return the transformed data."""
-        modeled_data = [IntrinioCompanyNewsData.model_validate(d) for d in data]
-        return filter_by_dates(modeled_data, query.start_date, query.end_date)
+        return [IntrinioIndexHistoricalData.model_validate(d) for d in data]
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/currency_pairs.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/financial_attributes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,78 @@
-"""Intrinio Currency Available Pairs Model."""
+"""Intrinio Financial Attributes Model."""
 
+from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.currency_pairs import (
-    CurrencyPairsData,
-    CurrencyPairsQueryParams,
+from openbb_core.provider.standard_models.financial_attributes import (
+    FinancialAttributesData,
+    FinancialAttributesQueryParams,
 )
+from openbb_core.provider.utils.helpers import get_querystring
 from openbb_intrinio.utils.helpers import get_data_many
-from pydantic import Field
 
 
-class IntrinioCurrencyPairsQueryParams(CurrencyPairsQueryParams):
-    """Intrinio Currency Available Pairs Query.
+class IntrinioFinancialAttributesQueryParams(FinancialAttributesQueryParams):
+    """Intrinio Financial Attributes Query."""
 
-    Source: https://docs.intrinio.com/documentation/web_api/get_forex_pairs_v2
-    """
+    __alias_dict__ = {"sort": "sort_order", "limit": "page_size"}
 
 
-class IntrinioCurrencyPairsData(CurrencyPairsData):
-    """Intrinio Currency Available Pairs Data."""
+class IntrinioFinancialAttributesData(FinancialAttributesData):
+    """Intrinio Financial Attributes Data."""
 
-    __alias_dict__ = {"name": "code"}
 
-    code: str = Field(description="Code of the currency pair.", alias="name")
-    base_currency: str = Field(
-        description="ISO 4217 currency code of the base currency."
-    )
-    quote_currency: str = Field(
-        description="ISO 4217 currency code of the quote currency."
-    )
-
-
-class IntrinioCurrencyPairsFetcher(
+class IntrinioFinancialAttributesFetcher(
     Fetcher[
-        IntrinioCurrencyPairsQueryParams,
-        List[IntrinioCurrencyPairsData],
+        IntrinioFinancialAttributesQueryParams,
+        List[IntrinioFinancialAttributesData],
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> IntrinioCurrencyPairsQueryParams:
+    def transform_query(
+        params: Dict[str, Any]
+    ) -> IntrinioFinancialAttributesQueryParams:
         """Transform the query params."""
-        return IntrinioCurrencyPairsQueryParams(**params)
+        transformed_params = params
+
+        now = datetime.now().date()
+        if params.get("start_date") is None:
+            transformed_params["start_date"] = now - relativedelta(years=5)
+
+        if params.get("end_date") is None:
+            transformed_params["end_date"] = now
+
+        return IntrinioFinancialAttributesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioCurrencyPairsQueryParams,
+        query: IntrinioFinancialAttributesQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
+        frequency = "yearly" if query.period == "annual" else "quarterly"
+        data: List[Dict] = []
 
         base_url = "https://api-v2.intrinio.com"
-        url = f"{base_url}/forex/pairs?api_key={api_key}"
+        query_str = get_querystring(query.model_dump(by_alias=True), ["frequency"])
+        query_str = f"{query_str}&frequency={frequency}"
+
+        url = f"{base_url}/historical_data/{query.symbol}/{query.tag}?{query_str}&api_key={api_key}"
+        # data = get_data_one(url).get("historical_data", [])
+        data = await get_data_many(url, "historical_data")
 
-        return await get_data_many(url, "pairs", **kwargs)
+        return data
 
     @staticmethod
     def transform_data(
-        query: IntrinioCurrencyPairsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[IntrinioCurrencyPairsData]:
+        query: IntrinioFinancialAttributesQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[IntrinioFinancialAttributesData]:
         """Return the transformed data."""
-        return [IntrinioCurrencyPairsData.model_validate(d) for d in data]
+        return [IntrinioFinancialAttributesData.model_validate(item) for item in data]
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_historical.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_historical.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     EquityHistoricalData,
     EquityHistoricalQueryParams,
 )
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import (
     ClientResponse,
     ClientSession,
-    amake_requests,
+    amake_request,
     get_querystring,
 )
 from pydantic import Field, PrivateAttr, model_validator
 
 
 class IntrinioEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Intrinio Equity Historical Price Query.
@@ -68,17 +69,17 @@
             "1W": "weekly",
             "1M": "monthly",
             "1Q": "quarterly",
             "1Y": "yearly",
         }
 
         if values.interval in ["1m", "5m", "10m", "15m", "30m", "60m", "1h"]:
-            values._interval_size = values.interval
+            values._interval_size = values.interval  # type: ignore
         elif values.interval in ["1d", "1W", "1M", "1Q", "1Y"]:
-            values._frequency = frequency_dict[values.interval]
+            values._frequency = frequency_dict[values.interval]  # type: ignore
 
         return values
 
 
 class IntrinioEquityHistoricalData(EquityHistoricalData):
     """Intrinio Equity Historical Price Data."""
 
@@ -92,15 +93,15 @@
         default=None,
         description="Change in the price of the symbol from the previous day.",
     )
     change_percent: Optional[float] = Field(
         default=None,
         description="Percent change in the price of the symbol from the previous day.",
         alias="percent_change",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     adj_open: Optional[float] = Field(
         default=None,
         description="The adjusted open price.",
     )
     adj_high: Optional[float] = Field(
         default=None,
@@ -191,15 +192,14 @@
     async def aextract_data(
         query: IntrinioEquityHistoricalQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-
         base_url = f"https://api-v2.intrinio.com/securities/{query.symbol}/prices"
         query_str = get_querystring(
             query.model_dump(by_alias=True), ["symbol", "interval"]
         )
 
         if query._interval_size:
             base_url += f"/intervals?interval_size={query._interval_size}"
@@ -207,38 +207,44 @@
         elif query._frequency:
             base_url += f"?frequency={query._frequency}"
             data_key = "stock_prices"
 
         async def callback(response: ClientResponse, session: ClientSession) -> list:
             """Return the response."""
             init_response = await response.json()
+            if "error" in init_response:
+                raise RuntimeError(
+                    f"Intrinio Error Message -> {init_response['error']}: {init_response.get('message')}"  # type: ignore
+                )
 
-            all_data: list = init_response.get(data_key, [])
+            all_data: list = init_response.get(data_key, [])  # type: ignore
 
-            next_page = init_response.get("next_page", None)
+            next_page = init_response.get("next_page", None)  # type: ignore
             while next_page:
                 url = response.url.update_query(next_page=next_page).human_repr()
                 response_data = await session.get_json(url)
 
-                all_data.extend(response_data.get(data_key, []))
-                next_page = response_data.get("next_page", None)
+                all_data.extend(response_data.get(data_key, []))  # type: ignore
+                next_page = response_data.get("next_page", None)  # type: ignore
 
             return all_data
 
         url = f"{base_url}&{query_str}&api_key={api_key}"
 
-        return await amake_requests([url], callback, **kwargs)
+        return await amake_request(url, response_callback=callback, **kwargs)  # type: ignore
 
     @staticmethod
     def transform_data(
         query: IntrinioEquityHistoricalQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[IntrinioEquityHistoricalData]:
         """Return the transformed data."""
+        if not data:
+            raise EmptyDataError("The request was returned empty.")
         date_col = (
             "time"
             if query.interval in ["1m", "5m", "10m", "15m", "30m", "60m", "1h"]
             else "date"
         )
         return [
             IntrinioEquityHistoricalData.model_validate(d)
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_info.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class IntrinioEquityInfoQueryParams(EquityInfoQueryParams):
     """Intrinio Equity Info Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_company_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioEquityInfoData(EquityInfoData):
     """Intrinio Equity Info Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_quote.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Intrinio Equity Quote Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_security_realtime_price_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     symbol: str = Field(
         description="A Security identifier (Ticker, FIGI, ISIN, CUSIP, Intrinio ID)."
     )
     source: SOURCES = Field(default="iex", description="Source of the data.")
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/equity_search.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_holdings.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
         symbol = query.symbol + ":US" if ":" not in query.symbol else query.symbol
         URL = f"https://api-v2.intrinio.com/etfs/{symbol}/holdings?page_size=10000&api_key={api_key}"
         if query.date:
             URL += f"&as_of_date={query.date}"
-        data = []
+        data: List = []
 
         async def response_callback(response: ClientResponse, session: ClientSession):
             """Async response callback."""
             results = await response.json()
 
             if results.get("error"):  # type: ignore
                 return results
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_info.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class IntrinioEtfInfoQueryParams(EtfInfoQueryParams):
     """
     Intrinio ETF Info Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioEtfInfoData(EtfInfoData):
     """Intrinio ETF Info Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_price_performance.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_price_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     Intrinio ETF Performance Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_stats_v2
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_analytics_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     return_type: Literal["trailing", "calendar"] = Field(
         default="trailing",
         description="The type of returns to return, a trailing or calendar window.",
     )
     adjustment: Literal["splits_only", "splits_and_dividends"] = Field(
         default="splits_and_dividends",
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/etf_search.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/financial_attributes.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/search_attributes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,73 @@
-"""Intrinio Financial Attributes Model."""
+"""Intrinio Search Attributes Model."""
 
-from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.financial_attributes import (
-    FinancialAttributesData,
-    FinancialAttributesQueryParams,
+from openbb_core.provider.standard_models.search_attributes import (
+    SearchAttributesData,
+    SearchAttributesQueryParams,
 )
 from openbb_core.provider.utils.helpers import get_querystring
-from openbb_intrinio.utils.helpers import get_data_many
+from openbb_intrinio.utils.helpers import get_data_one
 
 
-class IntrinioFinancialAttributesQueryParams(FinancialAttributesQueryParams):
-    """Intrinio Financial Attributes Query."""
+class IntrinioSearchAttributesQueryParams(SearchAttributesQueryParams):
+    """Intrinio Search Attributes Query.
 
-    __alias_dict__ = {"sort": "sort_order", "limit": "page_size"}
+    Source: https://docs.intrinio.com/documentation/web_api/search_data_tags_v2
+    """
 
+    __alias_dict__ = {"limit": "page_size"}
 
-class IntrinioFinancialAttributesData(FinancialAttributesData):
-    """Intrinio Financial Attributes Data."""
 
+class IntrinioSearchAttributesData(SearchAttributesData):
+    """Intrinio Search Attributes Data."""
 
-class IntrinioFinancialAttributesFetcher(
+    __alias_dict__ = {
+        "parent_name": "parent",
+        "transaction": "balance",
+    }
+
+
+class IntrinioSearchAttributesFetcher(
     Fetcher[
-        IntrinioFinancialAttributesQueryParams,
-        List[IntrinioFinancialAttributesData],
+        IntrinioSearchAttributesQueryParams,
+        List[IntrinioSearchAttributesData],
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(
-        params: Dict[str, Any]
-    ) -> IntrinioFinancialAttributesQueryParams:
+    def transform_query(params: Dict[str, Any]) -> IntrinioSearchAttributesQueryParams:
         """Transform the query params."""
-        transformed_params = params
-
-        now = datetime.now().date()
-        if params.get("start_date") is None:
-            transformed_params["start_date"] = now - relativedelta(years=5)
-
-        if params.get("end_date") is None:
-            transformed_params["end_date"] = now
-
-        return IntrinioFinancialAttributesQueryParams(**transformed_params)
+        return IntrinioSearchAttributesQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioFinancialAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioSearchAttributesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-        frequency = "yearly" if query.period == "annual" else "quarterly"
-        data: List[Dict] = []
 
         base_url = "https://api-v2.intrinio.com"
-        query_str = get_querystring(query.model_dump(by_alias=True), ["frequency"])
-        query_str = f"{query_str}&frequency={frequency}"
+        query_str = get_querystring(query.model_dump(by_alias=True), [])
+
+        url = f"{base_url}/data_tags/search?{query_str}&api_key={api_key}"
+        data = await get_data_one(url, **kwargs)
 
-        url = f"{base_url}/historical_data/{query.symbol}/{query.tag}?{query_str}&api_key={api_key}"
-        # data = get_data_one(url).get("historical_data", [])
-        data = await get_data_many(url, "historical_data")
+        # Intrinio doesn't return the correct number of results when using the limit parameter
+        # Temporary fix until they fix it
+        data = data.get("tags", [])[: query.limit]
 
         return data
 
     @staticmethod
     def transform_data(
-        query: IntrinioFinancialAttributesQueryParams,
+        query: IntrinioSearchAttributesQueryParams,
         data: List[Dict],
         **kwargs: Any,
-    ) -> List[IntrinioFinancialAttributesData]:
+    ) -> List[IntrinioSearchAttributesData]:
         """Return the transformed data."""
-        return [IntrinioFinancialAttributesData.model_validate(item) for item in data]
+        return [IntrinioSearchAttributesData.model_validate(item) for item in data]
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/financial_ratios.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioForwardEpsEstimatesQueryParams(ForwardEpsEstimatesQueryParams):
     """Intrinio Forward EPS Estimates Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales_estimates_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     fiscal_year: Optional[int] = Field(
         default=None,
         description="The future fiscal year to retrieve estimates for."
         + " When no symbol and year is supplied the current calendar year is used.",
     )
     fiscal_period: Union[Literal["fy", "q1", "q2", "q3", "q4"], None] = Field(
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioForwardSalesEstimatesQueryParams(ForwardSalesEstimatesQueryParams):
     """Intrinio Forward Sales Estimates Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales_estimates_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     fiscal_year: Optional[int] = Field(
         default=None,
         description="The future fiscal year to retrieve estimates for."
         + " When no symbol and year is supplied the current calendar year is used.",
     )
     fiscal_period: Union[Literal["fy", "q1", "q2", "q3", "q4"], None] = Field(
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/fred_series.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/historical_attributes.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/historical_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     """Intrinio Historical Attributes Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_historical_data_v2
     """
 
     __alias_dict__ = {"sort": "sort_order", "limit": "page_size", "tag_type": "type"}
     __json_schema_extra__ = {
-        "tag": ["multiple_items_allowed"],
-        "symbol": ["multiple_items_allowed"],
+        "tag": {"multiple_items_allowed": True},
+        "symbol": {"multiple_items_allowed": True},
     }
 
 
 class IntrinioHistoricalAttributesData(HistoricalAttributesData):
     """Intrinio Historical Attributes Data."""
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/historical_dividends.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/income_statement.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/insider_trading.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/institutional_ownership.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/key_metrics.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/key_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class IntrinioKeyMetricsQueryParams(KeyMetricsQueryParams):
     """
     Intrinio Key Metrics Query.
 
     Source: https://data.intrinio.com/data-tags/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioKeyMetricsData(KeyMetricsData):
     """Intrinio Key Metrics Data."""
 
     __alias_dict__ = {
         "market_cap": "marketcap",
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/latest_attributes.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/latest_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     """Intrinio Latest Attributes Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_data_point_number_v2
             https://docs.intrinio.com/documentation/web_api/get_data_point_text_v2
     """
 
     __json_schema_extra__ = {
-        "tag": ["multiple_items_allowed"],
-        "symbol": ["multiple_items_allowed"],
+        "tag": {"multiple_items_allowed": True},
+        "symbol": {"multiple_items_allowed": True},
     }
 
 
 class IntrinioLatestAttributesData(LatestAttributesData):
     """Intrinio Latest Attributes Data."""
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/market_indices.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/market_snapshots.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/options_chains.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/options_unusual.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/price_target_consensus.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """Intrinio Price Target Consensus  Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales__v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     industry_group_number: Optional[int] = Field(
         default=None,
         description="The Zacks industry group number.",
     )
```

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/reported_financials.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/models/share_statistics.py` & `openbb_intrinio-1.2.0/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/utils/helpers.py` & `openbb_intrinio-1.2.0/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/openbb_intrinio/utils/references.py` & `openbb_intrinio-1.2.0/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.1.5/PKG-INFO` & `openbb_intrinio-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-intrinio
-Version: 1.1.5
+Version: 1.2.0
 Summary: Intrinio extension for OpenBB
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Intrinio Provider
 
 This extension integrates the [Intrinio](https://intrinio.com/) data provider into the OpenBB Platform.
 
@@ -23,11 +25,9 @@
 
 To install the extension:
 
 ```bash
 pip install openbb-intrinio
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

