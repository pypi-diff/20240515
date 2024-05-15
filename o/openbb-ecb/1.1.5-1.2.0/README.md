# Comparing `tmp/openbb_ecb-1.1.5.tar.gz` & `tmp/openbb_ecb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_ecb-1.1.5.tar", max compression
+gzip compressed data, was "openbb_ecb-1.2.0.tar", max compression
```

## Comparing `openbb_ecb-1.1.5.tar` & `openbb_ecb-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      426 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/README.md
--rw-r--r--   0        0        0      895 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-19 13:10:31.744034 openbb_ecb-1.1.5/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-17 12:33:20.561645 openbb_ecb-1.1.5/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      455 2024-04-19 16:42:36.987430 openbb_ecb-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 openbb_ecb-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      299 2024-05-15 14:26:04.197157 openbb_ecb-1.2.0/README.md
+-rw-r--r--   0        0        0      931 2024-05-14 15:30:05.611286 openbb_ecb-1.2.0/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-23 10:22:39.656547 openbb_ecb-1.2.0/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-03-21 17:38:35.638719 openbb_ecb-1.2.0/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-02-29 11:03:36.767005 openbb_ecb-1.2.0/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-04-08 12:02:16.587780 openbb_ecb-1.2.0/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-04-23 10:22:39.656649 openbb_ecb-1.2.0/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-02-29 11:03:36.767215 openbb_ecb-1.2.0/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-02-29 11:03:36.767284 openbb_ecb-1.2.0/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-04-08 12:02:16.587857 openbb_ecb-1.2.0/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      481 2024-05-15 16:07:27.469945 openbb_ecb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 openbb_ecb-1.2.0/PKG-INFO
```

### Comparing `openbb_ecb-1.1.5/openbb_ecb/__init__.py` & `openbb_ecb-1.2.0/openbb_ecb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from openbb_core.provider.abstract.provider import Provider
 from openbb_ecb.models.balance_of_payments import ECBBalanceOfPaymentsFetcher
 from openbb_ecb.models.currency_reference_rates import ECBCurrencyReferenceRatesFetcher
 from openbb_ecb.models.eu_yield_curve import ECBEUYieldCurveFetcher
 
 ecb_provider = Provider(
     name="ECB",
-    website="https://data.ecb.europa.eu/",
+    website="https://data.ecb.europa.eu",
     description="""The ECB Data Portal provides access to all official ECB statistics.
-    The portal also provides options to download data and comprehensive metadata for each dataset.
-    Statistical publications and dashboards offer a compilation of key data on selected topics.""",
+The portal also provides options to download data and comprehensive metadata for each dataset.
+Statistical publications and dashboards offer a compilation of key data on selected topics.""",
     fetcher_dict={
         "BalanceOfPayments": ECBBalanceOfPaymentsFetcher,
         "CurrencyReferenceRates": ECBCurrencyReferenceRatesFetcher,
         "EUYieldCurve": ECBEUYieldCurveFetcher,
     },
+    repr_name="European Central Bank (ECB)",
 )
```

### Comparing `openbb_ecb-1.1.5/openbb_ecb/models/balance_of_payments.py` & `openbb_ecb-1.2.0/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.5/openbb_ecb/models/currency_reference_rates.py` & `openbb_ecb-1.2.0/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.5/openbb_ecb/models/eu_yield_curve.py` & `openbb_ecb-1.2.0/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.5/openbb_ecb/utils/bps_series.py` & `openbb_ecb-1.2.0/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.5/openbb_ecb/utils/ecb_helpers.py` & `openbb_ecb-1.2.0/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.1.5/openbb_ecb/utils/yield_curve_series.py` & `openbb_ecb-1.2.0/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

