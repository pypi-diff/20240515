# Comparing `tmp/openbb_government_us-1.1.5.tar.gz` & `tmp/openbb_government_us-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_government_us-1.1.5.tar", max compression
+gzip compressed data, was "openbb_government_us-1.2.0.tar", max compression
```

## Comparing `openbb_government_us-1.1.5.tar` & `openbb_government_us-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      445 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/README.md
--rw-r--r--   0        0        0      988 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5269 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-17 12:33:20.669645 openbb_government_us-1.1.5/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0      522 2024-04-19 16:42:24.367398 openbb_government_us-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 openbb_government_us-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      318 2024-05-15 14:25:32.440933 openbb_government_us-1.2.0/README.md
+-rw-r--r--   0        0        0      976 2024-05-14 15:30:05.616106 openbb_government_us-1.2.0/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-02-29 11:03:36.873377 openbb_government_us-1.2.0/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-08 12:02:16.650213 openbb_government_us-1.2.0/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5138 2024-05-09 13:34:29.221479 openbb_government_us-1.2.0/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-04-23 10:22:39.670563 openbb_government_us-1.2.0/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-02 11:35:59.475353 openbb_government_us-1.2.0/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0      548 2024-05-15 16:06:14.659267 openbb_government_us-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 openbb_government_us-1.2.0/PKG-INFO
```

### Comparing `openbb_government_us-1.1.5/openbb_government_us/__init__.py` & `openbb_government_us-1.2.0/openbb_government_us/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 )
 from openbb_government_us.models.treasury_prices import (
     GovernmentUSTreasuryPricesFetcher,
 )
 
 government_us_provider = Provider(
     name="government_us",
-    website="https://data.gov/",
-    description=(
-        "Data.gov is the United States government's open data website."
-        + " It provides access to datasets published by agencies across the federal government. "
-        + "Data.gov is intended to provide access to government open data to the public, "
-        + "achieve agency missions, drive innovation, fuel economic activity, "
-        + "and uphold the ideals of an open and transparent government."
-    ),
+    website="https://data.gov",
+    description="""Data.gov is the United States government's open data website.
+It provides access to datasets published by agencies across the federal government.
+Data.gov is intended to provide access to government open data to the public, achieve
+agency missions, drive innovation, fuel economic activity, and uphold the ideals of
+an open and transparent government.""",
     fetcher_dict={
         "TreasuryAuctions": GovernmentUSTreasuryAuctionsFetcher,
         "TreasuryPrices": GovernmentUSTreasuryPricesFetcher,
     },
+    repr_name="Data.gov | United States Government",
 )
```

### Comparing `openbb_government_us-1.1.5/openbb_government_us/models/treasury_auctions.py` & `openbb_government_us-1.2.0/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.1.5/openbb_government_us/models/treasury_prices.py` & `openbb_government_us-1.2.0/openbb_government_us/models/treasury_prices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """US Government Treasury Prices."""
 
 # pylint: disable=unused-argument
 import asyncio
-from datetime import datetime, timedelta
+from datetime import date, timedelta
 from io import StringIO
 from typing import Any, Dict, List, Literal, Optional
 
 import requests
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.treasury_prices import (
     TreasuryPricesData,
@@ -18,15 +18,15 @@
 from pydantic import Field
 
 
 class GovernmentUSTreasuryPricesQueryParams(TreasuryPricesQueryParams):
     """US Government Treasury Prices Query."""
 
     cusip: Optional[str] = Field(description="Filter by CUSIP.", default=None)
-    security_type: Literal[None, "bill", "note", "bond", "tips", "frn"] = Field(
+    security_type: Optional[Literal["bill", "note", "bond", "tips", "frn"]] = Field(
         description="Filter by security type.",
         default=None,
     )
 
 
 class GovernmentUSTreasuryPricesData(TreasuryPricesData):
     """US Government Treasury Prices Data."""
@@ -41,26 +41,22 @@
     """US Government Treasury Prices Fetcher."""
 
     @staticmethod
     def transform_query(
         params: Dict[str, Any]
     ) -> GovernmentUSTreasuryPricesQueryParams:
         """Transform query params."""
+        yesterday = date.today() - timedelta(days=1)
+        last_bd = (
+            yesterday - timedelta(yesterday.weekday() - 4)
+            if yesterday.weekday() > 4
+            else yesterday
+        )
         if params.get("date") is None:
-            _date = datetime.now().date()
-        else:
-            _date = (
-                datetime.strptime(params["date"], "%Y-%m-%d").date()
-                if isinstance(params["date"], str)
-                else params["date"]
-            )
-        if _date.weekday() > 4:
-            _date = _date - timedelta(days=_date.weekday() - 4)
-        params["date"] = _date
-
+            params["date"] = last_bd
         return GovernmentUSTreasuryPricesQueryParams(**params)
 
     # pylint: disable=unused-argument
     @staticmethod
     async def aextract_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
```

### Comparing `openbb_government_us-1.1.5/pyproject.toml` & `openbb_government_us-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "openbb-government-us"
-version = "1.1.5"
+version = "1.2.0"
 description = "US Government Data Extension for OpenBB"
 authors = ["OpenBB <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_government_us" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.6"
+openbb-core = "^1.2.1"
 random-user-agent = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_government_us-1.1.5/PKG-INFO` & `openbb_government_us-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-government-us
-Version: 1.1.5
+Version: 1.2.0
 Summary: US Government Data Extension for OpenBB
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
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Government US Provider
 
 This extension integrates the [US Government](https://data.gov) data provider into the OpenBB Platform.
 
@@ -23,11 +25,9 @@
 
 To install the extension:
 
 ```bash
 pip install openbb-us-government
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

