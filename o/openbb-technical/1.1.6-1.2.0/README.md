# Comparing `tmp/openbb_technical-1.1.6.tar.gz` & `tmp/openbb_technical-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_technical-1.1.6.tar", max compression
+gzip compressed data, was "openbb_technical-1.2.0.tar", max compression
```

## Comparing `openbb_technical-1.1.6.tar` & `openbb_technical-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      605 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/README.md
--rw-r--r--   0        0        0       43 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.505645 openbb_technical-1.1.6/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    64220 2024-04-19 16:31:25.534563 openbb_technical-1.1.6/openbb_technical/technical_router.py
--rw-r--r--   0        0        0      614 2024-04-19 16:40:37.463144 openbb_technical-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 openbb_technical-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      478 2024-05-15 14:26:27.342633 openbb_technical-1.2.0/README.md
+-rw-r--r--   0        0        0       43 2024-02-29 11:03:36.744125 openbb_technical-1.2.0/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-04-23 10:22:39.610514 openbb_technical-1.2.0/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.744320 openbb_technical-1.2.0/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-04-23 10:22:39.610659 openbb_technical-1.2.0/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    63911 2024-05-15 11:31:42.982565 openbb_technical-1.2.0/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0      640 2024-05-15 16:05:06.756816 openbb_technical-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 openbb_technical-1.2.0/PKG-INFO
```

### Comparing `openbb_technical-1.1.6/openbb_technical/helpers.py` & `openbb_technical-1.2.0/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.1.6/openbb_technical/relative_rotation.py` & `openbb_technical-1.2.0/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.1.6/openbb_technical/technical_router.py` & `openbb_technical-1.2.0/openbb_technical/technical_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,23 +49,18 @@
         ),
         PythonEx(
             description="When the assets are not traded 252 days per year,"
             + "adjust the momentum and volatility periods accordingly.",
             code=[
                 "crypto_data = obb.crypto.price.historical("
                 + " symbol='BTCUSD,ETHUSD,SOLUSD', start_date='2021-01-01', provider='yfinance')",
-                "rr_data = obb.technical.relative_rotation(data=crypto_data.results, benchmark='BTCUSD',"
+                "rr_data = obb.technical.relative_rotation(data=crypto_data.results, benchmark='BTC-USD',"
                 + " long_period=365, short_period=30, window=30, trading_periods=365)",
             ],
         ),
-        APIEx(
-            description="Note that the mock data displayed here is insufficient."
-            + " It must contain multiple symbols, with the benchmark, and be daily data at least 1 year in length.",
-            parameters={"benchmark": "SPY", "data": APIEx.mock_data("timeseries")},
-        ),
     ],
 )
 async def relative_rotation(
     data: List[Data],
     benchmark: str,
     study: Literal["price", "volume", "volatility"] = "price",
     long_period: Optional[int] = 252,
@@ -147,15 +142,14 @@
             benchmark_data : list[Data]
                 The data representing the selected 'study' for the benchmark.
             rs_ratios : list[Data]
                 The normalized relative strength ratios data.
             rs_momentum : list[Data]
                 The normalized relative strength momentum data.
     """
-
     params = RelativeRotationQueryParams(
         data=data,
         benchmark=benchmark,
         study=study,
         long_period=long_period,
         short_period=short_period,
         window=window,
```

### Comparing `openbb_technical-1.1.6/pyproject.toml` & `openbb_technical-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "openbb-technical"
-version = "1.1.6"
+version = "1.2.0"
 description = "Technical Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_technical" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.1"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.1.6"
+openbb-core = "^1.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 technical = "openbb_technical.technical_router:router"
```

### Comparing `openbb_technical-1.1.6/PKG-INFO` & `openbb_technical-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-technical
-Version: 1.1.6
+Version: 1.2.0
 Summary: Technical Analysis extension for OpenBB
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
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Technical Analysis Extension
@@ -29,11 +31,9 @@
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-technical
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

