# Comparing `tmp/bpx_py-1.1.2.tar.gz` & `tmp/bpx_py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpx_py-1.1.2.tar", max compression
+gzip compressed data, was "bpx_py-1.1.4.tar", max compression
```

## Comparing `bpx_py-1.1.2.tar` & `bpx_py-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-02 10:37:46.359101 bpx_py-1.1.2/LICENSE
--rw-r--r--   0        0        0     2311 2024-05-02 10:37:46.359101 bpx_py-1.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:37:46.359101 bpx_py-1.1.2/bpx/__async/__init__.py
--rw-r--r--   0        0        0     5170 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/__async/account.py
--rw-r--r--   0        0        0     1573 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/__async/public.py
--rw-r--r--   0        0        0        1 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/__init__.py
--rw-r--r--   0        0        0     5025 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/account.py
--rw-r--r--   0        0        0        0 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/base/__init__.py
--rw-r--r--   0        0        0     8448 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/base/base_account.py
--rw-r--r--   0        0        0     1804 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/base/base_public.py
--rw-r--r--   0        0        0     1131 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/enums/__init__.py
--rw-r--r--   0        0        0     1793 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/http_client/__init__.py
--rw-r--r--   0        0        0     2100 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/http_client/async_http_client.py
--rw-r--r--   0        0        0      409 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/http_client/http_client.py
--rw-r--r--   0        0        0     1003 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/http_client/sync_http_client.py
--rw-r--r--   0        0        0     1452 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/public.py
--rw-r--r--   0        0        0     1181 2024-05-02 10:37:46.363101 bpx_py-1.1.2/bpx/simulations.py
--rw-r--r--   0        0        0     1280 2024-05-02 10:37:46.363101 bpx_py-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 bpx_py-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 15:40:43.485698 bpx_py-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2311 2024-05-15 15:40:43.485698 bpx_py-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/__async/__init__.py
+-rw-r--r--   0        0        0     5256 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/__async/account.py
+-rw-r--r--   0        0        0     1576 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/__async/public.py
+-rw-r--r--   0        0        0        1 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/__init__.py
+-rw-r--r--   0        0        0     5177 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/account.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/base/__init__.py
+-rw-r--r--   0        0        0     8696 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/base/base_account.py
+-rw-r--r--   0        0        0     1804 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/base/base_public.py
+-rw-r--r--   0        0        0     1131 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/enums/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:43.485698 bpx_py-1.1.4/bpx/http_client/__init__.py
+-rw-r--r--   0        0        0     2100 2024-05-15 15:40:43.489698 bpx_py-1.1.4/bpx/http_client/async_http_client.py
+-rw-r--r--   0        0        0      409 2024-05-15 15:40:43.489698 bpx_py-1.1.4/bpx/http_client/http_client.py
+-rw-r--r--   0        0        0     1003 2024-05-15 15:40:43.489698 bpx_py-1.1.4/bpx/http_client/sync_http_client.py
+-rw-r--r--   0        0        0     1462 2024-05-15 15:40:43.489698 bpx_py-1.1.4/bpx/public.py
+-rw-r--r--   0        0        0     1645 2024-05-15 15:40:43.489698 bpx_py-1.1.4/bpx/simulations.py
+-rw-r--r--   0        0        0     1280 2024-05-15 15:40:43.489698 bpx_py-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 bpx_py-1.1.4/PKG-INFO
```

### Comparing `bpx_py-1.1.2/LICENSE` & `bpx_py-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/README.md` & `bpx_py-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/__async/account.py` & `bpx_py-1.1.4/bpx/__async/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,26 @@
         self.http_client = http_client
         self.http_client.proxy = proxy
 
     async def get_balances(self, window: int = None):
         url, headers = super().get_balances(window)
         return await self.http_client.get(url, headers=headers)
 
-    async def deposits(self, limit: int = 100, offset: int = 0, window: int = None):
-        url, headers, params = super().deposits(limit, offset, window)
+    async def get_deposits(self, limit: int = 100, offset: int = 0, window: int = None):
+        url, headers, params = super().get_deposits(limit, offset, window)
         return await self.http_client.get(url, headers=headers, params=params)
 
     async def get_deposit_address(self, blockchain: str, window: int = None):
         url, headers, params = super().get_deposit_address(blockchain, window)
         return await self.http_client.get(url, headers=headers, params=params)
 
-    async def get_withdrawals(self, limit: int = 100, offset: int = 0, window: int = None):
-        url, headers, params = super().get_withdrawals(limit, offset, window)
+    async def get_withdrawals(self, limit: int = 100, offset: int = 0,
+                              __from: int = None,to: int = None, window: int = None):
+
+        url, headers, params = super().get_withdrawals(limit, offset, __from, to, window)
         return await self.http_client.get(url, headers=headers, params=params)
 
     async def withdrawal(self, address: str,
                    symbol: str,
                    blockchain: str,
                    quantity: str,
                    window: int = None):
```

### Comparing `bpx_py-1.1.2/bpx/__async/public.py` & `bpx_py-1.1.4/bpx/__async/public.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     async def get_ticker(self, symbol: str):
         return await self.http_client.get(self.get_ticker_url(symbol))
 
     async def get_depth(self, symbol: str):
         return await self.http_client.get(self.get_depth_url(symbol))
 
-    async def get_klines(self, symbol: str, interval: str, start_time=0, end_time=0):
+    async def get_klines(self, symbol: str, interval: str, start_time: int, end_time=0):
         return await self.http_client.get(self.get_klines_url(symbol, interval, start_time, end_time))
 
     async def get_status(self):
         return await self.http_client.get(self.get_status_url())
 
     async def get_ping(self):
         return await self.http_client.get(self.get_ping_url())
```

### Comparing `bpx_py-1.1.2/bpx/account.py` & `bpx_py-1.1.4/bpx/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,28 @@
         self.http_client = default_http_client
         self.http_client.proxies = proxy
 
     def get_balances(self, window: int = None):
         url, headers = super().get_balances(window)
         return self.http_client.get(url, headers=headers)
 
-    def deposits(self, limit: int = 100, offset: int = 0, window: int = None):
-        url, headers, params = super().deposits(limit, offset, window)
+    def get_deposits(self, limit: int = 100, offset: int = 0,
+                     __from: int = None, to: int = None,  window: int = None):
+
+        url, headers, params = super().get_deposits(limit, offset, window, __from, to)
         return self.http_client.get(url, headers=headers, params=params)
 
     def get_deposit_address(self, blockchain: str, window: int = None):
         url, headers, params = super().get_deposit_address(blockchain, window)
         return self.http_client.get(url, headers=headers, params=params)
 
-    def get_withdrawals(self, limit: int = 100, offset: int = 0, window: int = None):
-        url, headers, params = super().get_withdrawals(limit, offset, window)
+    def get_withdrawals(self, limit: int = 100, offset: int = 0,
+                        __from: int = None, to: int = None, window: int = None):
+
+        url, headers, params = super().get_withdrawals(limit, offset, __from, to, window)
         return self.http_client.get(url, headers=headers, params=params)
 
     def withdrawal(self, address: str,
                    symbol: str,
                    blockchain: str,
                    quantity: str,
                    window: int = None):
```

### Comparing `bpx_py-1.1.2/bpx/base/base_account.py` & `bpx_py-1.1.4/bpx/base/base_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,41 +22,49 @@
         self.debug = debug
 
     def get_balances(self, window: int):
         headers = self._headers({}, 'balanceQuery', window=window)
         url = self.BPX_API_URL + 'api/v1/capital'
         return url, headers
 
-    def deposits(self, limit: int, offset: int, window: int):
+    def get_deposits(self, limit: int, offset: int, window: int, __from=None, to=None):
         if limit > 1000 or limit < 0:
             raise LimitValueError
         if offset < 0:
             raise NegativeValueError(offset)
         params = {
             'limit': limit,
             'offset': offset,
         }
+        if __from:
+            params['from'] = __from
+        if to:
+            params['to'] = to
         headers = self._headers(params, 'depositQueryAll', window=window)
         url = self.BPX_API_URL + 'wapi/v1/capital/deposits'
         return url, headers, params
 
     def get_deposit_address(self, blockchain: str, window: int):
         if not Blockchain.has_value(blockchain):
             raise InvalidBlockchainValue(blockchain)
         params = {'blockchain': blockchain}
         headers = self._headers(params, 'depositAddressQuery', window=window)
         url = self.BPX_API_URL + 'wapi/v1/capital/deposit/address'
         return url, headers, params
 
-    def get_withdrawals(self, limit: int, offset: int, window: int):
+    def get_withdrawals(self, limit: int, offset: int, __from: int, to: int, window: int):
         if limit > 1000 or limit < 0:
             raise LimitValueError
         if offset < 0:
             raise NegativeValueError(offset)
         params = {'limit': limit, 'offset': offset}
+        if __from:
+            params['from'] = __from
+        if to:
+            params['to'] = to
         headers = self._headers(params, 'withdrawalQueryAll', window=window)
         url = self.BPX_API_URL + 'wapi/v1/capital/withdrawals'
         return url, headers, params
 
     def withdrawal(self, address: str,
                    symbol: str,
                    blockchain: str,
```

### Comparing `bpx_py-1.1.2/bpx/base/base_public.py` & `bpx_py-1.1.4/bpx/base/base_public.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/enums/__init__.py` & `bpx_py-1.1.4/bpx/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/exceptions/__init__.py` & `bpx_py-1.1.4/bpx/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/http_client/async_http_client.py` & `bpx_py-1.1.4/bpx/http_client/async_http_client.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/http_client/sync_http_client.py` & `bpx_py-1.1.4/bpx/http_client/sync_http_client.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.1.2/bpx/public.py` & `bpx_py-1.1.4/bpx/public.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def get_ticker(self, symbol: str):
         return self.http_client.get(self.get_ticker_url(symbol))
 
     def get_depth(self, symbol: str):
         return self.http_client.get(self.get_depth_url(symbol))
 
-    def get_klines(self, symbol: str, interval: str, start_time=0, end_time=0):
+    def get_klines(self, symbol: str, interval: str, start_time: int, end_time: int = 0):
         return self.http_client.get(self.get_klines_url(symbol, interval, start_time, end_time))
 
     def get_status(self):
         return self.http_client.get(self.get_status_url())
 
     def get_ping(self):
         return self.http_client.get(self.get_ping_url())
```

### Comparing `bpx_py-1.1.2/pyproject.toml` & `bpx_py-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpx-py"
-version = "1.1.2"
+version = "1.1.4"
 description = "Backpack API SDK tool"
 authors = ["sndmndss <yanfedorov120505@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage="https://backpack.exchange"
 repository="https://github.com/sndmndss/bpx-py/"
 keywords = ["api", "sdk", "backpack", "client", "wrapper"]
```

### Comparing `bpx_py-1.1.2/PKG-INFO` & `bpx_py-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpx-py
-Version: 1.1.2
+Version: 1.1.4
 Summary: Backpack API SDK tool
 Home-page: https://backpack.exchange
 License: Apache-2.0
 Keywords: api,sdk,backpack,client,wrapper
 Author: sndmndss
 Author-email: yanfedorov120505@gmail.com
 Requires-Python: >=3.8,<4.0
```

