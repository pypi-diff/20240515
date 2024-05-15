# Comparing `tmp/antchain_stlr-2.7.4.tar.gz` & `tmp/antchain_stlr-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.7.4.tar", last modified: Fri Apr 19 06:58:10 2024, max compression
+gzip compressed data, was "dist/antchain_stlr-2.8.1.tar", last modified: Wed May 15 10:03:41 2024, max compression
```

## Comparing `antchain_stlr-2.7.4.tar` & `antchain_stlr-2.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127505 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   307516 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 06:58:10.000000 antchain_stlr-2.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2024-04-19 06:58:09.000000 antchain_stlr-2.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158013 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   393543 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 10:03:41.000000 antchain_stlr-2.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-05-15 10:03:40.000000 antchain_stlr-2.8.1/setup.py
```

### Comparing `antchain_stlr-2.7.4/LICENSE` & `antchain_stlr-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.7.4/PKG-INFO` & `antchain_stlr-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.7.4
+Version: 2.8.1
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.7.4/README-CN.md` & `antchain_stlr-2.8.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.7.4/README.md` & `antchain_stlr-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.7.4/antchain_sdk_stlr/client.py` & `antchain_stlr-2.8.1/antchain_sdk_stlr/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 数据值条目
+            # 阶段评估明细数据
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.7.4',
+                    'sdk_version': '2.8.1',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -210,15 +210,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 数据值条目
+            # 阶段评估明细数据
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.7.4',
+                    'sdk_version': '2.8.1',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1447,14 +1447,686 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.QueryPdcpDataResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.pdcp.data.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def detail_pdcp_deposit(
+        self,
+        request: stlr_models.DetailPdcpDepositRequest,
+    ) -> stlr_models.DetailPdcpDepositResponse:
+        """
+        Description: 查询存证数据详情，包括存证内容、存证数据值、存证状态、存证交易等信息。 若指定版本，返回指定版本；若未指定，返回最新版本。
+        Summary: 查询存证数据详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_pdcp_deposit_ex(request, headers, runtime)
+
+    async def detail_pdcp_deposit_async(
+        self,
+        request: stlr_models.DetailPdcpDepositRequest,
+    ) -> stlr_models.DetailPdcpDepositResponse:
+        """
+        Description: 查询存证数据详情，包括存证内容、存证数据值、存证状态、存证交易等信息。 若指定版本，返回指定版本；若未指定，返回最新版本。
+        Summary: 查询存证数据详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_pdcp_deposit_ex_async(request, headers, runtime)
+
+    def detail_pdcp_deposit_ex(
+        self,
+        request: stlr_models.DetailPdcpDepositRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailPdcpDepositResponse:
+        """
+        Description: 查询存证数据详情，包括存证内容、存证数据值、存证状态、存证交易等信息。 若指定版本，返回指定版本；若未指定，返回最新版本。
+        Summary: 查询存证数据详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailPdcpDepositResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.deposit.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_pdcp_deposit_ex_async(
+        self,
+        request: stlr_models.DetailPdcpDepositRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.DetailPdcpDepositResponse:
+        """
+        Description: 查询存证数据详情，包括存证内容、存证数据值、存证状态、存证交易等信息。 若指定版本，返回指定版本；若未指定，返回最新版本。
+        Summary: 查询存证数据详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.DetailPdcpDepositResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.deposit.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_pdcp_dtrace(
+        self,
+        request: stlr_models.QueryPdcpDtraceRequest,
+    ) -> stlr_models.QueryPdcpDtraceResponse:
+        """
+        Description: 查询存证数据历史变更
+        Summary: 存证数据变更历史追溯查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_pdcp_dtrace_ex(request, headers, runtime)
+
+    async def query_pdcp_dtrace_async(
+        self,
+        request: stlr_models.QueryPdcpDtraceRequest,
+    ) -> stlr_models.QueryPdcpDtraceResponse:
+        """
+        Description: 查询存证数据历史变更
+        Summary: 存证数据变更历史追溯查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_pdcp_dtrace_ex_async(request, headers, runtime)
+
+    def query_pdcp_dtrace_ex(
+        self,
+        request: stlr_models.QueryPdcpDtraceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpDtraceResponse:
+        """
+        Description: 查询存证数据历史变更
+        Summary: 存证数据变更历史追溯查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpDtraceResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.dtrace.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_pdcp_dtrace_ex_async(
+        self,
+        request: stlr_models.QueryPdcpDtraceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpDtraceResponse:
+        """
+        Description: 查询存证数据历史变更
+        Summary: 存证数据变更历史追溯查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpDtraceResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.dtrace.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def check_pdcp_dtrace(
+        self,
+        request: stlr_models.CheckPdcpDtraceRequest,
+    ) -> stlr_models.CheckPdcpDtraceResponse:
+        """
+        Description: 通过链山存证内容校验存证数据可信性
+        Summary: 存证数据可信校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.check_pdcp_dtrace_ex(request, headers, runtime)
+
+    async def check_pdcp_dtrace_async(
+        self,
+        request: stlr_models.CheckPdcpDtraceRequest,
+    ) -> stlr_models.CheckPdcpDtraceResponse:
+        """
+        Description: 通过链山存证内容校验存证数据可信性
+        Summary: 存证数据可信校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.check_pdcp_dtrace_ex_async(request, headers, runtime)
+
+    def check_pdcp_dtrace_ex(
+        self,
+        request: stlr_models.CheckPdcpDtraceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.CheckPdcpDtraceResponse:
+        """
+        Description: 通过链山存证内容校验存证数据可信性
+        Summary: 存证数据可信校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.CheckPdcpDtraceResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.dtrace.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def check_pdcp_dtrace_ex_async(
+        self,
+        request: stlr_models.CheckPdcpDtraceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.CheckPdcpDtraceResponse:
+        """
+        Description: 通过链山存证内容校验存证数据可信性
+        Summary: 存证数据可信校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.CheckPdcpDtraceResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.dtrace.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def batchquery_pdcp_data(
+        self,
+        request: stlr_models.BatchqueryPdcpDataRequest,
+    ) -> stlr_models.BatchqueryPdcpDataResponse:
+        """
+        Description: 根据授权方和被授权方授权关系批量查询授权数据
+        Summary: 批量查询授权数据
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.batchquery_pdcp_data_ex(request, headers, runtime)
+
+    async def batchquery_pdcp_data_async(
+        self,
+        request: stlr_models.BatchqueryPdcpDataRequest,
+    ) -> stlr_models.BatchqueryPdcpDataResponse:
+        """
+        Description: 根据授权方和被授权方授权关系批量查询授权数据
+        Summary: 批量查询授权数据
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.batchquery_pdcp_data_ex_async(request, headers, runtime)
+
+    def batchquery_pdcp_data_ex(
+        self,
+        request: stlr_models.BatchqueryPdcpDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.BatchqueryPdcpDataResponse:
+        """
+        Description: 根据授权方和被授权方授权关系批量查询授权数据
+        Summary: 批量查询授权数据
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.BatchqueryPdcpDataResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.data.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def batchquery_pdcp_data_ex_async(
+        self,
+        request: stlr_models.BatchqueryPdcpDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.BatchqueryPdcpDataResponse:
+        """
+        Description: 根据授权方和被授权方授权关系批量查询授权数据
+        Summary: 批量查询授权数据
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.BatchqueryPdcpDataResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.data.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_pdcp_owndata(
+        self,
+        request: stlr_models.QueryPdcpOwndataRequest,
+    ) -> stlr_models.QueryPdcpOwndataResponse:
+        """
+        Description: 查询用户拥有的数据记录
+        Summary: 查询拥有的数据
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_pdcp_owndata_ex(request, headers, runtime)
+
+    async def query_pdcp_owndata_async(
+        self,
+        request: stlr_models.QueryPdcpOwndataRequest,
+    ) -> stlr_models.QueryPdcpOwndataResponse:
+        """
+        Description: 查询用户拥有的数据记录
+        Summary: 查询拥有的数据
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_pdcp_owndata_ex_async(request, headers, runtime)
+
+    def query_pdcp_owndata_ex(
+        self,
+        request: stlr_models.QueryPdcpOwndataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpOwndataResponse:
+        """
+        Description: 查询用户拥有的数据记录
+        Summary: 查询拥有的数据
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpOwndataResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.owndata.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_pdcp_owndata_ex_async(
+        self,
+        request: stlr_models.QueryPdcpOwndataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpOwndataResponse:
+        """
+        Description: 查询用户拥有的数据记录
+        Summary: 查询拥有的数据
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpOwndataResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.owndata.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_pdcp_dataasset(
+        self,
+        request: stlr_models.QueryPdcpDataassetRequest,
+    ) -> stlr_models.QueryPdcpDataassetResponse:
+        """
+        Description: 分页查询数据资产
+        Summary: 数据资产
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_pdcp_dataasset_ex(request, headers, runtime)
+
+    async def query_pdcp_dataasset_async(
+        self,
+        request: stlr_models.QueryPdcpDataassetRequest,
+    ) -> stlr_models.QueryPdcpDataassetResponse:
+        """
+        Description: 分页查询数据资产
+        Summary: 数据资产
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_pdcp_dataasset_ex_async(request, headers, runtime)
+
+    def query_pdcp_dataasset_ex(
+        self,
+        request: stlr_models.QueryPdcpDataassetRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpDataassetResponse:
+        """
+        Description: 分页查询数据资产
+        Summary: 数据资产
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpDataassetResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.dataasset.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_pdcp_dataasset_ex_async(
+        self,
+        request: stlr_models.QueryPdcpDataassetRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryPdcpDataassetResponse:
+        """
+        Description: 分页查询数据资产
+        Summary: 数据资产
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryPdcpDataassetResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.dataasset.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def register_pdcp_dataasset(
+        self,
+        request: stlr_models.RegisterPdcpDataassetRequest,
+    ) -> stlr_models.RegisterPdcpDataassetResponse:
+        """
+        Description: 注册数据资产
+        Summary: 注册数据资产
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.register_pdcp_dataasset_ex(request, headers, runtime)
+
+    async def register_pdcp_dataasset_async(
+        self,
+        request: stlr_models.RegisterPdcpDataassetRequest,
+    ) -> stlr_models.RegisterPdcpDataassetResponse:
+        """
+        Description: 注册数据资产
+        Summary: 注册数据资产
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.register_pdcp_dataasset_ex_async(request, headers, runtime)
+
+    def register_pdcp_dataasset_ex(
+        self,
+        request: stlr_models.RegisterPdcpDataassetRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.RegisterPdcpDataassetResponse:
+        """
+        Description: 注册数据资产
+        Summary: 注册数据资产
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.RegisterPdcpDataassetResponse(),
+            self.do_request('1.0', 'antchain.carbon.pdcp.dataasset.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def register_pdcp_dataasset_ex_async(
+        self,
+        request: stlr_models.RegisterPdcpDataassetRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.RegisterPdcpDataassetResponse:
+        """
+        Description: 注册数据资产
+        Summary: 注册数据资产
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.RegisterPdcpDataassetResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.pdcp.dataasset.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def add_auth_admin(
+        self,
+        request: stlr_models.AddAuthAdminRequest,
+    ) -> stlr_models.AddAuthAdminResponse:
+        """
+        Description: 添加数据授权策略
+        Summary: 添加数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.add_auth_admin_ex(request, headers, runtime)
+
+    async def add_auth_admin_async(
+        self,
+        request: stlr_models.AddAuthAdminRequest,
+    ) -> stlr_models.AddAuthAdminResponse:
+        """
+        Description: 添加数据授权策略
+        Summary: 添加数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.add_auth_admin_ex_async(request, headers, runtime)
+
+    def add_auth_admin_ex(
+        self,
+        request: stlr_models.AddAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddAuthAdminResponse:
+        """
+        Description: 添加数据授权策略
+        Summary: 添加数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddAuthAdminResponse(),
+            self.do_request('1.0', 'antchain.carbon.auth.admin.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def add_auth_admin_ex_async(
+        self,
+        request: stlr_models.AddAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddAuthAdminResponse:
+        """
+        Description: 添加数据授权策略
+        Summary: 添加数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddAuthAdminResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.auth.admin.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_auth_admin(
+        self,
+        request: stlr_models.PagequeryAuthAdminRequest,
+    ) -> stlr_models.PagequeryAuthAdminResponse:
+        """
+        Description: 分页查询数据授权策略
+        Summary: 分页查询数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_auth_admin_ex(request, headers, runtime)
+
+    async def pagequery_auth_admin_async(
+        self,
+        request: stlr_models.PagequeryAuthAdminRequest,
+    ) -> stlr_models.PagequeryAuthAdminResponse:
+        """
+        Description: 分页查询数据授权策略
+        Summary: 分页查询数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_auth_admin_ex_async(request, headers, runtime)
+
+    def pagequery_auth_admin_ex(
+        self,
+        request: stlr_models.PagequeryAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PagequeryAuthAdminResponse:
+        """
+        Description: 分页查询数据授权策略
+        Summary: 分页查询数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PagequeryAuthAdminResponse(),
+            self.do_request('1.0', 'antchain.carbon.auth.admin.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_auth_admin_ex_async(
+        self,
+        request: stlr_models.PagequeryAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PagequeryAuthAdminResponse:
+        """
+        Description: 分页查询数据授权策略
+        Summary: 分页查询数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PagequeryAuthAdminResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.auth.admin.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_auth_admin(
+        self,
+        request: stlr_models.QueryAuthAdminRequest,
+    ) -> stlr_models.QueryAuthAdminResponse:
+        """
+        Description: 查询数据授权策略
+        Summary: 查询数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_auth_admin_ex(request, headers, runtime)
+
+    async def query_auth_admin_async(
+        self,
+        request: stlr_models.QueryAuthAdminRequest,
+    ) -> stlr_models.QueryAuthAdminResponse:
+        """
+        Description: 查询数据授权策略
+        Summary: 查询数据授权策略
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_auth_admin_ex_async(request, headers, runtime)
+
+    def query_auth_admin_ex(
+        self,
+        request: stlr_models.QueryAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryAuthAdminResponse:
+        """
+        Description: 查询数据授权策略
+        Summary: 查询数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryAuthAdminResponse(),
+            self.do_request('1.0', 'antchain.carbon.auth.admin.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_auth_admin_ex_async(
+        self,
+        request: stlr_models.QueryAuthAdminRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryAuthAdminResponse:
+        """
+        Description: 查询数据授权策略
+        Summary: 查询数据授权策略
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryAuthAdminResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.auth.admin.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def add_dataasset_type(
+        self,
+        request: stlr_models.AddDataassetTypeRequest,
+    ) -> stlr_models.AddDataassetTypeResponse:
+        """
+        Description: 数据资产添加数据类型
+        Summary: 添加数据类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.add_dataasset_type_ex(request, headers, runtime)
+
+    async def add_dataasset_type_async(
+        self,
+        request: stlr_models.AddDataassetTypeRequest,
+    ) -> stlr_models.AddDataassetTypeResponse:
+        """
+        Description: 数据资产添加数据类型
+        Summary: 添加数据类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.add_dataasset_type_ex_async(request, headers, runtime)
+
+    def add_dataasset_type_ex(
+        self,
+        request: stlr_models.AddDataassetTypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddDataassetTypeResponse:
+        """
+        Description: 数据资产添加数据类型
+        Summary: 添加数据类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddDataassetTypeResponse(),
+            self.do_request('1.0', 'antchain.carbon.dataasset.type.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def add_dataasset_type_ex_async(
+        self,
+        request: stlr_models.AddDataassetTypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.AddDataassetTypeResponse:
+        """
+        Description: 数据资产添加数据类型
+        Summary: 添加数据类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.AddDataassetTypeResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.dataasset.type.add', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_dataasset_type(
+        self,
+        request: stlr_models.PagequeryDataassetTypeRequest,
+    ) -> stlr_models.PagequeryDataassetTypeResponse:
+        """
+        Description: 分页查询数据资产类型
+        Summary: 分页查询数据资产类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_dataasset_type_ex(request, headers, runtime)
+
+    async def pagequery_dataasset_type_async(
+        self,
+        request: stlr_models.PagequeryDataassetTypeRequest,
+    ) -> stlr_models.PagequeryDataassetTypeResponse:
+        """
+        Description: 分页查询数据资产类型
+        Summary: 分页查询数据资产类型
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_dataasset_type_ex_async(request, headers, runtime)
+
+    def pagequery_dataasset_type_ex(
+        self,
+        request: stlr_models.PagequeryDataassetTypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PagequeryDataassetTypeResponse:
+        """
+        Description: 分页查询数据资产类型
+        Summary: 分页查询数据资产类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PagequeryDataassetTypeResponse(),
+            self.do_request('1.0', 'antchain.carbon.dataasset.type.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_dataasset_type_ex_async(
+        self,
+        request: stlr_models.PagequeryDataassetTypeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PagequeryDataassetTypeResponse:
+        """
+        Description: 分页查询数据资产类型
+        Summary: 分页查询数据资产类型
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PagequeryDataassetTypeResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.dataasset.type.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def add_ecar_avitivedata(
         self,
         request: stlr_models.AddEcarAvitivedataRequest,
     ) -> stlr_models.AddEcarAvitivedataResponse:
         """
         Description: 新增排放活动数据
         Summary: 新增排放活动数据
@@ -2915,14 +3587,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.BatchcreateEcarGreencertificategenerationResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.greencertificategeneration.batchcreate', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def submit_ecar_lcacalc(
+        self,
+        request: stlr_models.SubmitEcarLcacalcRequest,
+    ) -> stlr_models.SubmitEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算请求提交
+        Summary: 产品碳足迹速算请求提交
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_ecar_lcacalc_ex(request, headers, runtime)
+
+    async def submit_ecar_lcacalc_async(
+        self,
+        request: stlr_models.SubmitEcarLcacalcRequest,
+    ) -> stlr_models.SubmitEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算请求提交
+        Summary: 产品碳足迹速算请求提交
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_ecar_lcacalc_ex_async(request, headers, runtime)
+
+    def submit_ecar_lcacalc_ex(
+        self,
+        request: stlr_models.SubmitEcarLcacalcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算请求提交
+        Summary: 产品碳足迹速算请求提交
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcacalcResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.lcacalc.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_ecar_lcacalc_ex_async(
+        self,
+        request: stlr_models.SubmitEcarLcacalcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.SubmitEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算请求提交
+        Summary: 产品碳足迹速算请求提交
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.SubmitEcarLcacalcResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.lcacalc.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_ecar_lcacalc(
+        self,
+        request: stlr_models.QueryEcarLcacalcRequest,
+    ) -> stlr_models.QueryEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算结果查询
+        Summary: 产品碳足迹速算结果查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_ecar_lcacalc_ex(request, headers, runtime)
+
+    async def query_ecar_lcacalc_async(
+        self,
+        request: stlr_models.QueryEcarLcacalcRequest,
+    ) -> stlr_models.QueryEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算结果查询
+        Summary: 产品碳足迹速算结果查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_ecar_lcacalc_ex_async(request, headers, runtime)
+
+    def query_ecar_lcacalc_ex(
+        self,
+        request: stlr_models.QueryEcarLcacalcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算结果查询
+        Summary: 产品碳足迹速算结果查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarLcacalcResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.lcacalc.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_ecar_lcacalc_ex_async(
+        self,
+        request: stlr_models.QueryEcarLcacalcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.QueryEcarLcacalcResponse:
+        """
+        Description: 产品碳足迹速算结果查询
+        Summary: 产品碳足迹速算结果查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.QueryEcarLcacalcResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.lcacalc.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.7.4/antchain_sdk_stlr/models.py` & `antchain_stlr-2.8.1/antchain_sdk_stlr/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,14 +150,273 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
+class EnterpriseLcaAssessmentItem(TeaModel):
+    def __init__(
+        self,
+        material_code: str = None,
+        assessment_item_name: str = None,
+        emission_amount: str = None,
+        transport_emission_amount: str = None,
+    ):
+        # 物料编码
+        self.material_code = material_code
+        # 数据明细名称
+        self.assessment_item_name = assessment_item_name
+        # 物料直接碳排放评估量
+        self.emission_amount = emission_amount
+        # 物料运输碳排放评估量
+        self.transport_emission_amount = transport_emission_amount
+
+    def validate(self):
+        self.validate_required(self.material_code, 'material_code')
+        self.validate_required(self.assessment_item_name, 'assessment_item_name')
+        self.validate_required(self.emission_amount, 'emission_amount')
+        self.validate_required(self.transport_emission_amount, 'transport_emission_amount')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.material_code is not None:
+            result['material_code'] = self.material_code
+        if self.assessment_item_name is not None:
+            result['assessment_item_name'] = self.assessment_item_name
+        if self.emission_amount is not None:
+            result['emission_amount'] = self.emission_amount
+        if self.transport_emission_amount is not None:
+            result['transport_emission_amount'] = self.transport_emission_amount
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('material_code') is not None:
+            self.material_code = m.get('material_code')
+        if m.get('assessment_item_name') is not None:
+            self.assessment_item_name = m.get('assessment_item_name')
+        if m.get('emission_amount') is not None:
+            self.emission_amount = m.get('emission_amount')
+        if m.get('transport_emission_amount') is not None:
+            self.transport_emission_amount = m.get('transport_emission_amount')
+        return self
+
+
+class TransportActiveData(TeaModel):
+    def __init__(
+        self,
+        transport_code: str = None,
+        equipment: str = None,
+        distance: str = None,
+        is_empty_load: bool = None,
+    ):
+        # 运输方式编码
+        self.transport_code = transport_code
+        # 运输设备
+        self.equipment = equipment
+        # 运输里程
+        self.distance = distance
+        # 是否空载
+        self.is_empty_load = is_empty_load
+
+    def validate(self):
+        self.validate_required(self.transport_code, 'transport_code')
+        self.validate_required(self.equipment, 'equipment')
+        self.validate_required(self.distance, 'distance')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.transport_code is not None:
+            result['transport_code'] = self.transport_code
+        if self.equipment is not None:
+            result['equipment'] = self.equipment
+        if self.distance is not None:
+            result['distance'] = self.distance
+        if self.is_empty_load is not None:
+            result['is_empty_load'] = self.is_empty_load
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('transport_code') is not None:
+            self.transport_code = m.get('transport_code')
+        if m.get('equipment') is not None:
+            self.equipment = m.get('equipment')
+        if m.get('distance') is not None:
+            self.distance = m.get('distance')
+        if m.get('is_empty_load') is not None:
+            self.is_empty_load = m.get('is_empty_load')
+        return self
+
+
+class EnterpriseLcaStageAssessmentItem(TeaModel):
+    def __init__(
+        self,
+        lca_stage: str = None,
+        lca_stage_carbon_rate: str = None,
+        lca_stage_carbon_emissions: str = None,
+        lca_assessment_datum: List[EnterpriseLcaAssessmentItem] = None,
+    ):
+        # LCA阶段
+        self.lca_stage = lca_stage
+        # 阶段排放占比
+        self.lca_stage_carbon_rate = lca_stage_carbon_rate
+        # 阶段排放量
+        self.lca_stage_carbon_emissions = lca_stage_carbon_emissions
+        # 阶段评估明细数据
+        self.lca_assessment_datum = lca_assessment_datum
+
+    def validate(self):
+        self.validate_required(self.lca_stage, 'lca_stage')
+        self.validate_required(self.lca_stage_carbon_rate, 'lca_stage_carbon_rate')
+        self.validate_required(self.lca_stage_carbon_emissions, 'lca_stage_carbon_emissions')
+        self.validate_required(self.lca_assessment_datum, 'lca_assessment_datum')
+        if self.lca_assessment_datum:
+            for k in self.lca_assessment_datum:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.lca_stage is not None:
+            result['lca_stage'] = self.lca_stage
+        if self.lca_stage_carbon_rate is not None:
+            result['lca_stage_carbon_rate'] = self.lca_stage_carbon_rate
+        if self.lca_stage_carbon_emissions is not None:
+            result['lca_stage_carbon_emissions'] = self.lca_stage_carbon_emissions
+        result['lca_assessment_datum'] = []
+        if self.lca_assessment_datum is not None:
+            for k in self.lca_assessment_datum:
+                result['lca_assessment_datum'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('lca_stage') is not None:
+            self.lca_stage = m.get('lca_stage')
+        if m.get('lca_stage_carbon_rate') is not None:
+            self.lca_stage_carbon_rate = m.get('lca_stage_carbon_rate')
+        if m.get('lca_stage_carbon_emissions') is not None:
+            self.lca_stage_carbon_emissions = m.get('lca_stage_carbon_emissions')
+        self.lca_assessment_datum = []
+        if m.get('lca_assessment_datum') is not None:
+            for k in m.get('lca_assessment_datum'):
+                temp_model = EnterpriseLcaAssessmentItem()
+                self.lca_assessment_datum.append(temp_model.from_map(k))
+        return self
+
+
+class DepositFieldValue(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        value: str = None,
+    ):
+        # 存证数据字段名
+        self.name = name
+        # 存证数据字段值
+        self.value = value
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class InputStreamActiveData(TeaModel):
+    def __init__(
+        self,
+        material_code: str = None,
+        amount: str = None,
+        unit: str = None,
+        transport_list: List[TransportActiveData] = None,
+    ):
+        # 物料编码
+        self.material_code = material_code
+        # 用量，非负，最多6位小数
+        self.amount = amount
+        # 单位
+        self.unit = unit
+        # 运输信息列表
+        self.transport_list = transport_list
+
+    def validate(self):
+        self.validate_required(self.material_code, 'material_code')
+        self.validate_required(self.amount, 'amount')
+        self.validate_required(self.unit, 'unit')
+        if self.transport_list:
+            for k in self.transport_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.material_code is not None:
+            result['material_code'] = self.material_code
+        if self.amount is not None:
+            result['amount'] = self.amount
+        if self.unit is not None:
+            result['unit'] = self.unit
+        result['transport_list'] = []
+        if self.transport_list is not None:
+            for k in self.transport_list:
+                result['transport_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('material_code') is not None:
+            self.material_code = m.get('material_code')
+        if m.get('amount') is not None:
+            self.amount = m.get('amount')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
+        self.transport_list = []
+        if m.get('transport_list') is not None:
+            for k in m.get('transport_list'):
+                temp_model = TransportActiveData()
+                self.transport_list.append(temp_model.from_map(k))
+        return self
+
+
 class AnyAmountItem(TeaModel):
     def __init__(
         self,
         item_code: str = None,
         item_amount: str = None,
     ):
         # 数据项编码
@@ -275,14 +534,88 @@
         if m.get('lca_stage_code') is not None:
             self.lca_stage_code = m.get('lca_stage_code')
         if m.get('lca_stage_carbon_amount') is not None:
             self.lca_stage_carbon_amount = m.get('lca_stage_carbon_amount')
         return self
 
 
+class OutputStreamActiveData(TeaModel):
+    def __init__(
+        self,
+        material_code: str = None,
+        amount: str = None,
+        unit: str = None,
+        unit_price: str = None,
+        disposal_type_code: str = None,
+        transport_list: List[TransportActiveData] = None,
+    ):
+        # 物料编码
+        self.material_code = material_code
+        # 用量，非负，最多6位小数
+        self.amount = amount
+        # 单位
+        self.unit = unit
+        # 单价（仅产品用，产品不传时默认为空）
+        self.unit_price = unit_price
+        # 处置方式编码（仅废弃物用）
+        self.disposal_type_code = disposal_type_code
+        # 运输信息列表（仅废弃物用）
+        self.transport_list = transport_list
+
+    def validate(self):
+        self.validate_required(self.material_code, 'material_code')
+        self.validate_required(self.amount, 'amount')
+        self.validate_required(self.unit, 'unit')
+        if self.transport_list:
+            for k in self.transport_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.material_code is not None:
+            result['material_code'] = self.material_code
+        if self.amount is not None:
+            result['amount'] = self.amount
+        if self.unit is not None:
+            result['unit'] = self.unit
+        if self.unit_price is not None:
+            result['unit_price'] = self.unit_price
+        if self.disposal_type_code is not None:
+            result['disposal_type_code'] = self.disposal_type_code
+        result['transport_list'] = []
+        if self.transport_list is not None:
+            for k in self.transport_list:
+                result['transport_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('material_code') is not None:
+            self.material_code = m.get('material_code')
+        if m.get('amount') is not None:
+            self.amount = m.get('amount')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
+        if m.get('unit_price') is not None:
+            self.unit_price = m.get('unit_price')
+        if m.get('disposal_type_code') is not None:
+            self.disposal_type_code = m.get('disposal_type_code')
+        self.transport_list = []
+        if m.get('transport_list') is not None:
+            for k in m.get('transport_list'):
+                temp_model = TransportActiveData()
+                self.transport_list.append(temp_model.from_map(k))
+        return self
+
+
 class EnterpriseDocumentFile(TeaModel):
     def __init__(
         self,
         document_name: str = None,
         document_address: str = None,
     ):
         # 文档名称
@@ -542,14 +875,82 @@
         if m.get('auth_products') is not None:
             for k in m.get('auth_products'):
                 temp_model = CertProductAuthDO()
                 self.auth_products.append(temp_model.from_map(k))
         return self
 
 
+class LcaCalcResult(TeaModel):
+    def __init__(
+        self,
+        record_no: str = None,
+        carbon_amount: str = None,
+        lca_stage_assessment_datum: List[EnterpriseLcaStageAssessmentItem] = None,
+        record_date: str = None,
+        custom_context: str = None,
+    ):
+        # 速算记录编号
+        self.record_no = record_no
+        # 碳足迹排放量
+        self.carbon_amount = carbon_amount
+        # 各阶段评估数据明细
+        self.lca_stage_assessment_datum = lca_stage_assessment_datum
+        # 速算发起时间
+        self.record_date = record_date
+        # 自定义业务标识
+        self.custom_context = custom_context
+
+    def validate(self):
+        self.validate_required(self.record_no, 'record_no')
+        self.validate_required(self.carbon_amount, 'carbon_amount')
+        self.validate_required(self.lca_stage_assessment_datum, 'lca_stage_assessment_datum')
+        if self.lca_stage_assessment_datum:
+            for k in self.lca_stage_assessment_datum:
+                if k:
+                    k.validate()
+        self.validate_required(self.record_date, 'record_date')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.record_no is not None:
+            result['record_no'] = self.record_no
+        if self.carbon_amount is not None:
+            result['carbon_amount'] = self.carbon_amount
+        result['lca_stage_assessment_datum'] = []
+        if self.lca_stage_assessment_datum is not None:
+            for k in self.lca_stage_assessment_datum:
+                result['lca_stage_assessment_datum'].append(k.to_map() if k else None)
+        if self.record_date is not None:
+            result['record_date'] = self.record_date
+        if self.custom_context is not None:
+            result['custom_context'] = self.custom_context
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('record_no') is not None:
+            self.record_no = m.get('record_no')
+        if m.get('carbon_amount') is not None:
+            self.carbon_amount = m.get('carbon_amount')
+        self.lca_stage_assessment_datum = []
+        if m.get('lca_stage_assessment_datum') is not None:
+            for k in m.get('lca_stage_assessment_datum'):
+                temp_model = EnterpriseLcaStageAssessmentItem()
+                self.lca_stage_assessment_datum.append(temp_model.from_map(k))
+        if m.get('record_date') is not None:
+            self.record_date = m.get('record_date')
+        if m.get('custom_context') is not None:
+            self.custom_context = m.get('custom_context')
+        return self
+
+
 class AnnualMonthEmissionDatum(TeaModel):
     def __init__(
         self,
         year: str = None,
         month: str = None,
         value: str = None,
     ):
@@ -734,14 +1135,66 @@
         if m.get('date') is not None:
             self.date = m.get('date')
         if m.get('value') is not None:
             self.value = m.get('value')
         return self
 
 
+class DataAssetInfo(TeaModel):
+    def __init__(
+        self,
+        dataset_did: str = None,
+        user_did: str = None,
+        dataset_name: str = None,
+        data_type: str = None,
+    ):
+        # 数据资产DID
+        self.dataset_did = dataset_did
+        # 数据资产所有方DID
+        self.user_did = user_did
+        # 数据资产名称
+        self.dataset_name = dataset_name
+        # 数据类型
+        self.data_type = data_type
+
+    def validate(self):
+        self.validate_required(self.dataset_did, 'dataset_did')
+        self.validate_required(self.user_did, 'user_did')
+        self.validate_required(self.dataset_name, 'dataset_name')
+        self.validate_required(self.data_type, 'data_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_did is not None:
+            result['dataset_did'] = self.dataset_did
+        if self.user_did is not None:
+            result['user_did'] = self.user_did
+        if self.dataset_name is not None:
+            result['dataset_name'] = self.dataset_name
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('dataset_did') is not None:
+            self.dataset_did = m.get('dataset_did')
+        if m.get('user_did') is not None:
+            self.user_did = m.get('user_did')
+        if m.get('dataset_name') is not None:
+            self.dataset_name = m.get('dataset_name')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        return self
+
+
 class EmissionCounteractionStatistics(TeaModel):
     def __init__(
         self,
         assert_type: str = None,
         assert_type_name: str = None,
         counteraction_amount: str = None,
         data_unit: str = None,
@@ -895,14 +1348,90 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('user_did') is not None:
             self.user_did = m.get('user_did')
         return self
 
 
+class DataDepositInfo(TeaModel):
+    def __init__(
+        self,
+        data_value: List[DepositFieldValue] = None,
+        tx_id: str = None,
+        user_id: str = None,
+        deposit_content: str = None,
+        status: str = None,
+        timestamp: int = None,
+    ):
+        # 存证字段值
+        self.data_value = data_value
+        # 数据存证区块链交易ID
+        self.tx_id = tx_id
+        # 数据存证操作用户ID
+        self.user_id = user_id
+        # 存证数据内容
+        self.deposit_content = deposit_content
+        # 存证执行状态
+        self.status = status
+        # 存证执行(发起)时间
+        self.timestamp = timestamp
+
+    def validate(self):
+        self.validate_required(self.data_value, 'data_value')
+        if self.data_value:
+            for k in self.data_value:
+                if k:
+                    k.validate()
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.deposit_content, 'deposit_content')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.timestamp, 'timestamp')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['data_value'] = []
+        if self.data_value is not None:
+            for k in self.data_value:
+                result['data_value'].append(k.to_map() if k else None)
+        if self.tx_id is not None:
+            result['tx_id'] = self.tx_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.deposit_content is not None:
+            result['deposit_content'] = self.deposit_content
+        if self.status is not None:
+            result['status'] = self.status
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data_value = []
+        if m.get('data_value') is not None:
+            for k in m.get('data_value'):
+                temp_model = DepositFieldValue()
+                self.data_value.append(temp_model.from_map(k))
+        if m.get('tx_id') is not None:
+            self.tx_id = m.get('tx_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('deposit_content') is not None:
+            self.deposit_content = m.get('deposit_content')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        return self
+
+
 class CarbonOffsetAcquisitionItem(TeaModel):
     def __init__(
         self,
         acquisition_item_no: str = None,
         project_no: str = None,
         account_did: str = None,
         occurrent_time: str = None,
@@ -1332,14 +1861,66 @@
         if m.get('item_code') is not None:
             self.item_code = m.get('item_code')
         if m.get('item_value') is not None:
             self.item_value = m.get('item_value')
         return self
 
 
+class DataTypeInfo(TeaModel):
+    def __init__(
+        self,
+        data_type_no: str = None,
+        data_type_name: str = None,
+        data_type_config: str = None,
+        data_json_schema: str = None,
+    ):
+        # 数据类型编码
+        self.data_type_no = data_type_no
+        # 数据类型名称
+        self.data_type_name = data_type_name
+        # 数据类型配置
+        self.data_type_config = data_type_config
+        # 数据JSON格式检查
+        self.data_json_schema = data_json_schema
+
+    def validate(self):
+        self.validate_required(self.data_type_no, 'data_type_no')
+        self.validate_required(self.data_type_name, 'data_type_name')
+        self.validate_required(self.data_type_config, 'data_type_config')
+        self.validate_required(self.data_json_schema, 'data_json_schema')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_type_no is not None:
+            result['data_type_no'] = self.data_type_no
+        if self.data_type_name is not None:
+            result['data_type_name'] = self.data_type_name
+        if self.data_type_config is not None:
+            result['data_type_config'] = self.data_type_config
+        if self.data_json_schema is not None:
+            result['data_json_schema'] = self.data_json_schema
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data_type_no') is not None:
+            self.data_type_no = m.get('data_type_no')
+        if m.get('data_type_name') is not None:
+            self.data_type_name = m.get('data_type_name')
+        if m.get('data_type_config') is not None:
+            self.data_type_config = m.get('data_type_config')
+        if m.get('data_json_schema') is not None:
+            self.data_json_schema = m.get('data_json_schema')
+        return self
+
+
 class LcaCarbonDatum(TeaModel):
     def __init__(
         self,
         lca_carbon_amount: str = None,
         lca_report_file_url: str = None,
         lca_detail_file_url: str = None,
         life_cycle_boundary: str = None,
@@ -1417,14 +1998,58 @@
         if m.get('lca_stage_carbon_datum') is not None:
             for k in m.get('lca_stage_carbon_datum'):
                 temp_model = LcaStageCarbonItem()
                 self.lca_stage_carbon_datum.append(temp_model.from_map(k))
         return self
 
 
+class AuthorizePolicy(TeaModel):
+    def __init__(
+        self,
+        policy_id: str = None,
+        description: str = None,
+        authorize_config: str = None,
+    ):
+        # 授权策略ID
+        self.policy_id = policy_id
+        # 授权策略描述
+        self.description = description
+        # 授权策略配置
+        self.authorize_config = authorize_config
+
+    def validate(self):
+        self.validate_required(self.policy_id, 'policy_id')
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.authorize_config, 'authorize_config')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_id is not None:
+            result['policy_id'] = self.policy_id
+        if self.description is not None:
+            result['description'] = self.description
+        if self.authorize_config is not None:
+            result['authorize_config'] = self.authorize_config
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('policy_id') is not None:
+            self.policy_id = m.get('policy_id')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('authorize_config') is not None:
+            self.authorize_config = m.get('authorize_config')
+        return self
+
+
 class EnterpriseProductOutline(TeaModel):
     def __init__(
         self,
         enterprise_custom_code: str = None,
         product_name: str = None,
         specification: str = None,
         product_description: str = None,
@@ -1847,14 +2472,76 @@
         if m.get('category_emissions_list') is not None:
             for k in m.get('category_emissions_list'):
                 temp_model = EmissionsCategoryStatistics()
                 self.category_emissions_list.append(temp_model.from_map(k))
         return self
 
 
+class LcaStageActiveData(TeaModel):
+    def __init__(
+        self,
+        lca_stage: str = None,
+        input_stream_list: List[InputStreamActiveData] = None,
+        output_stream_list: List[OutputStreamActiveData] = None,
+    ):
+        # LCA阶段
+        self.lca_stage = lca_stage
+        # 输入流活动数据列表
+        self.input_stream_list = input_stream_list
+        # 输出流活动数据列表
+        self.output_stream_list = output_stream_list
+
+    def validate(self):
+        self.validate_required(self.lca_stage, 'lca_stage')
+        self.validate_required(self.input_stream_list, 'input_stream_list')
+        if self.input_stream_list:
+            for k in self.input_stream_list:
+                if k:
+                    k.validate()
+        self.validate_required(self.output_stream_list, 'output_stream_list')
+        if self.output_stream_list:
+            for k in self.output_stream_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.lca_stage is not None:
+            result['lca_stage'] = self.lca_stage
+        result['input_stream_list'] = []
+        if self.input_stream_list is not None:
+            for k in self.input_stream_list:
+                result['input_stream_list'].append(k.to_map() if k else None)
+        result['output_stream_list'] = []
+        if self.output_stream_list is not None:
+            for k in self.output_stream_list:
+                result['output_stream_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('lca_stage') is not None:
+            self.lca_stage = m.get('lca_stage')
+        self.input_stream_list = []
+        if m.get('input_stream_list') is not None:
+            for k in m.get('input_stream_list'):
+                temp_model = InputStreamActiveData()
+                self.input_stream_list.append(temp_model.from_map(k))
+        self.output_stream_list = []
+        if m.get('output_stream_list') is not None:
+            for k in m.get('output_stream_list'):
+                temp_model = OutputStreamActiveData()
+                self.output_stream_list.append(temp_model.from_map(k))
+        return self
+
+
 class GreenOperationStatisticsByFrequence(TeaModel):
     def __init__(
         self,
         occurrence_period: str = None,
         green_energy_amount: int = None,
         green_operation_records: int = None,
     ):
@@ -4481,14 +5168,1457 @@
         if m.get('page_size') is not None:
             self.page_size = m.get('page_size')
         if m.get('data_list') is not None:
             self.data_list = m.get('data_list')
         return self
 
 
+class DetailPdcpDepositRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type: str = None,
+        data_id: str = None,
+        tx_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 数据类型名称，用户标识记录的数据类型。
+        self.data_type = data_type
+        # 存证数据ID，存证数据唯一标识ID。
+        self.data_id = data_id
+        # 数据存证区块链交易ID，对应数据版本号。 若未指定，返回最近的版本。
+        self.tx_id = tx_id
+
+    def validate(self):
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.data_id, 'data_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        if self.tx_id is not None:
+            result['tx_id'] = self.tx_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        if m.get('tx_id') is not None:
+            self.tx_id = m.get('tx_id')
+        return self
+
+
+class DetailPdcpDepositResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data_type: str = None,
+        data_id: str = None,
+        deposit_data: DataDepositInfo = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 存证数据类型
+        self.data_type = data_type
+        # 存证数据唯一ID
+        self.data_id = data_id
+        # 存证数据内容
+        self.deposit_data = deposit_data
+
+    def validate(self):
+        if self.deposit_data:
+            self.deposit_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        if self.deposit_data is not None:
+            result['deposit_data'] = self.deposit_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        if m.get('deposit_data') is not None:
+            temp_model = DataDepositInfo()
+            self.deposit_data = temp_model.from_map(m['deposit_data'])
+        return self
+
+
+class QueryPdcpDtraceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type: str = None,
+        data_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 存证数据类型名称
+        self.data_type = data_type
+        # 存证数据ID
+        self.data_id = data_id
+
+    def validate(self):
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.data_id, 'data_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        return self
+
+
+class QueryPdcpDtraceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data_type: str = None,
+        data_id: str = None,
+        versions: List[DataDepositInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 存证数据类型名称
+        self.data_type = data_type
+        # 存证数据ID
+        self.data_id = data_id
+        # 存证数据版本列表
+        self.versions = versions
+
+    def validate(self):
+        if self.versions:
+            for k in self.versions:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        result['versions'] = []
+        if self.versions is not None:
+            for k in self.versions:
+                result['versions'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        self.versions = []
+        if m.get('versions') is not None:
+            for k in m.get('versions'):
+                temp_model = DataDepositInfo()
+                self.versions.append(temp_model.from_map(k))
+        return self
+
+
+class CheckPdcpDtraceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type: str = None,
+        data_id: str = None,
+        tx_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 存证数据类型名称
+        self.data_type = data_type
+        # 存证数据ID
+        self.data_id = data_id
+        # 存证操作区块链交易ID，即存证数据版本号。若未指定，检查当前最新版本。
+        self.tx_id = tx_id
+
+    def validate(self):
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.data_id, 'data_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_id is not None:
+            result['data_id'] = self.data_id
+        if self.tx_id is not None:
+            result['tx_id'] = self.tx_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_id') is not None:
+            self.data_id = m.get('data_id')
+        if m.get('tx_id') is not None:
+            self.tx_id = m.get('tx_id')
+        return self
+
+
+class CheckPdcpDtraceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        deposit_data: DataDepositInfo = None,
+        block_number: int = None,
+        deposit_type: str = None,
+        on_chain_data: str = None,
+        off_chain_data: str = None,
+        consistent: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 存证操作内容
+        self.deposit_data = deposit_data
+        # 区块链编号
+        self.block_number = block_number
+        # 数据存证方式
+        self.deposit_type = deposit_type
+        # 链上数据
+        self.on_chain_data = on_chain_data
+        # 链下数据
+        self.off_chain_data = off_chain_data
+        # 链上-链下数据是否一致
+        self.consistent = consistent
+
+    def validate(self):
+        if self.deposit_data:
+            self.deposit_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.deposit_data is not None:
+            result['deposit_data'] = self.deposit_data.to_map()
+        if self.block_number is not None:
+            result['block_number'] = self.block_number
+        if self.deposit_type is not None:
+            result['deposit_type'] = self.deposit_type
+        if self.on_chain_data is not None:
+            result['on_chain_data'] = self.on_chain_data
+        if self.off_chain_data is not None:
+            result['off_chain_data'] = self.off_chain_data
+        if self.consistent is not None:
+            result['consistent'] = self.consistent
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('deposit_data') is not None:
+            temp_model = DataDepositInfo()
+            self.deposit_data = temp_model.from_map(m['deposit_data'])
+        if m.get('block_number') is not None:
+            self.block_number = m.get('block_number')
+        if m.get('deposit_type') is not None:
+            self.deposit_type = m.get('deposit_type')
+        if m.get('on_chain_data') is not None:
+            self.on_chain_data = m.get('on_chain_data')
+        if m.get('off_chain_data') is not None:
+            self.off_chain_data = m.get('off_chain_data')
+        if m.get('consistent') is not None:
+            self.consistent = m.get('consistent')
+        return self
+
+
+class BatchqueryPdcpDataRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type: str = None,
+        authorizer_did: str = None,
+        authorized_did: str = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务数据类型，查询该数据类型的授权数据
+        self.data_type = data_type
+        # 授权方身份ID，若指定查询该用户授权的数据
+        self.authorizer_did = authorizer_did
+        # 被授权方身份ID，若指定查询授权给该用户的数据
+        self.authorized_did = authorized_did
+        # 当前页面，默认1
+        self.page_number = page_number
+        # 分页大小，默认20
+        self.page_size = page_size
+
+    def validate(self):
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.page_number, 'page_number')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.authorizer_did is not None:
+            result['authorizer_did'] = self.authorizer_did
+        if self.authorized_did is not None:
+            result['authorized_did'] = self.authorized_did
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('authorizer_did') is not None:
+            self.authorizer_did = m.get('authorizer_did')
+        if m.get('authorized_did') is not None:
+            self.authorized_did = m.get('authorized_did')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class BatchqueryPdcpDataResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total: int = None,
+        page_number: int = None,
+        page_size: int = None,
+        data_list: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 总记录条数
+        self.total = total
+        # 当前页面
+        self.page_number = page_number
+        # 分页大小
+        self.page_size = page_size
+        # 数据列表
+        self.data_list = data_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.total is not None:
+            result['total'] = self.total
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.data_list is not None:
+            result['data_list'] = self.data_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('data_list') is not None:
+            self.data_list = m.get('data_list')
+        return self
+
+
+class QueryPdcpOwndataRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type: str = None,
+        user_did: str = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务数据类型
+        self.data_type = data_type
+        # 拥有数据的用户
+        self.user_did = user_did
+        # 当前分页，默认1
+        self.page_number = page_number
+        # 分页大小，默认20
+        self.page_size = page_size
+
+    def validate(self):
+        self.validate_required(self.data_type, 'data_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.user_did is not None:
+            result['user_did'] = self.user_did
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('user_did') is not None:
+            self.user_did = m.get('user_did')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class QueryPdcpOwndataResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total: int = None,
+        page_number: int = None,
+        page_size: int = None,
+        data_list: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 总记录条数
+        self.total = total
+        # 当前分页
+        self.page_number = page_number
+        # 分页大小
+        self.page_size = page_size
+        # 数据记录列表
+        self.data_list = data_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.total is not None:
+            result['total'] = self.total
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.data_list is not None:
+            result['data_list'] = self.data_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('data_list') is not None:
+            self.data_list = m.get('data_list')
+        return self
+
+
+class QueryPdcpDataassetRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        data_type_no: str = None,
+        user_did: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 当前页码，默认1
+        self.page_number = page_number
+        # 页面大小，默认20
+        self.page_size = page_size
+        # 数据类型
+        self.data_type_no = data_type_no
+        # 数据资产所有者
+        self.user_did = user_did
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.data_type_no is not None:
+            result['data_type_no'] = self.data_type_no
+        if self.user_did is not None:
+            result['user_did'] = self.user_did
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('data_type_no') is not None:
+            self.data_type_no = m.get('data_type_no')
+        if m.get('user_did') is not None:
+            self.user_did = m.get('user_did')
+        return self
+
+
+class QueryPdcpDataassetResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total: int = None,
+        page_number: int = None,
+        page_size: int = None,
+        data_asset_list: List[DataAssetInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 总量
+        self.total = total
+        # 当前页面
+        self.page_number = page_number
+        # 页面大小
+        self.page_size = page_size
+        # 数据资产信息
+        self.data_asset_list = data_asset_list
+
+    def validate(self):
+        if self.data_asset_list:
+            for k in self.data_asset_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.total is not None:
+            result['total'] = self.total
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        result['data_asset_list'] = []
+        if self.data_asset_list is not None:
+            for k in self.data_asset_list:
+                result['data_asset_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        self.data_asset_list = []
+        if m.get('data_asset_list') is not None:
+            for k in m.get('data_asset_list'):
+                temp_model = DataAssetInfo()
+                self.data_asset_list.append(temp_model.from_map(k))
+        return self
+
+
+class RegisterPdcpDataassetRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type_no: str = None,
+        user_did: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 数据类型编码
+        self.data_type_no = data_type_no
+        # 数据资产所有者id
+        self.user_did = user_did
+
+    def validate(self):
+        self.validate_required(self.data_type_no, 'data_type_no')
+        self.validate_required(self.user_did, 'user_did')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type_no is not None:
+            result['data_type_no'] = self.data_type_no
+        if self.user_did is not None:
+            result['user_did'] = self.user_did
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type_no') is not None:
+            self.data_type_no = m.get('data_type_no')
+        if m.get('user_did') is not None:
+            self.user_did = m.get('user_did')
+        return self
+
+
+class RegisterPdcpDataassetResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        dataset_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 资产id
+        self.dataset_id = dataset_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.dataset_id is not None:
+            result['dataset_id'] = self.dataset_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('dataset_id') is not None:
+            self.dataset_id = m.get('dataset_id')
+        return self
+
+
+class AddAuthAdminRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        policy_id: str = None,
+        description: str = None,
+        authorize_config: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 授权策略ID
+        self.policy_id = policy_id
+        # 授权策略描述
+        self.description = description
+        # 授权策略配置
+        self.authorize_config = authorize_config
+
+    def validate(self):
+        self.validate_required(self.policy_id, 'policy_id')
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.authorize_config, 'authorize_config')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.policy_id is not None:
+            result['policy_id'] = self.policy_id
+        if self.description is not None:
+            result['description'] = self.description
+        if self.authorize_config is not None:
+            result['authorize_config'] = self.authorize_config
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('policy_id') is not None:
+            self.policy_id = m.get('policy_id')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('authorize_config') is not None:
+            self.authorize_config = m.get('authorize_config')
+        return self
+
+
+class AddAuthAdminResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class PagequeryAuthAdminRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 当前查询页数
+        self.page_number = page_number
+        # 每页记录条数，默认为20
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class PagequeryAuthAdminResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        authorize_policy_list: List[AuthorizePolicy] = None,
+        total: int = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 授权策略配置
+        self.authorize_policy_list = authorize_policy_list
+        # 总数量
+        self.total = total
+        # 当前页
+        self.page_number = page_number
+        # 每页条数
+        self.page_size = page_size
+
+    def validate(self):
+        if self.authorize_policy_list:
+            for k in self.authorize_policy_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['authorize_policy_list'] = []
+        if self.authorize_policy_list is not None:
+            for k in self.authorize_policy_list:
+                result['authorize_policy_list'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['total'] = self.total
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.authorize_policy_list = []
+        if m.get('authorize_policy_list') is not None:
+            for k in m.get('authorize_policy_list'):
+                temp_model = AuthorizePolicy()
+                self.authorize_policy_list.append(temp_model.from_map(k))
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class QueryAuthAdminRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        policy_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 数据授权策略ID
+        self.policy_id = policy_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.policy_id is not None:
+            result['policy_id'] = self.policy_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('policy_id') is not None:
+            self.policy_id = m.get('policy_id')
+        return self
+
+
+class QueryAuthAdminResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: AuthorizePolicy = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 授权策略
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('data') is not None:
+            temp_model = AuthorizePolicy()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class AddDataassetTypeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        data_type_no: str = None,
+        data_type_name: str = None,
+        data_type_config: str = None,
+        data_json_schema: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 数据类型编码
+        self.data_type_no = data_type_no
+        # 数据类型名称
+        self.data_type_name = data_type_name
+        # 数据类型配置
+        self.data_type_config = data_type_config
+        # 数据JSON格式检查
+        self.data_json_schema = data_json_schema
+
+    def validate(self):
+        self.validate_required(self.data_type_no, 'data_type_no')
+        self.validate_required(self.data_type_name, 'data_type_name')
+        self.validate_required(self.data_type_config, 'data_type_config')
+        self.validate_required(self.data_json_schema, 'data_json_schema')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.data_type_no is not None:
+            result['data_type_no'] = self.data_type_no
+        if self.data_type_name is not None:
+            result['data_type_name'] = self.data_type_name
+        if self.data_type_config is not None:
+            result['data_type_config'] = self.data_type_config
+        if self.data_json_schema is not None:
+            result['data_json_schema'] = self.data_json_schema
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('data_type_no') is not None:
+            self.data_type_no = m.get('data_type_no')
+        if m.get('data_type_name') is not None:
+            self.data_type_name = m.get('data_type_name')
+        if m.get('data_type_config') is not None:
+            self.data_type_config = m.get('data_type_config')
+        if m.get('data_json_schema') is not None:
+            self.data_json_schema = m.get('data_json_schema')
+        return self
+
+
+class AddDataassetTypeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class PagequeryDataassetTypeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 当前查询页数
+        self.page_number = page_number
+        # 每页记录条数，默认为20
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class PagequeryDataassetTypeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data_type_info: List[DataTypeInfo] = None,
+        total: int = None,
+        page_number: int = None,
+        page_size: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # DataTypeInfo
+        self.data_type_info = data_type_info
+        # 总数量
+        self.total = total
+        # 1
+        self.page_number = page_number
+        # pageSize
+        self.page_size = page_size
+
+    def validate(self):
+        if self.data_type_info:
+            for k in self.data_type_info:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['data_type_info'] = []
+        if self.data_type_info is not None:
+            for k in self.data_type_info:
+                result['data_type_info'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['total'] = self.total
+        if self.page_number is not None:
+            result['page_number'] = self.page_number
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.data_type_info = []
+        if m.get('data_type_info') is not None:
+            for k in m.get('data_type_info'):
+                temp_model = DataTypeInfo()
+                self.data_type_info.append(temp_model.from_map(k))
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('page_number') is not None:
+            self.page_number = m.get('page_number')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
 class AddEcarAvitivedataRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         enterprise_biz_no: str = None,
         inventory_item_no: str = None,
@@ -7870,14 +10000,321 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class SubmitEcarLcacalcRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        material_code: str = None,
+        process_no: str = None,
+        life_cycle_boundary: str = None,
+        functional_unit: str = None,
+        functional_amount: str = None,
+        stage_active_data_list: List[LcaStageActiveData] = None,
+        custom_context: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 目标产品编码
+        self.material_code = material_code
+        # 授权过程编码
+        self.process_no = process_no
+        # 生命周期边界
+        self.life_cycle_boundary = life_cycle_boundary
+        # 产品功能单位
+        self.functional_unit = functional_unit
+        # 功能单位数量
+        self.functional_amount = functional_amount
+        # 各阶段活动数据
+        self.stage_active_data_list = stage_active_data_list
+        # 自定义业务标识
+        self.custom_context = custom_context
+
+    def validate(self):
+        self.validate_required(self.material_code, 'material_code')
+        self.validate_required(self.process_no, 'process_no')
+        self.validate_required(self.life_cycle_boundary, 'life_cycle_boundary')
+        self.validate_required(self.functional_unit, 'functional_unit')
+        self.validate_required(self.functional_amount, 'functional_amount')
+        self.validate_required(self.stage_active_data_list, 'stage_active_data_list')
+        if self.stage_active_data_list:
+            for k in self.stage_active_data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.material_code is not None:
+            result['material_code'] = self.material_code
+        if self.process_no is not None:
+            result['process_no'] = self.process_no
+        if self.life_cycle_boundary is not None:
+            result['life_cycle_boundary'] = self.life_cycle_boundary
+        if self.functional_unit is not None:
+            result['functional_unit'] = self.functional_unit
+        if self.functional_amount is not None:
+            result['functional_amount'] = self.functional_amount
+        result['stage_active_data_list'] = []
+        if self.stage_active_data_list is not None:
+            for k in self.stage_active_data_list:
+                result['stage_active_data_list'].append(k.to_map() if k else None)
+        if self.custom_context is not None:
+            result['custom_context'] = self.custom_context
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('material_code') is not None:
+            self.material_code = m.get('material_code')
+        if m.get('process_no') is not None:
+            self.process_no = m.get('process_no')
+        if m.get('life_cycle_boundary') is not None:
+            self.life_cycle_boundary = m.get('life_cycle_boundary')
+        if m.get('functional_unit') is not None:
+            self.functional_unit = m.get('functional_unit')
+        if m.get('functional_amount') is not None:
+            self.functional_amount = m.get('functional_amount')
+        self.stage_active_data_list = []
+        if m.get('stage_active_data_list') is not None:
+            for k in m.get('stage_active_data_list'):
+                temp_model = LcaStageActiveData()
+                self.stage_active_data_list.append(temp_model.from_map(k))
+        if m.get('custom_context') is not None:
+            self.custom_context = m.get('custom_context')
+        return self
+
+
+class SubmitEcarLcacalcResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        record_no: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 速算记录编号
+        self.record_no = record_no
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.record_no is not None:
+            result['record_no'] = self.record_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('record_no') is not None:
+            self.record_no = m.get('record_no')
+        return self
+
+
+class QueryEcarLcacalcRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        record_no_list: List[str] = None,
+        start_date: str = None,
+        end_date: str = None,
+        current: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 速算记录编号列表
+        self.record_no_list = record_no_list
+        # 开始日期，yyyy-MM-dd
+        self.start_date = start_date
+        # 结束日期，yyyy-MM-dd
+        self.end_date = end_date
+        # 分页查询页码，从1开始，不传时默认为1
+        self.current = current
+        # 每页记录条数，取值范围[10, 200]，不传时默认为20
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.record_no_list is not None:
+            result['record_no_list'] = self.record_no_list
+        if self.start_date is not None:
+            result['start_date'] = self.start_date
+        if self.end_date is not None:
+            result['end_date'] = self.end_date
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('record_no_list') is not None:
+            self.record_no_list = m.get('record_no_list')
+        if m.get('start_date') is not None:
+            self.start_date = m.get('start_date')
+        if m.get('end_date') is not None:
+            self.end_date = m.get('end_date')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class QueryEcarLcacalcResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        start_date: str = None,
+        end_date: str = None,
+        list: List[LcaCalcResult] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 当前查询页码
+        self.current = current
+        # 每页记录条数
+        self.page_size = page_size
+        # 记录总条数
+        self.total = total
+        # 开始日期
+        self.start_date = start_date
+        # 结束日期
+        self.end_date = end_date
+        # Lca速算记录列表
+        self.list = list
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        if self.start_date is not None:
+            result['start_date'] = self.start_date
+        if self.end_date is not None:
+            result['end_date'] = self.end_date
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        if m.get('start_date') is not None:
+            self.start_date = m.get('start_date')
+        if m.get('end_date') is not None:
+            self.end_date = m.get('end_date')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = LcaCalcResult()
+                self.list.append(temp_model.from_map(k))
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.7.4/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.8.1/antchain_stlr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.7.4
+Version: 2.8.1
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.7.4/setup.py` & `antchain_stlr-2.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 19/04/2024
+Created on 15/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

