# Comparing `tmp/openbb_tradingeconomics-1.1.5.tar.gz` & `tmp/openbb_tradingeconomics-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradingeconomics-1.1.5.tar", max compression
+gzip compressed data, was "openbb_tradingeconomics-1.2.0.tar", max compression
```

## Comparing `openbb_tradingeconomics-1.1.5.tar` & `openbb_tradingeconomics-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      469 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/README.md
--rw-r--r--   0        0        0      440 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     4606 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-04-17 12:33:20.849645 openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0      512 2024-04-19 16:43:06.055506 openbb_tradingeconomics-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-05-15 14:24:32.425446 openbb_tradingeconomics-1.2.0/README.md
+-rw-r--r--   0        0        0      944 2024-05-14 15:30:05.620721 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     8326 2024-05-15 12:02:12.290758 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-04-23 10:22:39.799520 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     4104 2024-05-14 15:30:05.621205 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0      538 2024-05-15 16:07:37.861279 openbb_tradingeconomics-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.2.0/PKG-INFO
```

### Comparing `openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/countries.py` & `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.1.5/openbb_tradingeconomics/utils/url_generator.py` & `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/url_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     # Check if all fields in to_include are present in query_args
     # and elements in available_args that are not in to_include are not present in query_args
     return all(field in query_args for field in to_include) and all(
         field not in query_args for field in available_args if field not in to_include
     )
 
 
+# pylint: disable = R0912
 def generate_url(in_query):
     """Generate the url for trading economimcs.
 
     There is not a single api endpoint to hit so these are generated based on the combinations.
     There are also some combinations that return no data so that will return an empty string.
     """
     # Converting the input query to a dict of params that are not None
@@ -58,14 +59,17 @@
         url = f"{base_url}/country/{country}?{urlencode(query)}&c="
     # Country + Group
     elif check_args(query, ["country", "group"]):
         url = f"{base_url}/country/{country}/group/{group}?c="
     # Country + Group + Date
     elif check_args(query, ["country", "group", "start_date", "end_date"]):
         url = f'{base_url}/country/{country}/group/{group}/{query["start_date"]}/{query["end_date"]}?c='
+    # Country + Date + Importance
+    elif check_args(query, ["country", "importance", "start_date", "end_date"]):
+        url = f'{base_url}/country/{country}/{query["start_date"]}/{query["end_date"]}?{urlencode(query)}&c='
     # By date only
     elif check_args(query, ["start_date", "end_date"]):
         url = f'{base_url}/country/All/{query["start_date"]}/{query["end_date"]}?c='
     # By importance only
     elif check_args(query, ["importance"]):
         url = f"{base_url}?{urlencode(query)}&c="
     # By importance and date
@@ -80,9 +84,12 @@
     # All fields
     elif check_args(
         query, ["country", "group", "importance", "start_date", "end_date"]
     ):
         start_date = query["start_date"]
         end_date = query["end_date"]
         url = f"{base_url}/country/{country}/group/{group}/{start_date}/{end_date}?{urlencode(query)}&c="
+    # Calendar IDs
+    elif check_args(query, ["calendar_id"]):
+        url = f'{base_url}/calendarid/{str(query["calendar_id"])}?c='
 
     return url if url else ""
```

### Comparing `openbb_tradingeconomics-1.1.5/pyproject.toml` & `openbb_tradingeconomics-1.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "openbb-tradingeconomics"
-version = "1.1.5"
+version = "1.2.0"
 description = "Trading Economics extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_tradingeconomics" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.1.6"
+openbb-core = "^1.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
```

### Comparing `openbb_tradingeconomics-1.1.5/PKG-INFO` & `openbb_tradingeconomics-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-tradingeconomics
-Version: 1.1.5
+Version: 1.2.0
 Summary: Trading Economics extension for OpenBB
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
 
 # OpenBB Trading Economics Provider
 
 This extension integrates the [Trading Economics](https://docs.tradingeconomics.com/) data provider into the OpenBB SDK.
 
 ## Installation
 
 To install the extension:
 
 ```bash
 pip install openbb-tradingeconomics
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

