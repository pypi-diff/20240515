# Comparing `tmp/openbb_tradier-1.0.2.tar.gz` & `tmp/openbb_tradier-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradier-1.0.2.tar", max compression
+gzip compressed data, was "openbb_tradier-1.1.0.tar", max compression
```

## Comparing `openbb_tradier-1.0.2.tar` & `openbb_tradier-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      438 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/README.md
--rw-r--r--   0        0        0     1241 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6582 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9222 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-04-19 16:31:25.550563 openbb_tradier-1.0.2/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-17 12:33:20.845646 openbb_tradier-1.0.2/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      474 2024-04-19 16:43:00.275490 openbb_tradier-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_tradier-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-05-15 14:32:56.427613 openbb_tradier-1.1.0/README.md
+-rw-r--r--   0        0        0     1740 2024-05-14 15:30:05.620279 openbb_tradier-1.1.0/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-23 10:22:39.796948 openbb_tradier-1.1.0/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6588 2024-05-10 10:40:27.303718 openbb_tradier-1.1.0/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9228 2024-05-10 10:40:27.304076 openbb_tradier-1.1.0/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-04-08 12:02:16.760537 openbb_tradier-1.1.0/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-04-23 10:22:39.797971 openbb_tradier-1.1.0/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:02:16.760617 openbb_tradier-1.1.0/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.798100 openbb_tradier-1.1.0/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-04-08 12:02:16.760718 openbb_tradier-1.1.0/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      500 2024-05-15 16:05:23.906169 openbb_tradier-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 openbb_tradier-1.1.0/PKG-INFO
```

### Comparing `openbb_tradier-1.0.2/openbb_tradier/__init__.py` & `openbb_tradier-1.1.0/openbb_tradier/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from openbb_tradier.models.equity_quote import TradierEquityQuoteFetcher
 from openbb_tradier.models.equity_search import TradierEquitySearchFetcher
 from openbb_tradier.models.options_chains import TradierOptionsChainsFetcher
 
 tradier_provider = Provider(
     name="tradier",
     website="https://tradier.com",
-    description="Tradier provides a full range of services in a scalable, secure,"
-    + " and easy-to-use REST-based API for businesses and individual developers."
-    + " Fast, secure, simple. Start in minutes."
-    + " Get access to trading, account management, and market-data for"
-    + " Tradier Brokerage accounts through our APIs.",
+    description="""Tradier provides a full range of services in a scalable, secure,
+and easy-to-use REST-based API for businesses and individual developers.
+Fast, secure, simple. Start in minutes.
+Get access to trading, account management, and market-data for
+Tradier Brokerage accounts through our APIs.""",
     credentials=[
         "api_key",
         "account_type",
     ],  # account_type is either "sandbox" or "live"
     fetcher_dict={
         "EquityHistorical": TradierEquityHistoricalFetcher,
         "EtfHistorical": TradierEquityHistoricalFetcher,
         "EquityQuote": TradierEquityQuoteFetcher,
         "EquitySearch": TradierEquitySearchFetcher,
         "OptionsChains": TradierOptionsChainsFetcher,
     },
+    repr_name="Tradier",
+    v3_credentials=["API_TRADIER_TOKEN"],
+    instructions='Go to: https://documentation.tradier.com\n\n![Tradier](https://user-images.githubusercontent.com/46355364/207829178-a8bba770-f2ea-4480-b28e-efd81cf30980.png)\n\nClick on, "Open Account", to start the sign-up process. After the account has been setup, navigate to [Tradier Broker Dash](https://dash.tradier.com/login?redirect=settings.api) and create the application. Request a sandbox access token.',  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_tradier-1.0.2/openbb_tradier/models/equity_historical.py` & `openbb_tradier-1.1.0/openbb_tradier/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pydantic import Field
 from pytz import timezone
 
 
 class TradierEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Tradier Equity Historical Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "1d", "1W", "1M"] = Field(
         description=QUERY_DESCRIPTIONS.get("interval", ""),
         default="1d",
     )
     extended_hours: bool = Field(
         default=False,
```

### Comparing `openbb_tradier-1.0.2/openbb_tradier/models/equity_quote.py` & `openbb_tradier-1.1.0/openbb_tradier/models/equity_quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Tradier Equity Quote Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TradierEquityQuoteData(EquityQuoteData):
     """Tradier Equity Quote Data."""
 
     __alias_dict__ = {
         "name": "description",
```

### Comparing `openbb_tradier-1.0.2/openbb_tradier/models/equity_search.py` & `openbb_tradier-1.1.0/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.2/openbb_tradier/models/options_chains.py` & `openbb_tradier-1.1.0/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.2/openbb_tradier/utils/constants.py` & `openbb_tradier-1.1.0/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

