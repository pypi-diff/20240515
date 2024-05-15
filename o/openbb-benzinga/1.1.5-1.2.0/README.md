# Comparing `tmp/openbb_benzinga-1.1.5.tar.gz` & `tmp/openbb_benzinga-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_benzinga-1.1.5.tar", max compression
+gzip compressed data, was "openbb_benzinga-1.2.0.tar", max compression
```

## Comparing `openbb_benzinga-1.1.5.tar` & `openbb_benzinga-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      439 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/README.md
--rw-r--r--   0        0        0      877 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    17979 2024-04-19 16:31:25.550563 openbb_benzinga-1.1.5/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9801 2024-04-19 16:31:25.550563 openbb_benzinga-1.1.5/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-04-17 12:33:20.553645 openbb_benzinga-1.1.5/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      463 2024-04-19 16:41:36.303279 openbb_benzinga-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_benzinga-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      312 2024-05-15 14:21:47.631780 openbb_benzinga-1.2.0/README.md
+-rw-r--r--   0        0        0      898 2024-05-14 15:30:05.610153 openbb_benzinga-1.2.0/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-23 10:22:39.652736 openbb_benzinga-1.2.0/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    18109 2024-05-10 10:40:27.289939 openbb_benzinga-1.2.0/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6206 2024-05-10 10:40:27.290127 openbb_benzinga-1.2.0/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9807 2024-05-10 10:40:27.290287 openbb_benzinga-1.2.0/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-04-08 12:02:16.579354 openbb_benzinga-1.2.0/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754477 openbb_benzinga-1.2.0/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-04-23 10:22:39.653147 openbb_benzinga-1.2.0/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-15 16:07:32.771241 openbb_benzinga-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 openbb_benzinga-1.2.0/PKG-INFO
```

### Comparing `openbb_benzinga-1.1.5/openbb_benzinga/__init__.py` & `openbb_benzinga-1.2.0/openbb_benzinga/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from openbb_benzinga.models.company_news import BenzingaCompanyNewsFetcher
 from openbb_benzinga.models.price_target import BenzingaPriceTargetFetcher
 from openbb_benzinga.models.world_news import BenzingaWorldNewsFetcher
 from openbb_core.provider.abstract.provider import Provider
 
 benzinga_provider = Provider(
     name="benzinga",
-    website="https://www.benzinga.com/",
+    website="https://www.benzinga.com",
     description="""Benzinga is a financial data provider that offers an API
-    focused on information that moves the market.""",
+focused on information that moves the market.""",
     credentials=["api_key"],
     fetcher_dict={
         "AnalystSearch": BenzingaAnalystSearchFetcher,
         "CompanyNews": BenzingaCompanyNewsFetcher,
         "WorldNews": BenzingaWorldNewsFetcher,
         "PriceTarget": BenzingaPriceTargetFetcher,
     },
+    repr_name="Benzinga",
 )
```

### Comparing `openbb_benzinga-1.1.5/openbb_benzinga/models/analyst_search.py` & `openbb_benzinga-1.2.0/openbb_benzinga/models/analyst_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
     __alias_dict__ = {
         "analyst_ids": "analyst",
         "firm_ids": "firm",
         "limit": "pageSize",
     }
     __json_schema_extra__ = {
-        "analyst_name": ["multiple_items_allowed"],
-        "firm_name": ["multiple_items_allowed"],
-        "analyst_ids": ["multiple_items_allowed"],
-        "firm_ids": ["multiple_items_allowed"],
-        "fields": ["multiple_items_allowed"],
+        "analyst_name": {"multiple_items_allowed": True},
+        "firm_name": {"multiple_items_allowed": True},
+        "analyst_ids": {"multiple_items_allowed": True},
+        "firm_ids": {"multiple_items_allowed": True},
+        "fields": {"multiple_items_allowed": True},
     }
 
     analyst_ids: Optional[str] = Field(
         default=None,
         description="List of analyst IDs to return.",
     )
     firm_ids: Optional[str] = Field(
@@ -86,27 +86,27 @@
         default=None,
         description="A weighted average of the total_ratings_percentile,"
         + " overall_avg_return_percentile, and overall_success_rate",
     )
     overall_success_rate: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain overall.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     overall_avg_return_percentile: Optional[float] = Field(
         default=None,
         description="The percentile (normalized) of this analyst's overall average"
         + " return per rating in comparison to other analysts' overall average returns per rating.",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     total_ratings_percentile: Optional[float] = Field(
         default=None,
         description="The percentile (normalized) of this analyst's total number of ratings"
         + " in comparison to the total number of ratings published by all other analysts",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     total_ratings: Optional[int] = Field(
         default=None,
         description="Number of recommendations made by this analyst.",
     )
     overall_gain_count: Optional[int] = Field(
         default=None,
@@ -115,21 +115,21 @@
     overall_loss_count: Optional[int] = Field(
         default=None,
         description="The number of ratings that have lost value since the date of recommendation",
     )
     overall_average_return: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating since the date of recommendation",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
     )
     overall_std_dev: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings since the date of recommendation",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="overall_stdev",
     )
     gain_count_1m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last month",
         alias="1m_gain_count",
     )
@@ -137,33 +137,33 @@
         default=None,
         description="The number of ratings that have lost value over the last month",
         alias="1m_loss_count",
     )
     average_return_1m: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over the last month",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1m_average_return",
     )
     std_dev_1m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last month",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1m_stdev",
     )
     smart_score_1m: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last month.",
         alias="1m_smart_score",
     )
     success_rate_1m: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last month",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1m_success_rate",
     )
     gain_count_3m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 3 months",
         alias="3m_gain_count",
     )
@@ -172,33 +172,33 @@
         description="The number of ratings that have lost value over the last 3 months",
         alias="3m_loss_count",
     )
     average_return_3m: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 3 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3m_average_return",
     )
     std_dev_3m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 3 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3m_stdev",
     )
     smart_score_3m: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last 3 months.",
         alias="3m_smart_score",
     )
     success_rate_3m: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 3 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3m_success_rate",
     )
     gain_count_6m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 6 months",
         alias="6m_gain_count",
     )
@@ -207,22 +207,22 @@
         description="The number of ratings that have lost value over the last 6 months",
         alias="6m_loss_count",
     )
     average_return_6m: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 6 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="6m_average_return",
     )
     std_dev_6m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 6 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="6m_stdev",
     )
     gain_count_9m: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 9 months",
         alias="9m_gain_count",
     )
@@ -231,33 +231,33 @@
         description="The number of ratings that have lost value over the last 9 months",
         alias="9m_loss_count",
     )
     average_return_9m: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 9 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="9m_average_return",
     )
     std_dev_9m: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 9 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="9m_stdev",
     )
     smart_score_9m: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last 9 months.",
         alias="9m_smart_score",
     )
     success_rate_9m: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 9 months",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="9m_success_rate",
     )
     gain_count_1y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 1 year",
         alias="1y_gain_count",
     )
@@ -266,33 +266,33 @@
         description="The number of ratings that have lost value over the last 1 year",
         alias="1y_loss_count",
     )
     average_return_1y: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 1 year",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1y_average_return",
     )
     std_dev_1y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 1 year",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1y_stdev",
     )
     smart_score_1y: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last 1 year.",
         alias="1y_smart_score",
     )
     success_rate_1y: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 1 year",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="1y_success_rate",
     )
     gain_count_2y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 2 years",
         alias="2y_gain_count",
     )
@@ -301,33 +301,33 @@
         description="The number of ratings that have lost value over the last 2 years",
         alias="2y_loss_count",
     )
     average_return_2y: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 2 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="2y_average_return",
     )
     std_dev_2y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 2 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="2y_stdev",
     )
     smart_score_2y: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last 3 years.",
         alias="2y_smart_score",
     )
     success_rate_2y: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 2 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="2y_success_rate",
     )
     gain_count_3y: Optional[int] = Field(
         default=None,
         description="The number of ratings that have gained value over the last 3 years",
         alias="3y_gain_count",
     )
@@ -336,33 +336,33 @@
         description="The number of ratings that have lost value over the last 3 years",
         alias="3y_loss_count",
     )
     average_return_3y: Optional[float] = Field(
         default=None,
         description="The average percent (normalized) price difference per rating over"
         + " the last 3 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3y_average_return",
     )
     std_dev_3y: Optional[float] = Field(
         default=None,
         description="The standard deviation in percent (normalized) price difference in the"
         + " analyst's ratings over the last 3 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3y_stdev",
     )
     smart_score_3y: Optional[float] = Field(
         default=None,
         description="A weighted average smart score over the last 3 years.",
         alias="3y_smart_score",
     )
     success_rate_3y: Optional[float] = Field(
         default=None,
         description="The percentage (normalized) of gain/loss ratings that resulted in a gain over the last 3 years",
-        json_schema_extra={"unit_measurement": "percent", "frontend_multiply": 100},
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
         alias="3y_success_rate",
     )
 
     @field_validator("last_updated", mode="before", check_fields=False)
     @classmethod
     def validate_date(cls, v: float) -> Optional[dateType]:
         """Validate last_updated."""
```

### Comparing `openbb_benzinga-1.1.5/openbb_benzinga/models/company_news.py` & `openbb_benzinga-1.2.0/openbb_benzinga/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "display": "displayOutput",
         "limit": "pageSize",
         "start_date": "dateFrom",
         "end_date": "dateTo",
         "updated_since": "updatedSince",
         "published_since": "publishedSince",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("date", "")
     )
     display: Literal["headline", "abstract", "full"] = Field(
         default="full",
         description="Specify headline only (headline), headline + teaser (abstract), or headline + full body (full).",
@@ -148,18 +148,19 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract data."""
         token = credentials.get("benzinga_api_key") if credentials else ""
 
         base_url = "https://api.benzinga.com/api/v2/news"
 
-        query.sort = f"{query.sort}:{query.order}" if query.sort and query.order else ""
-        querystring = get_querystring(
-            query.model_dump(by_alias=True), ["order", "pageSize"]
+        model = query.model_dump(by_alias=True)
+        model["sort"] = (
+            f"{query.sort}:{query.order}" if query.sort and query.order else ""
         )
+        querystring = get_querystring(model, ["order", "pageSize"])
 
         pages = math.ceil(query.limit / 100) if query.limit else 1
         page_size = 100 if query.limit and query.limit > 100 else query.limit
         urls = [
             f"{base_url}?{querystring}&page={page}&pageSize={page_size}&token={token}"
             for page in range(pages)
         ]
```

### Comparing `openbb_benzinga-1.1.5/openbb_benzinga/models/price_target.py` & `openbb_benzinga-1.2.0/openbb_benzinga/models/price_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-ratings
     """
 
     __alias_dict__ = {
         "limit": "pagesize",
         "symbol": "parameters[tickers]",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=0,
         description="Page offset. For optimization, performance and technical reasons,"
         + " page offsets are limited from 0 - 100000. Limit the query results by other parameters such as date."
         + " Used in conjunction with the limit and date parameters.",
     )
```

### Comparing `openbb_benzinga-1.1.5/openbb_benzinga/models/world_news.py` & `openbb_benzinga-1.2.0/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.5/PKG-INFO` & `openbb_benzinga-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-benzinga
-Version: 1.1.5
+Version: 1.2.0
 Summary: Benzinga extension for OpenBB
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
 
 # OpenBB Benzinga Provider
 
 This extension integrates the [Benzinga](https://www.benzinga.com/) data provider into the OpenBB Platform.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-benzinga
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

