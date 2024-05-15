# Comparing `tmp/hydradx-api-0.3.0.tar.gz` & `tmp/hydradx-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydradx-api-0.3.0.tar", max compression
+gzip compressed data, was "hydradx-api-0.3.1.tar", max compression
```

## Comparing `hydradx-api-0.3.0.tar` & `hydradx-api-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-10-22 09:22:23.089507 hydradx-api-0.3.0/LICENSE
--rw-r--r--   0        0        0       46 2023-10-22 09:24:43.873179 hydradx-api-0.3.0/hydradxapi/__init__.py
--rw-r--r--   0        0        0     1879 2024-01-03 08:50:43.933584 hydradx-api-0.3.0/hydradxapi/__main__.py
--rw-r--r--   0        0        0      752 2023-12-08 14:24:16.503815 hydradx-api-0.3.0/hydradxapi/api.py
--rw-r--r--   0        0        0      990 2023-10-24 09:56:48.463623 hydradx-api-0.3.0/hydradxapi/base.py
--rw-r--r--   0        0        0      751 2023-11-02 13:39:43.136143 hydradx-api-0.3.0/hydradxapi/client.py
--rw-r--r--   0        0        0      391 2023-10-23 14:58:13.927674 hydradx-api-0.3.0/hydradxapi/pallets/__init__.py
--rw-r--r--   0        0        0      261 2023-10-23 15:25:54.614641 hydradx-api-0.3.0/hydradxapi/pallets/balances.py
--rw-r--r--   0        0        0      703 2023-12-29 10:00:26.430773 hydradx-api-0.3.0/hydradxapi/pallets/fees.py
--rw-r--r--   0        0        0     3753 2023-12-29 10:00:26.431089 hydradx-api-0.3.0/hydradxapi/pallets/omnipool.py
--rw-r--r--   0        0        0     1583 2024-03-17 07:31:21.949695 hydradx-api-0.3.0/hydradxapi/pallets/registry.py
--rw-r--r--   0        0        0     2988 2024-02-02 07:58:03.588328 hydradx-api-0.3.0/hydradxapi/pallets/stableswap.py
--rw-r--r--   0        0        0      278 2023-10-23 14:58:13.891025 hydradx-api-0.3.0/hydradxapi/pallets/tokens.py
--rw-r--r--   0        0        0      531 2024-03-17 07:32:25.168376 hydradx-api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      741 2024-03-17 07:32:29.719421 hydradx-api-0.3.0/setup.py
--rw-r--r--   0        0        0      656 2024-03-17 07:32:29.719674 hydradx-api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-10-22 09:22:23.089507 hydradx-api-0.3.1/LICENSE
+-rw-r--r--   0        0        0       46 2023-10-22 09:24:43.873179 hydradx-api-0.3.1/hydradxapi/__init__.py
+-rw-r--r--   0        0        0     1879 2024-01-03 08:50:43.933584 hydradx-api-0.3.1/hydradxapi/__main__.py
+-rw-r--r--   0        0        0      752 2023-12-08 14:24:16.503815 hydradx-api-0.3.1/hydradxapi/api.py
+-rw-r--r--   0        0        0      990 2023-10-24 09:56:48.463623 hydradx-api-0.3.1/hydradxapi/base.py
+-rw-r--r--   0        0        0      751 2023-11-02 13:39:43.136143 hydradx-api-0.3.1/hydradxapi/client.py
+-rw-r--r--   0        0        0      391 2023-10-23 14:58:13.927674 hydradx-api-0.3.1/hydradxapi/pallets/__init__.py
+-rw-r--r--   0        0        0      261 2023-10-23 15:25:54.614641 hydradx-api-0.3.1/hydradxapi/pallets/balances.py
+-rw-r--r--   0        0        0      703 2023-12-29 10:00:26.430773 hydradx-api-0.3.1/hydradxapi/pallets/fees.py
+-rw-r--r--   0        0        0     3753 2023-12-29 10:00:26.431089 hydradx-api-0.3.1/hydradxapi/pallets/omnipool.py
+-rw-r--r--   0        0        0     1583 2024-03-17 07:31:21.949695 hydradx-api-0.3.1/hydradxapi/pallets/registry.py
+-rw-r--r--   0        0        0     3125 2024-05-15 19:10:17.698397 hydradx-api-0.3.1/hydradxapi/pallets/stableswap.py
+-rw-r--r--   0        0        0      418 2024-05-15 19:10:17.699431 hydradx-api-0.3.1/hydradxapi/pallets/tokens.py
+-rw-r--r--   0        0        0      531 2024-05-15 19:10:30.845267 hydradx-api-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      741 2024-05-15 19:10:37.591902 hydradx-api-0.3.1/setup.py
+-rw-r--r--   0        0        0      656 2024-05-15 19:10:37.592175 hydradx-api-0.3.1/PKG-INFO
```

### Comparing `hydradx-api-0.3.0/LICENSE` & `hydradx-api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/__main__.py` & `hydradx-api-0.3.1/hydradxapi/__main__.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/api.py` & `hydradx-api-0.3.1/hydradxapi/api.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/base.py` & `hydradx-api-0.3.1/hydradxapi/base.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/client.py` & `hydradx-api-0.3.1/hydradxapi/client.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/pallets/fees.py` & `hydradx-api-0.3.1/hydradxapi/pallets/fees.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/pallets/omnipool.py` & `hydradx-api-0.3.1/hydradxapi/pallets/omnipool.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/pallets/registry.py` & `hydradx-api-0.3.1/hydradxapi/pallets/registry.py`

 * *Files identical despite different names*

### Comparing `hydradx-api-0.3.0/hydradxapi/pallets/stableswap.py` & `hydradx-api-0.3.1/hydradxapi/pallets/stableswap.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,28 @@
     assets: List[Asset]
     initial_amplification: int
     final_amplification: int
     initial_block: int
     final_block: int
     fee: float
     reserves: dict[int, str]
+    shares: int
     account: str
 
     def as_dict(self):
         return {
             "pool_id": self.pool_id,
             "assets": [asset.as_dict() for asset in self.assets],
             "initial_amplification": self.initial_amplification,
             "final_amplification": self.final_amplification,
             "initial_block": self.initial_block,
             "final_block": self.final_block,
             "fee": self.fee,
             "reserves": self.reserves,
+            "shares": self.shares,
             "account": self.account,
         }
 
 
 class StableSwap(Pallet):
     MODULE_NAME = "Stableswap"
 
@@ -61,15 +63,15 @@
             i_amp = entry[1]["initial_amplification"].value
             f_amp = entry[1]["final_amplification"].value
             i_block = entry[1]["initial_block"].value
             f_block = entry[1]["final_block"].value
             fee = int(entry[1]["fee"].value) / 10000
 
             s_assets = [self._registry.asset_metadata(int(asset)) for asset in assets]
-
+            shares = self._tokens.total_issuance(int(pool_id))
             try:
                 pool_account = POOL_ACCOUNTS[int(pool_id)]
                 reserves = {}
                 for asset in assets:
                     balance = self._tokens.account_free_balance(
                         pool_account, int(asset)
                     )
@@ -83,11 +85,12 @@
                 s_assets,
                 int(i_amp),
                 int(f_amp),
                 int(i_block),
                 int(f_block),
                 fee,
                 reserves,
+                shares,
                 pool_account,
             )
 
         return result
```

### Comparing `hydradx-api-0.3.0/pyproject.toml` & `hydradx-api-0.3.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydradx-api"
-version = "0.3.0"
+version = "0.3.1"
 description = "HydraDX interface"
 authors = ["Martin Hloska <martin.hloska@gmail.com>"]
 repository = "https://github.com/enthusiastmartin/hydradx-api"
 license = "MIT OR Apache-2.0"
 packages = [
     {include = "hydradxapi"}
 ]
```

### Comparing `hydradx-api-0.3.0/setup.py` & `hydradx-api-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['click>=8.1.7,<9.0.0',
  'pytest>=7.4.2,<8.0.0',
  'substrate-interface>=1.7.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'hydradx-api',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'HydraDX interface',
     'long_description': None,
     'author': 'Martin Hloska',
     'author_email': 'martin.hloska@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/enthusiastmartin/hydradx-api',
```

### Comparing `hydradx-api-0.3.0/PKG-INFO` & `hydradx-api-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydradx-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: HydraDX interface
 Home-page: https://github.com/enthusiastmartin/hydradx-api
 License: MIT OR Apache-2.0
 Author: Martin Hloska
 Author-email: martin.hloska@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

