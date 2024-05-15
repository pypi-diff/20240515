# Comparing `tmp/openbb_federal_reserve-1.1.5.tar.gz` & `tmp/openbb_federal_reserve-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_federal_reserve-1.1.5.tar", max compression
+gzip compressed data, was "openbb_federal_reserve-1.2.0.tar", max compression
```

## Comparing `openbb_federal_reserve-1.1.5.tar` & `openbb_federal_reserve-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      474 2024-04-17 12:33:20.597645 openbb_federal_reserve-1.1.5/README.md
--rw-r--r--   0        0        0      716 2024-04-17 12:33:20.597645 openbb_federal_reserve-1.1.5/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-17 12:33:20.597645 openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-17 12:33:20.597645 openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-04-17 12:33:20.597645 openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      508 2024-04-19 16:41:24.695252 openbb_federal_reserve-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      347 2024-05-15 14:25:55.077678 openbb_federal_reserve-1.2.0/README.md
+-rw-r--r--   0        0        0      882 2024-05-14 15:30:05.612043 openbb_federal_reserve-1.2.0/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-04-08 12:02:16.625822 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-04-02 11:35:59.435928 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3517 2024-05-09 15:04:29.070261 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      534 2024-05-15 16:06:36.900651 openbb_federal_reserve-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.2.0/PKG-INFO
```

### Comparing `openbb_federal_reserve-1.1.5/openbb_federal_reserve/__init__.py` & `openbb_federal_reserve-1.2.0/openbb_federal_reserve/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 )
 from openbb_federal_reserve.models.treasury_rates import (
     FederalReserveTreasuryRatesFetcher,
 )
 
 federal_reserve_provider = Provider(
     name="federal_reserve",
-    website="https://www.federalreserve.gov/data.htm",
-    description=(),
+    website="https://www.federalreserve.gov/data.htm",  #  Not a typo, it's really .htm
+    description="""Access data provided by the Federal Reserve System,
+the Central Bank of the United States.""",
     fetcher_dict={
         "TreasuryRates": FederalReserveTreasuryRatesFetcher,
         "MoneyMeasures": FederalReserveMoneyMeasuresFetcher,
         "FEDFUNDS": FederalReserveFEDFetcher,
     },
+    repr_name="Federal Reserve (FED)",
 )
```

### Comparing `openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/fed_rates.py` & `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/money_measures.py` & `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.5/openbb_federal_reserve/models/treasury_rates.py` & `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/treasury_rates.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     @staticmethod
     def transform_data(
         query: FederalReserveTreasuryRatesQueryParams, data: DataFrame, **kwargs: Any
     ) -> List[FederalReserveTreasuryRatesData]:
         """Return the transformed data."""
 
-        df = data
+        df = data.copy()
         df = df[
             (to_datetime(df.date) >= to_datetime(query.start_date))  # type: ignore
             & (to_datetime(df.date) <= to_datetime(query.end_date))  # type: ignore
         ]
         for col in maturities:
             df[col] = df[col].astype(float) / 100
         df = df.fillna("N/A").replace("N/A", None)
```

### Comparing `openbb_federal_reserve-1.1.5/PKG-INFO` & `openbb_federal_reserve-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-federal-reserve
-Version: 1.1.5
+Version: 1.2.0
 Summary: US Federal Reserve Data Extension for OpenBB
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
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Federal Reserve Provider
 
 This extension integrates the [Federal Reserve](https://www.federalreserve.gov/data.htm) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-federal-reserve
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

