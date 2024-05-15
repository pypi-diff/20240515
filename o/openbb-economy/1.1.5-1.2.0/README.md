# Comparing `tmp/openbb_economy-1.1.5.tar.gz` & `tmp/openbb_economy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_economy-1.1.5.tar", max compression
+gzip compressed data, was "openbb_economy-1.2.0.tar", max compression
```

## Comparing `openbb_economy-1.1.5.tar` & `openbb_economy-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      461 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/README.md
--rw-r--r--   0        0        0       32 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/__init__.py
--rw-r--r--   0        0        0     9797 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_economy-1.1.5/openbb_economy/py.typed
--rw-r--r--   0        0        0      458 2024-04-19 16:39:30.623005 openbb_economy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openbb_economy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-05-15 14:27:51.744569 openbb_economy-1.2.0/README.md
+-rw-r--r--   0        0        0       32 2024-04-23 10:22:39.599846 openbb_economy-1.2.0/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    12007 2024-05-09 15:04:29.063912 openbb_economy-1.2.0/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-04-23 10:22:39.600176 openbb_economy-1.2.0/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.734317 openbb_economy-1.2.0/openbb_economy/py.typed
+-rw-r--r--   0        0        0      484 2024-05-15 16:03:57.437693 openbb_economy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 openbb_economy-1.2.0/PKG-INFO
```

### Comparing `openbb_economy-1.1.5/openbb_economy/economy_router.py` & `openbb_economy-1.2.0/openbb_economy/economy_router.py`

 * *Files 15% similar despite different names*

```diff
@@ -302,7 +302,77 @@
     extra_params: ExtraParams,
 ) -> OBBject:
     """Query the Geo Fred API for regional economic data by series group.
 
     The series group ID is found by using `fred_search` and the `series_id` parameter.
     """
     return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="CountryProfile",
+    examples=[
+        APIEx(parameters={"provider": "econdb", "country": "united_kingdom"}),
+        APIEx(
+            description="Enter the country as the full name, or iso code."
+            + " If `latest` is False, the complete history for each series is returned.",
+            parameters={
+                "country": "united_states,jp",
+                "latest": False,
+                "provider": "econdb",
+            },
+        ),
+    ],
+)
+async def country_profile(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get a profile of country statistics and economic indicators."""
+    return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="AvailableIndicators",
+    examples=[
+        APIEx(parameters={"provider": "econdb"}),
+    ],
+)
+async def available_indicators(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get the available economic indicators for a provider."""
+    return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="EconomicIndicators",
+    examples=[
+        APIEx(parameters={"provider": "econdb", "symbol": "PCOCO"}),
+        APIEx(
+            description="Enter the country as the full name, or iso code."
+            + " Use `available_indicators()` to get a list of supported indicators from EconDB.",
+            parameters={
+                "symbol": "CPI",
+                "country": "united_states,jp",
+                "provider": "econdb",
+            },
+        ),
+        APIEx(
+            description="Use the `main` symbol to get the group of main indicators for a country.",
+            parameters={"provider": "econdb", "symbol": "main", "country": "eu"},
+        ),
+    ],
+)
+async def indicators(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get economic indicators by country and indicator."""
+    return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_economy-1.1.5/openbb_economy/gdp/gdp_router.py` & `openbb_economy-1.2.0/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_economy-1.1.5/PKG-INFO` & `openbb_economy-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: openbb-economy
-Version: 1.1.5
+Version: 1.2.0
 Summary: Economy extension for OpenBB
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
 
 # OpenBB Economy Extension
 
 The Economy extension provides global macroeconomic data access for the OpenBB Platform.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-economy
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

