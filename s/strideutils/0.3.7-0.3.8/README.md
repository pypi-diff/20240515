# Comparing `tmp/strideutils-0.3.7.tar.gz` & `tmp/strideutils-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.7.tar", max compression
+gzip compressed data, was "strideutils-0.3.8.tar", max compression
```

## Comparing `strideutils-0.3.7.tar` & `strideutils-0.3.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1835 2024-05-06 20:50:09.251204 strideutils-0.3.7/README.md
--rw-r--r--   0        0        0     1046 2024-05-06 20:50:09.251204 strideutils-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/__init__.py
--rw-r--r--   0        0        0     5408 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1594 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    13332 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/stride_config.py
--rw-r--r--   0        0        0    42613 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/twilio_connector.py
--rw-r--r--   0        0        0      659 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils/types.py
--rw-r--r--   0        0        0        0 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-06 20:50:09.251204 strideutils-0.3.7/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-06 20:50:09.255204 strideutils-0.3.7/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 strideutils-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-15 17:08:23.022040 strideutils-0.3.8/README.md
+-rw-r--r--   0        0        0     1046 2024-05-15 17:08:23.022040 strideutils-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/__init__.py
+-rw-r--r--   0        0        0     6064 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    13348 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_config.py
+-rw-r--r--   0        0        0    42613 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0      659 2024-05-15 17:08:23.026040 strideutils-0.3.8/strideutils/types.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-15 17:08:23.022040 strideutils-0.3.8/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 strideutils-0.3.8/PKG-INFO
```

### Comparing `strideutils-0.3.7/README.md` & `strideutils-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/pyproject.toml` & `strideutils-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
 python = ">=3.11"
```

### Comparing `strideutils-0.3.7/strideutils/coingecko.py` & `strideutils-0.3.8/strideutils/coingecko.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 
 from strideutils import stride_config, stride_requests
 from strideutils.stride_config import config
 
 COINGECKO_ENDPOINT = "https://pro-api.coingecko.com/"
 COINGECKO_PRICE_QUERY = "api/v3/simple/price?ids={ticker_id}&vs_currencies=usd"
+COINGECKO_TVL_QUERY = "api/v3/coins/{ticker_id}"
 
 
 def get_coingecko_name(chain_config: stride_config.ChainConfig) -> str:
     """
     Returns the coingecko name for a given chain
     """
     try:
@@ -27,15 +28,14 @@
 def get_token_price(
     ticker: str,
     api_token: str = config.COINGECKO_API_TOKEN,
     cache_response: bool = False,
 ):
     """
     Reads token price from coingecko
-    If a redis_client is provided, then store the value.
     """
     # TODO: Consider using the coingecko ID for stTokens instead of the redemption rate
     # Get redemption rate for calculating st token prices
     redemption_rate = float(1)
     if ticker.startswith('st') and ticker[3].isupper():
         redemption_rate = stride_requests.get_redemption_rate(ticker[2:])
         ticker = ticker[2:]
@@ -49,34 +49,52 @@
     headers = {'x-cg-pro-api-key': api_token}
     response = stride_requests.request(endpoint, headers=headers, cache_response=cache_response)
     price = response[coingecko_name]["usd"] * redemption_rate
 
     return price
 
 
+def get_tvl(
+    chain_config: stride_config.ChainConfig,
+    api_token: str = config.COINGECKO_API_TOKEN,
+    cache_response: bool = False,
+) -> float:
+    """
+    Fetch TVL from coingecko in USD
+    """
+    coingecko_name = get_coingecko_name(chain_config)
+    endpoint = COINGECKO_ENDPOINT + COINGECKO_TVL_QUERY.format(ticker_id=coingecko_name)
+    headers = {'x-cg-pro-api-key': api_token}
+
+    # The data structure is huge https://docs.coingecko.com/reference/coins-id
+    response = stride_requests.request(endpoint, headers=headers, cache_response=cache_response)
+    return float(response['market_data']['market_cap']['usd'])
+
+
 def get_token_price_history(token: str, num_days=90, use_key=False, memo={}) -> pd.Series:
     """
     returns a Pandas Series with token price data going back num_days
     e.g. get_token_price_history('uatom', 30) returns a Series with 30 days of ATOM price data
     TODO: Figure out why API key is throwing an error when used.
     """
     price_key = (token, num_days)
     if price_key not in memo:
         tstr = get_coingecko_name(config.get_chain(ticker=token))
-        rurl = f"https://api.coingecko.com/api/v3/coins/{tstr}/market_chart?vs_currency=usd&days={num_days}"
-        rel_headers = {"x-cg-pro-api-key": config.COINGECKO_API_TOKEN}
-        if not use_key:
-            rel_headers = None
+        rurl = (
+            f"https://api.coingecko.com/api/v3/coins/{tstr}/market_chart?vs_currency=usd&days={num_days}"  # noqa:E231
+        )
+        rel_headers = {"x-cg-pro-api-key": config.COINGECKO_API_TOKEN} if use_key else None
+
         r = requests.get(
             rurl,
             headers=rel_headers,
         )
         assert r.status_code == 200
         out_df = pd.DataFrame(r.json()["prices"])
-        out_df.columns = ["time", "price"]
+        out_df.columns = pd.Index(["time", "price"])
         out_df["time"] = pd.to_datetime(out_df["time"], unit="ms")
         out_df["price"] = out_df["price"].astype(float)
         out_df.set_index("time", inplace=True)
         memo[token] = out_df
     return memo[token]
 
 
@@ -85,25 +103,26 @@
     returns a Pandas Series with token volume data going back num_days
     e.g. get_token_volume_history('uatom', 30) returns a Series with 30 days of ATOM volume data
     TODO: Figure out why API key is throwing an error when used.
     """
     volume_key = (token, num_days)
     if volume_key not in memo:
         tstr = get_coingecko_name(config.get_chain(ticker=token))
-        rurl = f"https://api.coingecko.com/api/v3/coins/{tstr}/market_chart?vs_currency=usd&days={num_days}"
-        rel_headers = {"x-cg-pro-api-key": config.COINGECKO_API_TOKEN}
-        if not use_key:
-            rel_headers = None
+        rurl = (
+            f"https://api.coingecko.com/api/v3/coins/{tstr}/market_chart?vs_currency=usd&days={num_days}"  # noqa:E231
+        )
+        rel_headers = {"x-cg-pro-api-key": config.COINGECKO_API_TOKEN} if use_key else None
+
         r = requests.get(
             rurl,
             headers=rel_headers,
         )
         assert r.status_code == 200
         out_df = pd.DataFrame(r.json()["total_volumes"])
-        out_df.columns = ["time", "volume"]
+        out_df.columns = pd.Index(["time", "volume"])
         out_df["time"] = pd.to_datetime(out_df["time"], unit="ms")
         out_df["volume"] = out_df["volume"].astype(float)
         out_df.set_index("time", inplace=True)
         memo[token] = out_df
     return memo[token]
```

### Comparing `strideutils-0.3.7/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.8/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/cryptography.py` & `strideutils-0.3.8/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/exec_tx.py` & `strideutils-0.3.8/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/invariant_helpers.py` & `strideutils-0.3.8/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/run_safely.py` & `strideutils-0.3.8/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/sheets_connector.py` & `strideutils-0.3.8/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/slack_connector.py` & `strideutils-0.3.8/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/stride_alerts.py` & `strideutils-0.3.8/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/stride_config.py` & `strideutils-0.3.8/strideutils/stride_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         'host_zones': host_zone_config,
         'app_chains': app_chain_config,
     }
 
     # Load non-nested configs, then overwrite with the chain configs
     config_dict = raw_secrets
     config_dict.update(raw_config)
-    config_dict.update(chain_configs)
+    config_dict.update(chain_configs)  # type: ignore
     return Config(**config_dict)  # type: ignore
 
 
 def _init_config() -> Config:
     """
     Initializes the main config files
     """
```

### Comparing `strideutils-0.3.7/strideutils/stride_requests.py` & `strideutils-0.3.8/strideutils/stride_requests.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/stride_upstash.py` & `strideutils-0.3.8/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/twilio_connector.py` & `strideutils-0.3.8/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils/types.py` & `strideutils-0.3.8/strideutils/types.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.8/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.8/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.8/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.8/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.7/PKG-INFO` & `strideutils-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

