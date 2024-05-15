# Comparing `tmp/openbb_sec-1.1.5.tar.gz` & `tmp/openbb_sec-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_sec-1.1.5.tar", max compression
+gzip compressed data, was "openbb_sec-1.2.0.tar", max compression
```

## Comparing `openbb_sec-1.1.5.tar` & `openbb_sec-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      424 2024-04-17 12:33:20.697645 openbb_sec-1.1.5/README.md
--rw-r--r--   0        0        0     1562 2024-04-17 12:33:20.697645 openbb_sec-1.1.5/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0     8328 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     2615 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2720 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    32406 2024-04-19 13:10:31.748034 openbb_sec-1.1.5/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2754 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2079 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2790 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3009 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1714 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    13896 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7434 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.701645 openbb_sec-1.1.5/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      516 2024-04-19 16:42:10.779363 openbb_sec-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 openbb_sec-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-05-15 14:25:02.970361 openbb_sec-1.2.0/README.md
+-rw-r--r--   0        0        0     1629 2024-05-14 15:30:05.618404 openbb_sec-1.2.0/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-23 10:22:39.680890 openbb_sec-1.2.0/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-09 13:34:29.234211 openbb_sec-1.2.0/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10150 2024-05-09 13:34:29.234378 openbb_sec-1.2.0/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     3154 2024-05-09 13:34:29.234542 openbb_sec-1.2.0/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-05-09 13:34:29.234665 openbb_sec-1.2.0/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    39078 2024-05-09 13:34:29.234955 openbb_sec-1.2.0/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2820 2024-05-09 13:34:29.235121 openbb_sec-1.2.0/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-05-09 13:34:29.235238 openbb_sec-1.2.0/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-04-02 11:35:59.520014 openbb_sec-1.2.0/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2916 2024-05-09 13:34:29.235351 openbb_sec-1.2.0/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-04-08 12:02:16.675933 openbb_sec-1.2.0/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3498 2024-05-09 13:34:29.235482 openbb_sec-1.2.0/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-05-09 13:34:29.235747 openbb_sec-1.2.0/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.896831 openbb_sec-1.2.0/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-04-23 10:22:39.682644 openbb_sec-1.2.0/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-02-29 11:03:36.896953 openbb_sec-1.2.0/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    12574 2024-05-09 13:34:29.235977 openbb_sec-1.2.0/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-05-09 13:34:29.236173 openbb_sec-1.2.0/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-04-02 11:35:59.520629 openbb_sec-1.2.0/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      559 2024-05-15 16:05:42.143525 openbb_sec-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 openbb_sec-1.2.0/PKG-INFO
```

### Comparing `openbb_sec-1.1.5/openbb_sec/__init__.py` & `openbb_sec-1.2.0/openbb_sec/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from openbb_sec.models.rss_litigation import SecRssLitigationFetcher
 from openbb_sec.models.schema_files import SecSchemaFilesFetcher
 from openbb_sec.models.sic_search import SecSicSearchFetcher
 from openbb_sec.models.symbol_map import SecSymbolMapFetcher
 
 sec_provider = Provider(
     name="sec",
-    website="https://sec.gov",
+    website="https://www.sec.gov/data",
     description="SEC is the public listings regulatory body for the United States.",
     credentials=None,
     fetcher_dict={
         "CikMap": SecCikMapFetcher,
         "CompanyFilings": SecCompanyFilingsFetcher,
         "EquityFTD": SecEquityFtdFetcher,
         "EquitySearch": SecEquitySearchFetcher,
@@ -28,8 +28,9 @@
         "Form13FHR": SecForm13FHRFetcher,
         "InstitutionsSearch": SecInstitutionsSearchFetcher,
         "RssLitigation": SecRssLitigationFetcher,
         "SchemaFiles": SecSchemaFilesFetcher,
         "SicSearch": SecSicSearchFetcher,
         "SymbolMap": SecSymbolMapFetcher,
     },
+    repr_name="Securities and Exchange Commission (SEC)",
 )
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/cik_map.py` & `openbb_sec-1.2.0/openbb_sec/models/cik_map.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """SEC CIK Mapping Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cik_map import CikMapData, CikMapQueryParams
 from openbb_sec.utils.helpers import symbol_map
+from pydantic import Field
 
 
 class SecCikMapQueryParams(CikMapQueryParams):
     """SEC CIK Mapping Query.
 
     Source: https://sec.gov/
     """
 
+    use_cache: Optional[bool] = Field(
+        default=True,
+        description="Whether or not to use cache for the request, default is True.",
+    )
+
 
 class SecCikMapData(CikMapData):
     """SEC CIK Mapping Data."""
 
 
 class SecCikMapFetcher(
     Fetcher[
@@ -28,21 +36,21 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecCikMapQueryParams:
         """Transform the query."""
         return SecCikMapQueryParams(**params)
 
     @staticmethod
-    def extract_data(
-        query: SecCikMapQueryParams,  # pylint: disable=W0613:unused-argument
+    async def aextract_data(
+        query: SecCikMapQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
-        results = {"cik": symbol_map(query.symbol)}
+        results = {"cik": await symbol_map(query.symbol, query.use_cache)}
         if not results:
             return {"Error": "Symbol not found."}
         return results
 
     @staticmethod
     def transform_data(
         query: SecCikMapQueryParams, data: Dict, **kwargs: Any
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/equity_search.py` & `openbb_sec-1.2.0/openbb_sec/models/equity_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """SEC Equity Search Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_search import (
     EquitySearchData,
     EquitySearchQueryParams,
 )
@@ -26,15 +28,14 @@
         description="Whether to direct the search to the list of mutual funds and ETFs.",
     )
 
 
 class SecEquitySearchData(EquitySearchData):
     """SEC Equity Search Data."""
 
-    name: Optional[str] = Field(default=None)
     cik: str = Field(description="Central Index Key")
 
 
 class SecEquitySearchFetcher(
     Fetcher[
         SecEquitySearchQueryParams,
         List[SecEquitySearchData],
@@ -44,33 +45,33 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecEquitySearchQueryParams:
         """Transform the query."""
         return SecEquitySearchQueryParams(**params)
 
     @staticmethod
-    def extract_data(
-        query: SecEquitySearchQueryParams,  # pylint: disable=unused-argument
+    async def aextract_data(
+        query: SecEquitySearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         results = DataFrame()
 
         if query.is_fund is True:
-            companies = get_mf_and_etf_map(use_cache=query.use_cache).astype(str)
+            companies = await get_mf_and_etf_map(use_cache=query.use_cache)
             results = companies[
                 companies["cik"].str.contains(query.query, case=False)
                 | companies["seriesId"].str.contains(query.query, case=False)
                 | companies["classId"].str.contains(query.query, case=False)
                 | companies["symbol"].str.contains(query.query, case=False)
             ]
 
         if query.is_fund is False:
-            companies = get_all_companies(use_cache=query.use_cache)
+            companies = await get_all_companies(use_cache=query.use_cache)
 
             results = companies[
                 companies["name"].str.contains(query.query, case=False)
                 | companies["symbol"].str.contains(query.query, case=False)
                 | companies["cik"].str.contains(query.query, case=False)
             ]
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/etf_holdings.py` & `openbb_sec-1.2.0/openbb_sec/models/etf_holdings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """SEC ETF Holings Model."""
 
 # pylint: disable =[unused-argument,too-many-locals,too-many-branches]
 
-import warnings
+import asyncio
 from datetime import date as dateType
 from typing import Any, Dict, List, Optional, Union
+from warnings import warn
 
 import pandas as pd
-import requests
 import xmltodict
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
+from openbb_core.app.utils import get_user_cache_directory
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.etf_holdings import (
     EtfHoldingsData,
     EtfHoldingsQueryParams,
 )
 from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
-from openbb_sec.utils.helpers import HEADERS, get_nport_candidates, sec_session_etf
-from pydantic import Field, model_validator
-
-_warn = warnings.warn
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_sec.utils.helpers import HEADERS, get_nport_candidates
+from pandas.tseries.offsets import MonthEnd
+from pydantic import Field, field_validator, model_validator
 
 
 class SecEtfHoldingsQueryParams(EtfHoldingsQueryParams):
     """SEC ETF Holdings Query.
 
     Source: https://www.sec.gov/Archives/edgar/data/
     """
@@ -53,14 +58,15 @@
     balance: Optional[float] = Field(
         description="The balance of the holding.", default=None
     )
     weight: Optional[float] = Field(
         description="The weight of the holding in ETF in %.",
         alias="pctVal",
         default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     value: Optional[float] = Field(
         description="The value of the holding in USD.", alias="valUSD", default=None
     )
     payoff_profile: Optional[str] = Field(
         description="The payoff profile of the holding.",
         alias="payoffProfile",
@@ -126,15 +132,17 @@
         description="The type of coupon for the debt security.", default=None
     )
     rate_type: Optional[str] = Field(
         description="The type of rate for the debt security, floating or fixed.",
         default=None,
     )
     annualized_return: Optional[float] = Field(
-        description="The annualized return on the debt security.", default=None
+        description="The annualized return on the debt security.",
+        default=None,
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     is_default: Optional[str] = Field(
         description="If the debt security is defaulted.", default=None
     )
     in_arrears: Optional[str] = Field(
         description="If the debt security is in arrears.", default=None
     )
@@ -167,42 +175,42 @@
     shares_per_contract: Optional[float] = Field(
         description="The number of shares per contract.", default=None
     )
     delta: Optional[Union[str, float]] = Field(
         description="The delta of the option.", default=None
     )
     rate_type_rec: Optional[str] = Field(
-        description="The type of rate for reveivable portion of the swap.", default=None
+        description="The type of rate for receivable portion of the swap.", default=None
     )
     receive_currency: Optional[str] = Field(
         description="The receive currency of the swap.", default=None
     )
     upfront_receive: Optional[float] = Field(
         description="The upfront amount received of the swap.", default=None
     )
     floating_rate_index_rec: Optional[str] = Field(
-        description="The floating rate index for reveivable portion of the swap.",
+        description="The floating rate index for receivable portion of the swap.",
         default=None,
     )
     floating_rate_spread_rec: Optional[float] = Field(
         description="The floating rate spread for reveivable portion of the swap.",
         default=None,
     )
     rate_tenor_rec: Optional[str] = Field(
-        description="The rate tenor for reveivable portion of the swap.", default=None
+        description="The rate tenor for receivable portion of the swap.", default=None
     )
     rate_tenor_unit_rec: Optional[Union[str, int]] = Field(
-        description="The rate tenor unit for reveivable portion of the swap.",
+        description="The rate tenor unit for receivable portion of the swap.",
         default=None,
     )
     reset_date_rec: Optional[str] = Field(
-        description="The reset date for reveivable portion of the swap.", default=None
+        description="The reset date for receivable portion of the swap.", default=None
     )
     reset_date_unit_rec: Optional[Union[str, int]] = Field(
-        description="The reset date unit for reveivable portion of the swap.",
+        description="The reset date unit for receivable portion of the swap.",
         default=None,
     )
     rate_type_pmnt: Optional[str] = Field(
         description="The type of rate for payment portion of the swap.", default=None
     )
     payment_currency: Optional[str] = Field(
         description="The payment currency of the swap.", default=None
@@ -280,14 +288,20 @@
     notional_currency: Optional[str] = Field(
         description="The currency of the derivative's notional amount.", default=None
     )
     unrealized_gain: Optional[float] = Field(
         description="The unrealized gain or loss on the derivative.", default=None
     )
 
+    @field_validator("weight", "annualized_return", mode="before", check_fields=False)
+    @classmethod
+    def normalize_percent(cls, v):
+        """Normalize the percent values."""
+        return float(v) / 100 if v else None
+
     @model_validator(mode="before")
     @classmethod
     def replace_zero(cls, values):
         """Check for zero values and replace with None."""
         return (
             {k: None if v == 0 else v for k, v in values.items()}
             if isinstance(values, dict)
@@ -305,69 +319,94 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecEtfHoldingsQueryParams:
         """Transform the query."""
         params["symbol"] = params["symbol"].upper()
         return SecEtfHoldingsQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecEtfHoldingsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
-        filing_candidates = pd.DataFrame.from_records(
-            get_nport_candidates(symbol=query.symbol, use_cache=query.use_cache)
-        )
+        # Implement a retry mechanism in case of RemoteDiconnected Error.
+        retries = 3
+        for i in range(retries):
+            filings = []
+            try:
+                filings = await get_nport_candidates(
+                    symbol=query.symbol, use_cache=query.use_cache
+                )
+                if filings:
+                    break
+            except Exception as e:
+                if i < retries - 1:
+                    warn(f"Error: {e}. Retrying...")
+                    await asyncio.sleep(1)
+                    continue
+                raise e
+        filing_candidates = pd.DataFrame.from_records(filings)
         if filing_candidates.empty:
             raise ValueError(f"No N-Port records found for {query.symbol}.")
-        dates = filing_candidates["period_ending"].to_list()
+        dates = filing_candidates.period_ending.to_list()
         new_date: str = ""
         if query.date is not None:
             date = query.date
             # Gets the URL for the nearest date to the requested date.
             __dates = pd.Series(pd.to_datetime(dates))
             __date = pd.to_datetime(date)
             __nearest = pd.DataFrame(__dates - __date)
             __nearest_date = abs(__nearest[0].astype("int64")).idxmin()
             new_date = __dates[__nearest_date].strftime("%Y-%m-%d")
             date = new_date if new_date else date
-            _warn(f"Closest filing date to, {query.date}, is the period ending: {date}")
+            warn(f"Closest filing date to, {query.date}, is the period ending: {date}")
             filing_url = filing_candidates[filing_candidates["period_ending"] == date][
                 "primary_doc"
             ].values[0]
         else:
             filing_url = filing_candidates["primary_doc"].values[0]
-            period_ending = filing_candidates["period_ending"].values[0]
-            _warn(f"The latest filing is for the period ending: {period_ending}")
-        _warn(f"Source Document: {filing_url}")
-        r = (
-            sec_session_etf.get(filing_url, headers=HEADERS, timeout=5)
-            if query.use_cache
-            else requests.get(filing_url, headers=HEADERS, timeout=5)
-        )
-        if r.status_code != 200:
-            raise RuntimeError(f"Request failed with status code {r.status_code}")
-        response = xmltodict.parse(r.content)
 
-        return response
+        async def callback(response, session):
+            """Response callback for the request."""
+            return await response.read()
+
+        if query.use_cache is True:
+            cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
+            async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+                try:
+                    response = await amake_request(
+                        filing_url, headers=HEADERS, session=session, response_callback=callback  # type: ignore
+                    )
+                finally:
+                    await session.close()
+        else:
+            response = await amake_request(
+                filing_url, headers=HEADERS, response_callback=callback  # type: ignore
+            )
+        results = xmltodict.parse(response)
+
+        return results
 
     # pylint: disable=too-many-statements
     @staticmethod
     def transform_data(  # noqa: PLR0912
         query: SecEtfHoldingsQueryParams,
         data: Dict,
         **kwargs: Any,
-    ) -> List[SecEtfHoldingsData]:
+    ) -> AnnotatedResult[List[SecEtfHoldingsData]]:
         """Transform the data."""
+
+        if not data:
+            raise EmptyDataError(f"No data was returned for the symbol, {query.symbol}")
         results = []
 
         response = data
+
         # Parse the response if it is a NPORT-P filing.
         if (
             "edgarSubmission" in response
             and "formData" in response["edgarSubmission"]
             and response["edgarSubmission"]["headerData"]["submissionType"] == "NPORT-P"
             and "invstOrSecs" in response["edgarSubmission"]["formData"]
             and "invstOrSec" in response["edgarSubmission"]["formData"]["invstOrSecs"]
@@ -702,9 +741,115 @@
             df["pctVal"] = df["pctVal"].astype(float)
             results = (
                 df.fillna("N/A")
                 .replace("N/A", None)
                 .sort_values(by="pctVal", ascending=False)
                 .to_dict(orient="records")
             )
-
-        return [SecEtfHoldingsData.model_validate(d) for d in results]
+        # Extract additional information from the form that doesn't belong in the holdings table.
+        metadata = {}
+        try:
+            gen_info = response["edgarSubmission"]["formData"].get("genInfo", {})  # type: ignore
+            if gen_info:
+                metadata["fund_name"] = gen_info.get("seriesName")
+                metadata["series_id"] = gen_info.get("seriesId")
+                metadata["lei"] = gen_info.get("seriesLei")
+                metadata["period_ending"] = gen_info.get("repPdDate")
+                metadata["fiscal_year_end"] = gen_info.get("repPdEnd")
+                current_month = pd.to_datetime(metadata["period_ending"])
+                month_1 = (current_month - MonthEnd(2)).date().strftime("%Y-%m-%d")
+                month_2 = (current_month - MonthEnd(1)).date().strftime("%Y-%m-%d")
+                month_3 = current_month.strftime("%Y-%m-%d")
+            fund_info = response["edgarSubmission"]["formData"].get("fundInfo", {})  # type: ignore
+            if fund_info:
+                metadata["total_assets"] = float(fund_info.pop("totAssets", None))
+                metadata["total_liabilities"] = float(fund_info.pop("totLiabs", None))
+                metadata["net_assets"] = float(fund_info.pop("netAssets", None))
+                metadata["cash_and_equivalents"] = fund_info.pop(
+                    "cshNotRptdInCorD", None
+                )
+                return_info = fund_info["returnInfo"]["monthlyTotReturns"].get(
+                    "monthlyTotReturn", {}
+                )
+                returns = {
+                    month_1: float(return_info.get("@rtn1")) / 100,
+                    month_2: float(return_info.get("@rtn2")) / 100,
+                    month_3: float(return_info.get("@rtn3")) / 100,
+                }
+                metadata["returns"] = returns
+                flow = {
+                    month_1: {
+                        "creation": float(fund_info["mon1Flow"].get("@sales", None)),
+                        "redemption": float(
+                            fund_info["mon1Flow"].get("@redemption", None)
+                        ),
+                    },
+                    month_2: {
+                        "creation": float(fund_info["mon2Flow"].get("@sales", None)),
+                        "redemption": float(
+                            fund_info["mon2Flow"].get("@redemption", None)
+                        ),
+                    },
+                    month_3: {
+                        "creation": float(fund_info["mon3Flow"].get("@sales")),
+                        "redemption": float(
+                            fund_info["mon3Flow"].get("@redemption", None)
+                        ),
+                    },
+                }
+                metadata["flow"] = flow
+                gains = {
+                    month_1: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon1"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon1"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                    month_2: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon2"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon2"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                    month_3: {
+                        "realized": float(
+                            fund_info["returnInfo"]["othMon3"].get(
+                                "@netRealizedGain", None
+                            )
+                        ),
+                        "unrealized": float(
+                            fund_info["returnInfo"]["othMon3"].get(
+                                "@netUnrealizedAppr", None
+                            )
+                        ),
+                    },
+                }
+                metadata["gains"] = gains
+                _borrowers = fund_info["borrowers"].get("borrower", [])
+                if _borrowers:
+                    borrowers = [
+                        {
+                            "name": d["@name"],
+                            "lei": d["@lei"],
+                            "value": float(d["@aggrVal"]),
+                        }
+                        for d in _borrowers
+                    ]
+                    metadata["borrowers"] = borrowers
+        except Exception as e:  # pylint: disable=W0718
+            warn(f"Error extracting metadata: {e}")
+        return AnnotatedResult(
+            result=[SecEtfHoldingsData.model_validate(d) for d in results],
+            metadata=metadata,
+        )
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/form_13FHR.py` & `openbb_sec-1.2.0/openbb_sec/models/form_13FHR.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,22 +52,23 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         symbol = query.symbol
         urls = []
         cik = symbol.isnumeric()
         filings = (
-            parse_13f.get_13f_candidates(symbol=symbol)
+            await parse_13f.get_13f_candidates(symbol=symbol)
             if cik is False
-            else parse_13f.get_13f_candidates(cik=symbol)
+            else await parse_13f.get_13f_candidates(cik=symbol)
         )
         if query.limit and query.date is None:
             urls = filings.iloc[: query.limit].to_list()
         if query.date is not None:
             date = parse_13f.date_to_quarter_end(query.date.strftime("%Y-%m-%d"))
+            filings.index = filings.index.astype(str)
             urls = [filings.loc[date]]
 
         results = []
 
         async def get_filing(url):
             """Get a single 13F-HR filing and parse it."""
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/institutions_search.py` & `openbb_sec-1.2.0/openbb_sec/models/institutions_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """SEC Institutions Search Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import CotSearchQueryParams
 from openbb_sec.utils.helpers import get_all_ciks
 from pydantic import Field
@@ -36,26 +38,24 @@
     """Transform the query, extract and transform the data from the SEC endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecInstitutionsSearchQueryParams:
         """Transform the query."""
         return SecInstitutionsSearchQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecInstitutionsSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
-        institutions = get_all_ciks(use_cache=query.use_cache)
+        institutions = await get_all_ciks(use_cache=query.use_cache)
         hp = institutions["Institution"].str.contains(query.query, case=False)
         return institutions[hp].astype(str).to_dict("records")
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: SecInstitutionsSearchQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecInstitutionsSearchData]:
         """Transform the data to the standard format."""
         return [SecInstitutionsSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/rss_litigation.py` & `openbb_sec-1.2.0/openbb_sec/models/rss_litigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """SEC Litigation RSS Feed Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
-import requests
 import xmltodict
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.abstract.query_params import QueryParams
-from openbb_sec.utils.definitions import SEC_HEADERS
+from openbb_core.provider.utils.helpers import make_request
+from openbb_sec.utils.definitions import HEADERS
 from pydantic import Field
 
 
 class SecRssLitigationQueryParams(QueryParams):
     """SEC Litigation RSS Feed Query.
 
     Source: https://sec.gov/
@@ -45,34 +47,36 @@
         query: SecRssLitigationQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the SEC endpoint."""
         results = []
         url = "https://www.sec.gov/rss/litigation/litreleases.xml"
-        r = requests.get(url, headers=SEC_HEADERS, timeout=5)
+        r = make_request(url, headers=HEADERS)
 
         if r.status_code == 200:
             data = xmltodict.parse(r.content)
             cols = ["title", "link", "summary", "date", "id"]
             feed = pd.DataFrame.from_records(data["rss"]["channel"]["item"])[
                 ["title", "link", "description", "pubDate", "dc:creator"]
             ]
             feed.columns = cols
-            feed["date"] = pd.to_datetime(feed["date"])
+            feed["date"] = pd.to_datetime(feed["date"], format="mixed")
             feed = feed.set_index("date")
             # Remove special characters
             for column in ["title", "summary"]:
                 feed[column] = (
                     feed[column]
                     .replace(r"[^\w\s]|_", "", regex=True)
                     .replace(r"\n", "", regex=True)
                 )
 
             results = feed.reset_index().to_dict(orient="records")
 
         return results
 
     @staticmethod
-    def transform_data(data: List[Dict], **kwargs: Any) -> List[SecRssLitigationData]:
+    def transform_data(
+        query: SecRssLitigationQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[SecRssLitigationData]:
         """Transform the data to the standard format."""
         return [SecRssLitigationData.model_validate(d) for d in data]
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/schema_files.py` & `openbb_sec-1.2.0/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.5/openbb_sec/models/sic_search.py` & `openbb_sec-1.2.0/openbb_sec/models/sic_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """SEC Standard Industrial Classification Code (SIC) Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
-import requests
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
+from openbb_core.app.utils import get_user_cache_directory
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.cot_search import CotSearchQueryParams
-from openbb_sec.utils.helpers import SEC_HEADERS, sec_session_companies
+from openbb_core.provider.utils.helpers import amake_request
+from openbb_sec.utils.helpers import SEC_HEADERS, sec_callback
 from pydantic import Field
 
 
 class SecSicSearchQueryParams(CotSearchQueryParams):
     """SEC Standard Industrial Classification Code (SIC) Query.
 
     Source: https://sec.gov/
@@ -33,57 +38,61 @@
     Fetcher[
         SecSicSearchQueryParams,
         List[SecSicSearchData],
     ]
 ):
     """Transform the query, extract and transform the data from the SEC endpoints."""
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_query(
         params: Dict[str, Any], **kwargs: Any
     ) -> SecSicSearchQueryParams:
         """Transform the query."""
         return SecSicSearchQueryParams(**params)
 
-    # pylint: disable=unused-argument
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecSicSearchQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract data from the SEC website table."""
         data = pd.DataFrame()
         results: List[Dict] = []
         url = (
             "https://www.sec.gov/corpfin/"
             "division-of-corporation-finance-standard-industrial-classification-sic-code-list"
         )
-        r = (
-            sec_session_companies.get(url, timeout=5, headers=SEC_HEADERS)
-            if query.use_cache is True
-            else requests.get(url, timeout=5, headers=SEC_HEADERS)
-        )
-
-        if r.status_code == 200:
-            data = pd.read_html(r.content.decode())[0].astype(str)
-            if len(data) == 0:
-                return results
-            if query:
-                data = data[
-                    data["SIC Code"].str.contains(query.query, case=False)
-                    | data["Office"].str.contains(query.query, case=False)
-                    | data["Industry Title"].str.contains(query.query, case=False)
-                ]
-            data["SIC Code"] = data["SIC Code"].astype(int)
+        if query.use_cache is True:
+            cache_dir = f"{get_user_cache_directory()}/http/sec_sic"
+            async with CachedSession(
+                cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 30)
+            ) as session:
+                try:
+                    response = await amake_request(
+                        url, headers=SEC_HEADERS, session=session, response_callback=sec_callback  # type: ignore
+                    )
+                finally:
+                    await session.close()
+        else:
+            response = await amake_request(url, headers=SEC_HEADERS, response_callback=sec_callback)  # type: ignore
+
+        data = pd.read_html(response)[0].astype(str)
+        if len(data) == 0:
+            return results
+        if query:
+            data = data[
+                data["SIC Code"].str.contains(query.query, case=False)
+                | data["Office"].str.contains(query.query, case=False)
+                | data["Industry Title"].str.contains(query.query, case=False)
+            ]
+        data["SIC Code"] = data["SIC Code"].astype(int)
         results = data.to_dict("records")
 
         return results
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: SecSicSearchQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[SecSicSearchData]:
         """Transform the data."""
         return [SecSicSearchData.model_validate(d) for d in data]
```

### Comparing `openbb_sec-1.1.5/openbb_sec/models/symbol_map.py` & `openbb_sec-1.2.0/openbb_sec/models/symbol_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """SEC Symbol Mapping Model."""
 
+# pylint: disable=unused-argument
+
 from typing import Any, Dict, Optional
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.symbol_map import SymbolMapQueryParams
 from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 from openbb_sec.utils.helpers import cik_map
 from pydantic import Field
 
-# pylint: disable=unused-argument
-
 
 class SecSymbolMapQueryParams(SymbolMapQueryParams):
     """SEC Symbol Mapping Query.
 
     Source: https://sec.gov/
     """
 
@@ -35,23 +35,25 @@
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> SecSymbolMapQueryParams:
         """Transform the query."""
         return SecSymbolMapQueryParams(**params)
 
     @staticmethod
-    def extract_data(
+    async def aextract_data(
         query: SecSymbolMapQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> Dict:
         """Return the raw data from the SEC endpoint."""
         if not query.query.isdigit():
             raise ValueError("Query is required and must be a valid CIK.")
-        return {"symbol": cik_map(int(query.query))}
+        symbol = await cik_map(int(query.query), query.use_cache)
+        response = {"symbol": symbol}
+        return response
 
     @staticmethod
     def transform_data(
         query: SecSymbolMapQueryParams, data: Dict, **kwargs: Any
     ) -> SecSymbolMapData:
         """Transform the data to the standard format."""
         return SecSymbolMapData.model_validate(data)
```

### Comparing `openbb_sec-1.1.5/openbb_sec/utils/definitions.py` & `openbb_sec-1.2.0/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_sec-1.1.5/openbb_sec/utils/helpers.py` & `openbb_sec-1.2.0/openbb_sec/utils/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,315 +1,260 @@
 """SEC Helpers module."""
 
-# pylint: skip-file
-from datetime import timedelta
+# pylint: disable =unused-argument
+
 from io import BytesIO
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 from zipfile import ZipFile
 
 import pandas as pd
-import requests
-import requests_cache
+from aiohttp_client_cache import SQLiteBackend
+from aiohttp_client_cache.session import CachedSession
 from openbb_core.app.utils import get_user_cache_directory
-from openbb_sec.utils.definitions import HEADERS, QUARTERS, SEC_HEADERS, TAXONOMIES
-
-cache_dir = get_user_cache_directory()
-
-sec_session_companies = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_companies", expire_after=timedelta(days=2)
-)
-sec_session_frames = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_frames", expire_after=timedelta(days=2)
-)
-sec_session_ftd = requests_cache.CachedSession(f"{cache_dir}/http/sec_ftd")
+from openbb_core.provider.utils.helpers import amake_request, make_request
+from openbb_sec.utils.definitions import HEADERS, SEC_HEADERS
 
-sec_session_etf = requests_cache.CachedSession(f"{cache_dir}/http/sec_etf")
 
-sec_session_company_filings = requests_cache.CachedSession(
-    f"{cache_dir}/http/sec_company_filings", expire_after=timedelta(days=1)
-)
+async def sec_callback(response, session):
+    """Response callback for SEC requests."""
+    content_type = response.headers.get("Content-Type", "")
+    if "application/json" in content_type:
+        return await response.json()
+    if "text/html" in content_type:
+        return await response.text(encoding="latin-1")
+    return await response.text()
 
 
-def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
+async def get_all_companies(use_cache: bool = True) -> pd.DataFrame:
     """Get all company names, tickers, and CIK numbers registered with the SEC.
 
     Companies are sorted by market cap.
 
     Returns
     -------
     pd.DataFrame: Pandas DataFrame with columns for Symbol, Company Name, and CIK Number.
 
     Example
     -------
     >>> tickers = get_all_companies()
     """
     url = "https://www.sec.gov/files/company_tickers.json"
 
-    r = (
-        sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=SEC_HEADERS, timeout=5)
-    )
-    df = pd.DataFrame(r.json()).transpose()
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_companies"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS)  # type: ignore
+
+    df = pd.DataFrame(response).transpose()
     cols = ["cik", "symbol", "name"]
     df.columns = cols
     return df.astype(str)
 
 
-def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
+async def get_all_ciks(use_cache: bool = True) -> pd.DataFrame:
     """Get a list of entity names and their CIK number."""
-    HEADERS = {
-        "User-Agent": "my real company name definitelynot@fakecompany.com",
-        "Accept-Encoding": "gzip, deflate",
-        "Host": "www.sec.gov",
-    }
     url = "https://www.sec.gov/Archives/edgar/cik-lookup-data.txt"
-    r = (
-        sec_session_companies.get(url, headers=HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=HEADERS, timeout=5)
-    )
-    data = r.text
-    lines = data.split("\n")
+
+    async def callback(response, session):
+        """Response callback for CIK lookup data."""
+        return await response.text(encoding="latin-1")
+
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_ciks"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS, response_callback=callback)  # type: ignore
+    data = response
+    lines = data.split("\n")  # type: ignore
     data_list = []
     delimiter = ":"
     for line in lines:
         row = line.split(delimiter)
         data_list.append(row)
     df = pd.DataFrame(data_list)
     df = df.iloc[:, 0:2]
     cols = ["Institution", "CIK Number"]
     df.columns = cols
     df = df.dropna()
 
-    return df
+    return df.astype(str)
 
 
-def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
+async def get_mf_and_etf_map(use_cache: bool = True) -> pd.DataFrame:
     """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbols = pd.DataFrame()
 
     url = "https://www.sec.gov/files/company_tickers_mf.json"
-    r = (
-        sec_session_companies.get(url, headers=SEC_HEADERS, timeout=5)
-        if use_cache is True
-        else requests.get(url, headers=SEC_HEADERS, timeout=5)
-    )
-    if r.status_code == 200:
-        symbols = pd.DataFrame(data=r.json()["data"], columns=r.json()["fields"])
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_mf_etf_map"
+        async with CachedSession(
+            cache=SQLiteBackend(cache_dir, expire_after=3600 * 24 * 2)
+        ) as session:
+            try:
+                response = await amake_request(url, headers=SEC_HEADERS, session=session, response_callback=sec_callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, headers=SEC_HEADERS, response_callback=sec_callback)  # type: ignore
+
+    symbols = pd.DataFrame(data=response["data"], columns=response["fields"])  # type: ignore
 
-    return symbols
+    return symbols.astype(str)
 
 
-def search_institutions(keyword: str, use_cache: bool = True) -> pd.DataFrame:
+async def search_institutions(keyword: str, use_cache: bool = True) -> pd.DataFrame:
     """Search for an institution by name.  It is case-insensitive."""
-    institutions = get_all_ciks(use_cache=use_cache)
+    institutions = await get_all_ciks(use_cache=use_cache)
     hp = institutions["Institution"].str.contains(keyword, case=False)
-    return institutions[hp].astype(str)
+    return institutions[hp]
 
 
-def symbol_map(symbol: str, use_cache: bool = True) -> str:
+async def symbol_map(symbol: str, use_cache: bool = True) -> str:
     """Return the CIK number of a ticker symbol for querying the SEC API."""
     symbol = symbol.upper().replace(".", "-")
-    symbols = get_all_companies(use_cache=use_cache)
+    symbols = await get_all_companies(use_cache=use_cache)
 
     if symbol not in symbols["symbol"].to_list():
-        symbols = get_mf_and_etf_map(use_cache=use_cache).astype(str)
+        symbols = await get_mf_and_etf_map(use_cache=use_cache)
         if symbol not in symbols["symbol"].to_list():
             return ""
-
     cik = symbols[symbols["symbol"] == symbol]["cik"].iloc[0]
     cik_: str = ""
     temp = 10 - len(cik)
-    for i in range(temp):
+    for i in range(temp):  # pylint: disable=W0612
         cik_ = cik_ + "0"
 
     return str(cik_ + cik)
 
 
-def cik_map(cik: int, use_cache: bool = True) -> str:
+async def cik_map(cik: Union[str, int], use_cache: bool = True) -> str:
     """Convert a CIK number to a ticker symbol.  Enter CIK as an integer with no leading zeros.
 
     Function is not meant for funds.
 
     Parameters
     ----------
     cik : int
         The CIK number to convert to a ticker symbol.
 
     Returns
     -------
     str: The ticker symbol associated with the CIK number.
     """
-    _cik = str(cik)
+    _cik = str(cik) if isinstance(cik, int) else cik.lstrip("0")
     symbol = ""
-    companies = get_all_companies(use_cache=use_cache).astype(str)
+    companies = await get_all_companies(use_cache=use_cache)
     if _cik in companies["cik"].to_list():
         symbol = companies[companies["cik"] == _cik]["symbol"].iloc[0]
     else:
-        return f"Error: CIK, {cik}, does not have a unique ticker."
+        return f"Error: CIK, {_cik}, does not have a unique ticker."
 
     return symbol
 
 
-def get_frame(
-    year: int,
-    quarter: Optional[QUARTERS] = None,
-    taxonomy: TAXONOMIES = "us-gaap",
-    units: str = "USD",
-    fact: str = "Revenues",
-    instantaneous: bool = False,
-    use_cache: bool = True,
-) -> Dict:
-    """Get a frame of data for a given fact.
-
-    The xbrl/frames API aggregates one fact for each reporting entity
-    that is last filed that most closely fits the calendrical period requested.
-
-    This API supports for annual, quarterly and instantaneous data:
-
-    https://data.sec.gov/api/xbrl/frames/us-gaap/AccountsPayableCurrent/USD/CY2019Q1I.json
-
-    Where the units of measure specified in the XBRL contains a numerator and a denominator,
-    these are separated by “-per-” such as “USD-per-shares”. Note that the default unit in XBRL is “pure”.
-
-    CY####Q# for quarterly data (duration 91 days +/- 30 days).
-    Because company financial calendars can start and end on any month or day and even change in length from quarter to
-    quarter according to the day of the week, the frame data is assembled by the dates that best align with a calendar
-    quarter or year. Data users should be mindful different reporting start and end dates for facts contained in a frame.
-
-    Example facts:
-    Revenues
-    GrossProfit
-    CostOfRevenue
-    DividendsCash
-    DistributedEarnings
-    AccountsPayableCurrent
-    OperatingExpenses
-    OperatingIncomeLoss
-    NoninterestIncome
-    InterestAndDebtExpense
-    IncomeTaxExpenseBenefit
-    NetIncomeLoss
-
-    Facts where units are, "shares":
-    WeightedAverageNumberOfDilutedSharesOutstanding
-    """
-    if fact in ["WeightedAverageNumberOfDilutedSharesOutstanding"]:
-        units = "shares"
-
-    url = f"https://data.sec.gov/api/xbrl/frames/{taxonomy}/{fact}/{units}/CY{year}"
-
-    if quarter:
-        url = url + f"Q{quarter}"
-
-    if instantaneous:
-        url = url + "I"
-    url = url + ".json"
-    r = (
-        requests.get(url, headers=HEADERS, timeout=5)
-        if use_cache is False
-        else sec_session_frames.get(url, headers=HEADERS, timeout=5)
-    )
-
-    if r.status_code != 200:
-        raise RuntimeError(f"Request failed with status code {r.status_code}")
-
-    response = r.json()
-
-    data = sorted(response["data"], key=lambda x: x["val"], reverse=True)
-    metadata = {
-        "frame": response["ccp"],
-        "tag": response["tag"],
-        "label": response["label"],
-        "description": response["description"],
-        "taxonomy": response["taxonomy"],
-        "unit": response["uom"],
-        "count": response["pts"],
-    }
-
-    results = {"metadata": metadata, "data": data}
-
-    return results
-
-
-def get_schema_filelist(query: str = "", url: str = "") -> List:
+def get_schema_filelist(query: str = "", url: str = "", use_cache: bool = True) -> List:
     """Get a list of schema files from the SEC website."""
     results: List = []
     url = url if url else f"https://xbrl.fasb.org/us-gaap/{query}"
     _url = url
     _url = url + "/" if query else _url
-    r = sec_session_companies.get(_url, headers=HEADERS, timeout=5)
-
-    if r.status_code != 200:
-        raise RuntimeError(f"Request failed with status code {r.status_code}")
-
-    data = pd.read_html(r.content.decode())[0]["Name"].dropna()
+    response = make_request(_url)
+    data = pd.read_html(response.content)[0]["Name"].dropna()
     if len(data) > 0:
         data.iloc[0] = url if not query else url + "/"
         results = data.to_list()
 
     return results
 
 
-def download_zip_file(url, symbol: Optional[str] = None) -> List[Dict]:
+async def download_zip_file(
+    url, symbol: Optional[str] = None, use_cache: bool = True
+) -> List[Dict]:
     """Download a list of files from URLs."""
     results = pd.DataFrame()
-    r = sec_session_ftd.get(url, timeout=5, headers=HEADERS)
-    if r.status_code == 200:
-        try:
-            data = pd.read_csv(BytesIO(r.content), compression="zip", sep="|")
-            results = data.iloc[:-2]
-        except ValueError:
-            zip_file = ZipFile(BytesIO(r.content))
-            file_list = [d.filename for d in zip_file.infolist()]
-            for item in file_list:
+
+    async def callback(response, session):
+        """Response callback for ZIP file downloads."""
+        return await response.read()
+
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_ftd"
+        async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+            try:
+                response = await amake_request(url, session=session, headers=HEADERS, response_callback=callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, response_callback=callback)  # type: ignore
+
+    try:
+        data = pd.read_csv(BytesIO(response), compression="zip", sep="|")  # type: ignore
+        results = data.iloc[:-2]
+    except ValueError:
+        zip_file = ZipFile(BytesIO(response))  # type: ignore
+        file_list = [d.filename for d in zip_file.infolist()]
+        for item in file_list:
+            with zip_file.open(item) as _item:
                 _file = pd.read_csv(
-                    zip_file.open(item),
+                    _item,
                     encoding="ISO-8859-1",
                     sep="|",
                     low_memory=False,
                     on_bad_lines="skip",
                 )
                 results = pd.concat([results, _file.iloc[:-2]])
-        if "SETTLEMENT DATE" in results.columns:
-            results = results.rename(
-                columns={
-                    "SETTLEMENT DATE": "date",
-                    "SYMBOL": "symbol",
-                    "CUSIP": "cusip",
-                    "QUANTITY (FAILS)": "quantity",
-                    "PRICE": "price",
-                    "DESCRIPTION": "description",
-                }
-            )
-            if symbol is not None:
-                results = results[results["symbol"] == symbol]
-            results["date"] = pd.to_datetime(results["date"], format="%Y%m%d").dt.date
-            results["price"] = results["price"].mask(
-                results["price"].str.contains(r"^\d+(?:\.\d+)?$", regex=True)
-                == False,  # noqa
-                None,
+
+    if "SETTLEMENT DATE" in results.columns:
+        results = results.rename(
+            columns={
+                "SETTLEMENT DATE": "date",
+                "SYMBOL": "symbol",
+                "CUSIP": "cusip",
+                "QUANTITY (FAILS)": "quantity",
+                "PRICE": "price",
+                "DESCRIPTION": "description",
+            }
+        )
+        if symbol is not None:
+            results = results[results["symbol"] == symbol]
+        results["date"] = pd.to_datetime(results["date"], format="%Y%m%d").dt.date
+        results["price"] = results["price"].mask(
+            results["price"].str.contains(  # pylint: disable=C0121
+                r"^\d+(?:\.\d+)?$", regex=True
             )
-            results["price"] = results["price"].astype(float)
+            == False,  # noqa
+            None,
+        )
+        results["price"] = results["price"].astype(float)
 
     return results.reset_index(drop=True).to_dict("records")
 
 
-def get_ftd_urls() -> Dict:
+async def get_ftd_urls() -> Dict:
     """Get Fails-to-Deliver Data URLs."""
     results = {}
     position = None
     key = "title"
     value = "Fails-to-Deliver Data"
 
-    r = requests.get("https://www.sec.gov/data.json", timeout=5, headers=SEC_HEADERS)
-    if r.status_code != 200:
-        raise RuntimeError(f"Request failed with status code {str(r.status_code)}")
-    data = r.json()["dataset"]
+    r = await amake_request("https://www.sec.gov/data.json", headers=SEC_HEADERS)
+    data = r.get("dataset", {})  # type: ignore
 
     for index, d in enumerate(data):
         if key in d and d[key] == value:
             position = index
             break
     if position is not None:
         fails = data[position]["distribution"]
@@ -319,15 +264,15 @@
         ftd_urls = pd.Series(index=dates, data=urls)
         ftd_urls.index = ftd_urls.index.str.replace("_", "")
         results = ftd_urls.to_dict()
 
     return results
 
 
-def get_series_id(
+async def get_series_id(
     symbol: Optional[str] = None, cik: Optional[str] = None, use_cache: bool = True
 ):
     """Map the fund to the series and class IDs for validating the correct filing.
 
     For an exact match, use a symbol.
     """
     symbol = symbol if symbol else ""
@@ -335,77 +280,69 @@
 
     results = pd.DataFrame()
     if not symbol and not cik:
         raise ValueError("Either symbol or cik must be provided.")
 
     target = symbol if symbol else cik
     choice = "cik" if not symbol else "symbol"
-    funds = get_mf_and_etf_map(use_cache=use_cache).astype(str)
+    funds = await get_mf_and_etf_map(use_cache=use_cache)
 
     results = funds[
         funds["cik"].str.contains(target, case=False)
         | funds["seriesId"].str.contains(target, case=False)
         | funds["classId"].str.contains(target, case=False)
         | funds["symbol"].str.contains(target, case=False)
     ]
 
     if len(results) > 0:
         results = results[results[choice if not symbol else choice] == target]
 
         return results
 
 
-def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
+async def get_nport_candidates(symbol: str, use_cache: bool = True) -> List[Dict]:
     """Get a list of all NPORT-P filings for a given fund's symbol."""
     results = []
-    _series_id = get_series_id(symbol, use_cache=use_cache)
+    _series_id = await get_series_id(symbol, use_cache=use_cache)
     try:
         series_id = (
-            symbol_map(symbol, use_cache)
+            await symbol_map(symbol, use_cache)
             if _series_id is None or len(_series_id) == 0
             else _series_id["seriesId"].iloc[0]
         )
-    except IndexError:
-        raise ValueError("Fund not found for, the symbol: " + symbol)
+    except IndexError as e:
+        raise ValueError("Fund not found for, the symbol: " + symbol) from e
     if series_id == "" or series_id is None:
         raise ValueError("Fund not found for, the symbol: " + symbol)
 
     url = f"https://efts.sec.gov/LATEST/search-index?q={series_id}&dateRange=all&forms=NPORT-P"
 
-    def request_data(url: str = url, use_cache: bool = use_cache):
-        r = (
-            sec_session_companies.get(url, timeout=5, headers=HEADERS)
-            if use_cache is True
-            else requests.get(url, headers=HEADERS, timeout=5)
-        )
-        return r
-
-    r = request_data(url, use_cache=use_cache)
-
-    if r.status_code != 200:
-        if r.status_code == 500:
-            r = request_data()
-            if r.status_code != 200:
-                raise RuntimeError(
-                    f"Request failed with status code {str(r.status_code)}"
-                )
-        if r.status_code not in (200, 500):
-            raise RuntimeError(f"Request failed with status code {str(r.status_code)}")
-    r_json = r.json()
+    if use_cache is True:
+        cache_dir = f"{get_user_cache_directory()}/http/sec_etf"
+        async with CachedSession(cache=SQLiteBackend(cache_dir)) as session:
+            try:
+                response = await amake_request(url, session=session, headers=HEADERS, response_callback=sec_callback)  # type: ignore
+            finally:
+                await session.close()
+    else:
+        response = await amake_request(url, response_callback=sec_callback)  # type: ignore
 
-    if "hits" in r_json and len(r_json["hits"]["hits"]) > 0:
-        hits = r_json["hits"]["hits"]
+    if "hits" in response and len(response["hits"].get("hits")) > 0:  # type: ignore
+        hits = response["hits"]["hits"]  # type: ignore
         results = [
             {
                 "name": d["_source"]["display_names"][0],
                 "cik": d["_source"]["ciks"][0],
                 "file_date": d["_source"]["file_date"],
                 "period_ending": d["_source"]["period_ending"],
                 "form_type": d["_source"]["form"],
-                "primary_doc": f"https://www.sec.gov/Archives/edgar/data/{int(d['_source']['ciks'][0])}/{d['_id'].replace('-', '').replace(':', '/')}",  # noqa
+                "primary_doc": (
+                    f"https://www.sec.gov/Archives/edgar/data/{int(d['_source']['ciks'][0])}"  # noqa
+                    + f"/{d['_id'].replace('-', '').replace(':', '/')}"  # noqa
+                ),
             }
             for d in hits
         ]
     return (
         sorted(results, key=lambda d: d["file_date"], reverse=True)
         if len(results) > 0
         else results
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openbb_sec-1.1.5/openbb_sec/utils/parse_13f.py` & `openbb_sec-1.2.0/openbb_sec/utils/parse_13f.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,37 +15,40 @@
     return (
         (to_datetime(date).to_period("Q").to_timestamp("D") + offsets.QuarterEnd())
         .date()
         .strftime("%Y-%m-%d")
     )
 
 
-def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
+async def get_13f_candidates(symbol: Optional[str] = None, cik: Optional[str] = None):
     """Get the 13F-HR filings for a given symbol or CIK."""
     fetcher = SecCompanyFilingsFetcher()
     params: Dict[str, Any] = {}
     if cik is not None:
         params["cik"] = str(cik)
     if symbol is not None:
         params["symbol"] = symbol
     if cik is None and symbol is None:
         raise ValueError("Either symbol or cik must be provided.")
 
     params["use_cache"] = False
     params["form_type"] = "13F-HR"
-    query = fetcher.transform_query(params)
-    filings = fetcher.extract_data(query, {})
+    filings = await fetcher.fetch_data(params, {})
+    filings = [d.model_dump() for d in filings]
     if len(filings) == 0:
         raise ValueError(f"No 13F-HR filings found for {symbol if symbol else cik}.")
 
     # Filings before June 30, 2013 are non-structured and are not supported by downstream parsers.
+    up_to = to_datetime("2013-06-30").date()  # pylint: disable=unused-variable # noqa
     return (
         DataFrame(data=filings)
-        .query("`reportDate` >= '2013-06-30'")
-        .set_index("reportDate")["completeSubmissionUrl"]
+        .query("`report_date` >= @up_to")
+        .set_index("report_date")["complete_submission_url"]
+        .fillna("N/A")
+        .replace("N/A", None)
     )
 
 
 async def complete_submission_callback(response, _):
     """Use callback function for processing the response object."""
     if response.status == 200:
         return await response.text()
```

### Comparing `openbb_sec-1.1.5/pyproject.toml` & `openbb_sec-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "openbb-sec"
-version = "1.1.5"
+version = "1.2.0"
 description = "SEC extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_sec" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.1.6"
-requests-cache = "^1.1.0"
+openbb-core = "^1.2.1"
+aiohttp-client-cache = "^0.11.0"
+aiosqlite = "^0.20.0"
 xmltodict = "^0.13.0"
-pytest-freezegun = "^0.4.2"
+lxml = "^5.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 sec = "openbb_sec:sec_provider"
```

### Comparing `openbb_sec-1.1.5/PKG-INFO` & `openbb_sec-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: openbb-sec
-Version: 1.1.5
+Version: 1.2.0
 Summary: SEC extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
-Requires-Dist: pytest-freezegun (>=0.4.2,<0.5.0)
-Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
+Requires-Dist: aiohttp-client-cache (>=0.11.0,<0.12.0)
+Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB SEC Provider
 
 This extension integrates the [SEC](https://www.sec.gov/edgar) data provider into the OpenBB Platform.
 
@@ -24,11 +27,9 @@
 
 To install the extension:
 
 ```bash
 pip install openbb-sec
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

