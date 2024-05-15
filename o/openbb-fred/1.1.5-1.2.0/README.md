# Comparing `tmp/openbb_fred-1.1.5.tar.gz` & `tmp/openbb_fred-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fred-1.1.5.tar", max compression
+gzip compressed data, was "openbb_fred-1.2.0.tar", max compression
```

## Comparing `openbb_fred-1.1.5.tar` & `openbb_fred-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      444 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/README.md
--rw-r--r--   0        0        0     3126 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-19 13:10:31.748034 openbb_fred-1.1.5/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-04-19 13:10:31.748034 openbb_fred-1.1.5/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-04-17 12:33:20.665645 openbb_fred-1.1.5/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-04-17 12:33:20.669645 openbb_fred-1.1.5/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      439 2024-04-19 16:41:03.859203 openbb_fred-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_fred-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      317 2024-05-15 14:25:37.598005 openbb_fred-1.2.0/README.md
+-rw-r--r--   0        0        0     4116 2024-05-14 15:30:05.615680 openbb_fred-1.2.0/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-02-29 11:03:36.866196 openbb_fred-1.2.0/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-02-29 11:03:36.866284 openbb_fred-1.2.0/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2953 2024-05-10 10:40:27.296801 openbb_fred-1.2.0/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-04-08 12:02:16.648313 openbb_fred-1.2.0/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-02-29 11:03:36.866494 openbb_fred-1.2.0/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-02-29 11:03:36.866551 openbb_fred-1.2.0/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-02-29 11:03:36.866626 openbb_fred-1.2.0/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-02-29 11:03:36.866706 openbb_fred-1.2.0/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-02-29 11:03:36.866781 openbb_fred-1.2.0/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-04-08 12:02:16.648416 openbb_fred-1.2.0/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-02-29 11:03:36.866951 openbb_fred-1.2.0/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-02-29 11:03:36.867021 openbb_fred-1.2.0/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-02-29 11:03:36.867092 openbb_fred-1.2.0/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-04-08 12:02:16.648506 openbb_fred-1.2.0/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6344 2024-05-09 13:34:29.220357 openbb_fred-1.2.0/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6726 2024-05-10 10:40:27.296996 openbb_fred-1.2.0/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-02-29 11:03:36.867365 openbb_fred-1.2.0/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-02-29 11:03:36.867442 openbb_fred-1.2.0/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2732 2024-05-10 10:40:27.297174 openbb_fred-1.2.0/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-02-29 11:03:36.867578 openbb_fred-1.2.0/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-02-29 11:03:36.867653 openbb_fred-1.2.0/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-02-29 11:03:36.867734 openbb_fred-1.2.0/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-02-29 11:03:36.867879 openbb_fred-1.2.0/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-02-29 11:03:36.868080 openbb_fred-1.2.0/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-02-29 11:03:36.868229 openbb_fred-1.2.0/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-04-08 12:02:16.648982 openbb_fred-1.2.0/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-04-08 12:02:16.649089 openbb_fred-1.2.0/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-02-29 11:03:36.868524 openbb_fred-1.2.0/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-02-29 11:03:36.868834 openbb_fred-1.2.0/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      465 2024-05-15 16:05:55.488948 openbb_fred-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 openbb_fred-1.2.0/PKG-INFO
```

### Comparing `openbb_fred-1.1.5/openbb_fred/__init__.py` & `openbb_fred-1.2.0/openbb_fred/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 from openbb_fred.models.spot import FREDSpotRateFetcher
 from openbb_fred.models.tbffr import FREDSelectedTreasuryBillFetcher
 from openbb_fred.models.tmc import FREDTreasuryConstantMaturityFetcher
 from openbb_fred.models.us_yield_curve import FREDYieldCurveFetcher
 
 fred_provider = Provider(
     name="fred",
-    website="https://fred.stlouisfed.org/",
+    website="https://fred.stlouisfed.org",
     description="""Federal Reserve Economic Data is a database maintained by the
-     Research division of the Federal Reserve Bank of St. Louis that has more than
-     816,000 economic time series from various sources.""",
+Research division of the Federal Reserve Bank of St. Louis that has more than
+816,000 economic time series from various sources.""",
     credentials=["api_key"],
     fetcher_dict={
         "ConsumerPriceIndex": FREDConsumerPriceIndexFetcher,
         "USYieldCurve": FREDYieldCurveFetcher,
         "SOFR": FREDSOFRFetcher,
         "ESTR": FREDESTRFetcher,
         "SONIA": FREDSONIAFetcher,
@@ -55,8 +55,11 @@
         "FredRegional": FredRegionalDataFetcher,
         "SpotRate": FREDSpotRateFetcher,
         "HighQualityMarketCorporateBond": FREDHighQualityMarketCorporateBondFetcher,
         "TreasuryConstantMaturity": FREDTreasuryConstantMaturityFetcher,
         "SelectedTreasuryConstantMaturity": FREDSelectedTreasuryConstantMaturityFetcher,
         "SelectedTreasuryBill": FREDSelectedTreasuryBillFetcher,
     },
+    repr_name="Federal Reserve Economic Data | St. Louis FED (FRED)",
+    v3_credentials=["API_FRED_KEY"],
+    instructions='Go to: https://fred.stlouisfed.org\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827137-d143ba4c-72cb-467d-a7f4-5cc27c597aec.png)\n\nClick on, "My Account", create a new account or sign in with Google:\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827011-65cdd501-27e3-436f-bd9d-b0d8381d46a7.png)\n\nAfter completing the sign-up, go to "My Account", and select "API Keys". Then, click on, "Request API Key".\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827577-c869f989-4ef4-4949-ab57-6f3931f2ae9d.png)\n\nFill in the box for information about the use-case for FRED, and by clicking, "Request API key", at the bottom of the page, the API key will be issued.\n\n![FRED](https://user-images.githubusercontent.com/46355364/207828032-0a32d3b8-1378-4db2-9064-aa1eb2111632.png)',  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_fred-1.1.5/openbb_fred/models/ameribor_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/cp.py` & `openbb_fred-1.2.0/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/cpi.py` & `openbb_fred-1.2.0/openbb_fred/models/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from openbb_fred.utils.fred_base import Fred
 from openbb_fred.utils.fred_helpers import all_cpi_options
 
 
 class FREDConsumerPriceIndexQueryParams(ConsumerPriceIndexQueryParams):
     """FRED Consumer Price Index Query."""
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
 
 class FREDConsumerPriceIndexData(ConsumerPriceIndexData):
     """FRED Consumer Price Index Data."""
 
 
 class FREDConsumerPriceIndexFetcher(
@@ -71,12 +71,11 @@
                 # If the date is not in the dictionary, add it
                 if item["date"] not in transformed_data:
                     transformed_data[item["date"]] = {"date": item["date"]}
                 # Update the dictionary with the country's value data
                 transformed_data[item["date"]].update({country: item["value"]})
 
         # Convert the dictionary to a list of dictionaries
-        transformed_data = list(transformed_data.values())
-
         return [
-            FREDConsumerPriceIndexData.model_validate(item) for item in transformed_data
+            FREDConsumerPriceIndexData.model_validate(item)
+            for item in list(transformed_data.values())
         ]
```

### Comparing `openbb_fred-1.1.5/openbb_fred/models/dwpcr_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/ecb_interest_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/estr_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/fed_projections.py` & `openbb_fred-1.2.0/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/fed_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/ffrmc.py` & `openbb_fred-1.2.0/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/hqm.py` & `openbb_fred-1.2.0/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/ice_bofa.py` & `openbb_fred-1.2.0/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/iorb_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/moody.py` & `openbb_fred-1.2.0/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/regional.py` & `openbb_fred-1.2.0/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/search.py` & `openbb_fred-1.2.0/openbb_fred/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         default=None,
         description=QUERY_DESCRIPTIONS.get("limit", "") + " (1-1000)",
     )
     offset: Optional[NonNegativeInt] = Field(
         default=0,
         description="Offset the results in conjunction with limit.",
     )
-    filter_variable: Literal[None, "frequency", "units", "seasonal_adjustment"] = Field(
-        default=None, description="Filter by an attribute."
+    filter_variable: Optional[Literal["frequency", "units", "seasonal_adjustment"]] = (
+        Field(default=None, description="Filter by an attribute.")
     )
     filter_value: Optional[str] = Field(
         default=None,
         description="String value to filter the variable by.  Used in conjunction with filter_variable.",
     )
     tag_names: Optional[str] = Field(
         default=None,
```

### Comparing `openbb_fred-1.1.5/openbb_fred/models/series.py` & `openbb_fred-1.2.0/openbb_fred/models/series.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,32 +24,33 @@
 
     __alias_dict__ = {
         "symbol": "series_id",
         "start_date": "observation_start",
         "end_date": "observation_end",
         "transform": "units",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
-    frequency: Literal[
-        None,
-        "a",
-        "q",
-        "m",
-        "w",
-        "d",
-        "wef",
-        "weth",
-        "wew",
-        "wetu",
-        "wem",
-        "wesu",
-        "wesa",
-        "bwew",
-        "bwem",
+    frequency: Optional[
+        Literal[
+            "a",
+            "q",
+            "m",
+            "w",
+            "d",
+            "wef",
+            "weth",
+            "wew",
+            "wetu",
+            "wem",
+            "wesu",
+            "wesa",
+            "bwew",
+            "bwem",
+        ]
     ] = Field(
         default=None,
         description="""
         Frequency aggregation to convert high frequency data to lower frequency.
             None = No change
             a = Annual
             q = Quarterly
@@ -63,40 +64,40 @@
             wem = Weekly, Ending Monday
             wesu = Weekly, Ending Sunday
             wesa = Weekly, Ending Saturday
             bwew = Biweekly, Ending Wednesday
             bwem = Biweekly, Ending Monday
         """,
     )
-    aggregation_method: Literal[None, "avg", "sum", "eop"] = Field(
+    aggregation_method: Optional[Literal["avg", "sum", "eop"]] = Field(
         default="eop",
         description="""
         A key that indicates the aggregation method used for frequency aggregation.
         This parameter has no affect if the frequency parameter is not set.
             avg = Average
             sum = Sum
             eop = End of Period
         """,
     )
-    transform: Literal[None, "chg", "ch1", "pch", "pc1", "pca", "cch", "cca", "log"] = (
-        Field(
-            default=None,
-            description="""
+    transform: Optional[
+        Literal["chg", "ch1", "pch", "pc1", "pca", "cch", "cca", "log"]
+    ] = Field(
+        default=None,
+        description="""
         Transformation type
             None = No transformation
             chg = Change
             ch1 = Change from Year Ago
             pch = Percent Change
             pc1 = Percent Change from Year Ago
             pca = Compounded Annual Rate of Change
             cch = Continuously Compounded Rate of Change
             cca = Continuously Compounded Annual Rate of Change
             log = Natural Log
         """,
-        )
     )
     limit: int = Field(description=QUERY_DESCRIPTIONS.get("limit", ""), default=100000)
 
 
 class FredSeriesData(SeriesData):
     """FRED Series Data."""
```

### Comparing `openbb_fred-1.1.5/openbb_fred/models/sofr_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/sonia_rates.py` & `openbb_fred-1.2.0/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/spot.py` & `openbb_fred-1.2.0/openbb_fred/models/spot.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pydantic import field_validator
 
 
 class FREDSpotRateQueryParams(SpotRateQueryParams):
     """FRED Spot Rate Query."""
 
     __json_schema_extra__ = {
-        "maturity": ["multiple_items_allowed"],
-        "category": ["multiple_items_allowed"],
+        "maturity": {"multiple_items_allowed": True},
+        "category": {"multiple_items_allowed": True},
     }
 
 
 class FREDSpotRateData(SpotRateData):
     """FRED Spot Rate Data."""
 
     __alias_dict__ = {"rate": "value"}
```

### Comparing `openbb_fred-1.1.5/openbb_fred/models/tbffr.py` & `openbb_fred-1.2.0/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/tmc.py` & `openbb_fred-1.2.0/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/models/us_yield_curve.py` & `openbb_fred-1.2.0/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/commercial_paper.csv` & `openbb_fred-1.2.0/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_fred-1.2.0/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/cpi.csv` & `openbb_fred-1.2.0/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/fred_base.py` & `openbb_fred-1.2.0/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/fred_helpers.py` & `openbb_fred-1.2.0/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/harmonized_cpi.csv` & `openbb_fred-1.2.0/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.5/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_fred-1.2.0/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

