# Comparing `tmp/alibabacloud_dm20151123-1.1.0.tar.gz` & `tmp/alibabacloud_dm20151123-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20151123-1.1.0.tar", last modified: Mon Apr 22 17:14:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dm20151123-1.1.1.tar", last modified: Wed May 15 02:02:23 2024, max compression
```

## Comparing `alibabacloud_dm20151123-1.1.0.tar` & `alibabacloud_dm20151123-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1669 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164700 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/client.py
--rw-r--r--   0 root         (0) root         (0)   245558 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-22 17:14:05.000000 alibabacloud_dm20151123-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198476 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/client.py
+-rw-r--r--   0 root         (0) root         (0)   247209 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-15 02:02:23.000000 alibabacloud_dm20151123-1.1.1/setup.py
```

### Comparing `alibabacloud_dm20151123-1.1.0/ChangeLog.md` & `alibabacloud_dm20151123-1.1.1/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+2024-04-22 Version: 1.1.0
+- Support API CreateUserSuppression.
+- Support API GetSuppressionListLevel.
+- Support API ListUserSuppression.
+- Support API RemoveUserSuppression.
+- Support API SetSuppressionListLevel.
+- Update API BatchSendMail: add param UnSubscribeFilterLevel.
+- Update API BatchSendMail: add param UnSubscribeLinkType.
+- Update API SenderStatisticsDetailByParam: update response param.
+- Update API SingleSendMail: add param UnSubscribeFilterLevel.
+- Update API SingleSendMail: add param UnSubscribeLinkType.
+
+
 2024-03-13 Version: 1.0.12
 - Update API BatchSendMail: add param UnSubscribeFilterLevel.
 - Update API BatchSendMail: add param UnSubscribeLinkType.
 - Update API SenderStatisticsDetailByParam: update response param.
 - Update API SingleSendMail: add param UnSubscribeFilterLevel.
 - Update API SingleSendMail: add param UnSubscribeLinkType.
```

### Comparing `alibabacloud_dm20151123-1.1.0/LICENSE` & `alibabacloud_dm20151123-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.0/PKG-INFO` & `alibabacloud_dm20151123-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20151123
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.0/README-CN.md` & `alibabacloud_dm20151123-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.0/README.md` & `alibabacloud_dm20151123-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/client.py` & `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_ipfilter_with_options(
         self,
         request: dm_20151123_models.AddIpfilterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.AddIpfilterResponse:
+        """
+        @summary 添加IP防护信息
+        
+        @param request: AddIpfilterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddIpfilterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_address):
             query['IpAddress'] = request.ip_address
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -76,14 +83,21 @@
         )
 
     async def add_ipfilter_with_options_async(
         self,
         request: dm_20151123_models.AddIpfilterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.AddIpfilterResponse:
+        """
+        @summary 添加IP防护信息
+        
+        @param request: AddIpfilterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddIpfilterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_address):
             query['IpAddress'] = request.ip_address
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -109,29 +123,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_ipfilter(
         self,
         request: dm_20151123_models.AddIpfilterRequest,
     ) -> dm_20151123_models.AddIpfilterResponse:
+        """
+        @summary 添加IP防护信息
+        
+        @param request: AddIpfilterRequest
+        @return: AddIpfilterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_ipfilter_with_options(request, runtime)
 
     async def add_ipfilter_async(
         self,
         request: dm_20151123_models.AddIpfilterRequest,
     ) -> dm_20151123_models.AddIpfilterResponse:
+        """
+        @summary 添加IP防护信息
+        
+        @param request: AddIpfilterRequest
+        @return: AddIpfilterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_ipfilter_with_options_async(request, runtime)
 
     def approve_reply_mail_address_with_options(
         self,
         request: dm_20151123_models.ApproveReplyMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ApproveReplyMailAddressResponse:
+        """
+        @summary 验证回信地址
+        
+        @param request: ApproveReplyMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ApproveReplyMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -158,14 +191,21 @@
         )
 
     async def approve_reply_mail_address_with_options_async(
         self,
         request: dm_20151123_models.ApproveReplyMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ApproveReplyMailAddressResponse:
+        """
+        @summary 验证回信地址
+        
+        @param request: ApproveReplyMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ApproveReplyMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -191,29 +231,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def approve_reply_mail_address(
         self,
         request: dm_20151123_models.ApproveReplyMailAddressRequest,
     ) -> dm_20151123_models.ApproveReplyMailAddressResponse:
+        """
+        @summary 验证回信地址
+        
+        @param request: ApproveReplyMailAddressRequest
+        @return: ApproveReplyMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.approve_reply_mail_address_with_options(request, runtime)
 
     async def approve_reply_mail_address_async(
         self,
         request: dm_20151123_models.ApproveReplyMailAddressRequest,
     ) -> dm_20151123_models.ApproveReplyMailAddressResponse:
+        """
+        @summary 验证回信地址
+        
+        @param request: ApproveReplyMailAddressRequest
+        @return: ApproveReplyMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.approve_reply_mail_address_with_options_async(request, runtime)
 
     def batch_send_mail_with_options(
         self,
         request: dm_20151123_models.BatchSendMailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.BatchSendMailResponse:
+        """
+        @summary 批量发送邮件
+        
+        @param request: BatchSendMailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchSendMailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.click_trace):
@@ -258,14 +317,21 @@
         )
 
     async def batch_send_mail_with_options_async(
         self,
         request: dm_20151123_models.BatchSendMailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.BatchSendMailResponse:
+        """
+        @summary 批量发送邮件
+        
+        @param request: BatchSendMailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchSendMailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.click_trace):
@@ -309,29 +375,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def batch_send_mail(
         self,
         request: dm_20151123_models.BatchSendMailRequest,
     ) -> dm_20151123_models.BatchSendMailResponse:
+        """
+        @summary 批量发送邮件
+        
+        @param request: BatchSendMailRequest
+        @return: BatchSendMailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.batch_send_mail_with_options(request, runtime)
 
     async def batch_send_mail_async(
         self,
         request: dm_20151123_models.BatchSendMailRequest,
     ) -> dm_20151123_models.BatchSendMailResponse:
+        """
+        @summary 批量发送邮件
+        
+        @param request: BatchSendMailRequest
+        @return: BatchSendMailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.batch_send_mail_with_options_async(request, runtime)
 
     def check_domain_with_options(
         self,
         request: dm_20151123_models.CheckDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CheckDomainResponse:
+        """
+        @summary 校验域名状态
+        
+        @param request: CheckDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -358,14 +443,21 @@
         )
 
     async def check_domain_with_options_async(
         self,
         request: dm_20151123_models.CheckDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CheckDomainResponse:
+        """
+        @summary 校验域名状态
+        
+        @param request: CheckDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -391,29 +483,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_domain(
         self,
         request: dm_20151123_models.CheckDomainRequest,
     ) -> dm_20151123_models.CheckDomainResponse:
+        """
+        @summary 校验域名状态
+        
+        @param request: CheckDomainRequest
+        @return: CheckDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_domain_with_options(request, runtime)
 
     async def check_domain_async(
         self,
         request: dm_20151123_models.CheckDomainRequest,
     ) -> dm_20151123_models.CheckDomainResponse:
+        """
+        @summary 校验域名状态
+        
+        @param request: CheckDomainRequest
+        @return: CheckDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_domain_with_options_async(request, runtime)
 
     def check_reply_to_mail_address_with_options(
         self,
         request: dm_20151123_models.CheckReplyToMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CheckReplyToMailAddressResponse:
+        """
+        @summary 校验回信地址
+        
+        @param request: CheckReplyToMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckReplyToMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
@@ -444,14 +555,21 @@
         )
 
     async def check_reply_to_mail_address_with_options_async(
         self,
         request: dm_20151123_models.CheckReplyToMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CheckReplyToMailAddressResponse:
+        """
+        @summary 校验回信地址
+        
+        @param request: CheckReplyToMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckReplyToMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
@@ -481,29 +599,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_reply_to_mail_address(
         self,
         request: dm_20151123_models.CheckReplyToMailAddressRequest,
     ) -> dm_20151123_models.CheckReplyToMailAddressResponse:
+        """
+        @summary 校验回信地址
+        
+        @param request: CheckReplyToMailAddressRequest
+        @return: CheckReplyToMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_reply_to_mail_address_with_options(request, runtime)
 
     async def check_reply_to_mail_address_async(
         self,
         request: dm_20151123_models.CheckReplyToMailAddressRequest,
     ) -> dm_20151123_models.CheckReplyToMailAddressResponse:
+        """
+        @summary 校验回信地址
+        
+        @param request: CheckReplyToMailAddressRequest
+        @return: CheckReplyToMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_reply_to_mail_address_with_options_async(request, runtime)
 
     def create_domain_with_options(
         self,
         request: dm_20151123_models.CreateDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateDomainResponse:
+        """
+        @summary 创建域名
+        
+        @param request: CreateDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -530,14 +667,21 @@
         )
 
     async def create_domain_with_options_async(
         self,
         request: dm_20151123_models.CreateDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateDomainResponse:
+        """
+        @summary 创建域名
+        
+        @param request: CreateDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -563,29 +707,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_domain(
         self,
         request: dm_20151123_models.CreateDomainRequest,
     ) -> dm_20151123_models.CreateDomainResponse:
+        """
+        @summary 创建域名
+        
+        @param request: CreateDomainRequest
+        @return: CreateDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_domain_with_options(request, runtime)
 
     async def create_domain_async(
         self,
         request: dm_20151123_models.CreateDomainRequest,
     ) -> dm_20151123_models.CreateDomainResponse:
+        """
+        @summary 创建域名
+        
+        @param request: CreateDomainRequest
+        @return: CreateDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_domain_with_options_async(request, runtime)
 
     def create_mail_address_with_options(
         self,
         request: dm_20151123_models.CreateMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateMailAddressResponse:
+        """
+        @param request: CreateMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.reply_address):
@@ -616,14 +777,19 @@
         )
 
     async def create_mail_address_with_options_async(
         self,
         request: dm_20151123_models.CreateMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateMailAddressResponse:
+        """
+        @param request: CreateMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.reply_address):
@@ -653,29 +819,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mail_address(
         self,
         request: dm_20151123_models.CreateMailAddressRequest,
     ) -> dm_20151123_models.CreateMailAddressResponse:
+        """
+        @param request: CreateMailAddressRequest
+        @return: CreateMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mail_address_with_options(request, runtime)
 
     async def create_mail_address_async(
         self,
         request: dm_20151123_models.CreateMailAddressRequest,
     ) -> dm_20151123_models.CreateMailAddressResponse:
+        """
+        @param request: CreateMailAddressRequest
+        @return: CreateMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mail_address_with_options_async(request, runtime)
 
     def create_receiver_with_options(
         self,
         request: dm_20151123_models.CreateReceiverRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateReceiverResponse:
+        """
+        @summary 创建收件人列表
+        
+        @param request: CreateReceiverRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateReceiverResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desc):
             query['Desc'] = request.desc
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receivers_alias):
@@ -706,14 +887,21 @@
         )
 
     async def create_receiver_with_options_async(
         self,
         request: dm_20151123_models.CreateReceiverRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateReceiverResponse:
+        """
+        @summary 创建收件人列表
+        
+        @param request: CreateReceiverRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateReceiverResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.desc):
             query['Desc'] = request.desc
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receivers_alias):
@@ -743,29 +931,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_receiver(
         self,
         request: dm_20151123_models.CreateReceiverRequest,
     ) -> dm_20151123_models.CreateReceiverResponse:
+        """
+        @summary 创建收件人列表
+        
+        @param request: CreateReceiverRequest
+        @return: CreateReceiverResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_receiver_with_options(request, runtime)
 
     async def create_receiver_async(
         self,
         request: dm_20151123_models.CreateReceiverRequest,
     ) -> dm_20151123_models.CreateReceiverResponse:
+        """
+        @summary 创建收件人列表
+        
+        @param request: CreateReceiverRequest
+        @return: CreateReceiverResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_receiver_with_options_async(request, runtime)
 
     def create_tag_with_options(
         self,
         request: dm_20151123_models.CreateTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateTagResponse:
+        """
+        @summary 创建标签
+        
+        @param request: CreateTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -794,14 +1001,21 @@
         )
 
     async def create_tag_with_options_async(
         self,
         request: dm_20151123_models.CreateTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateTagResponse:
+        """
+        @summary 创建标签
+        
+        @param request: CreateTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -829,29 +1043,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_tag(
         self,
         request: dm_20151123_models.CreateTagRequest,
     ) -> dm_20151123_models.CreateTagResponse:
+        """
+        @summary 创建标签
+        
+        @param request: CreateTagRequest
+        @return: CreateTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_tag_with_options(request, runtime)
 
     async def create_tag_async(
         self,
         request: dm_20151123_models.CreateTagRequest,
     ) -> dm_20151123_models.CreateTagResponse:
+        """
+        @summary 创建标签
+        
+        @param request: CreateTagRequest
+        @return: CreateTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_tag_with_options_async(request, runtime)
 
     def create_user_suppression_with_options(
         self,
         request: dm_20151123_models.CreateUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateUserSuppressionResponse:
+        """
+        @summary 创建用户无效地址
+        
+        @param request: CreateUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -878,14 +1111,21 @@
         )
 
     async def create_user_suppression_with_options_async(
         self,
         request: dm_20151123_models.CreateUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.CreateUserSuppressionResponse:
+        """
+        @summary 创建用户无效地址
+        
+        @param request: CreateUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -911,29 +1151,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_user_suppression(
         self,
         request: dm_20151123_models.CreateUserSuppressionRequest,
     ) -> dm_20151123_models.CreateUserSuppressionResponse:
+        """
+        @summary 创建用户无效地址
+        
+        @param request: CreateUserSuppressionRequest
+        @return: CreateUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_user_suppression_with_options(request, runtime)
 
     async def create_user_suppression_async(
         self,
         request: dm_20151123_models.CreateUserSuppressionRequest,
     ) -> dm_20151123_models.CreateUserSuppressionResponse:
+        """
+        @summary 创建用户无效地址
+        
+        @param request: CreateUserSuppressionRequest
+        @return: CreateUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_suppression_with_options_async(request, runtime)
 
     def delete_domain_with_options(
         self,
         request: dm_20151123_models.DeleteDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteDomainResponse:
+        """
+        @summary 删除域名
+        
+        @param request: DeleteDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -960,14 +1219,21 @@
         )
 
     async def delete_domain_with_options_async(
         self,
         request: dm_20151123_models.DeleteDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteDomainResponse:
+        """
+        @summary 删除域名
+        
+        @param request: DeleteDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -993,29 +1259,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_domain(
         self,
         request: dm_20151123_models.DeleteDomainRequest,
     ) -> dm_20151123_models.DeleteDomainResponse:
+        """
+        @summary 删除域名
+        
+        @param request: DeleteDomainRequest
+        @return: DeleteDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_domain_with_options(request, runtime)
 
     async def delete_domain_async(
         self,
         request: dm_20151123_models.DeleteDomainRequest,
     ) -> dm_20151123_models.DeleteDomainResponse:
+        """
+        @summary 删除域名
+        
+        @param request: DeleteDomainRequest
+        @return: DeleteDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_domain_with_options_async(request, runtime)
 
     def delete_invalid_address_with_options(
         self,
         request: dm_20151123_models.DeleteInvalidAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        """
+        @summary 从无效地址库删除无效地址
+        
+        @param request: DeleteInvalidAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteInvalidAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1042,14 +1327,21 @@
         )
 
     async def delete_invalid_address_with_options_async(
         self,
         request: dm_20151123_models.DeleteInvalidAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        """
+        @summary 从无效地址库删除无效地址
+        
+        @param request: DeleteInvalidAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteInvalidAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1075,29 +1367,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_invalid_address(
         self,
         request: dm_20151123_models.DeleteInvalidAddressRequest,
     ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        """
+        @summary 从无效地址库删除无效地址
+        
+        @param request: DeleteInvalidAddressRequest
+        @return: DeleteInvalidAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_invalid_address_with_options(request, runtime)
 
     async def delete_invalid_address_async(
         self,
         request: dm_20151123_models.DeleteInvalidAddressRequest,
     ) -> dm_20151123_models.DeleteInvalidAddressResponse:
+        """
+        @summary 从无效地址库删除无效地址
+        
+        @param request: DeleteInvalidAddressRequest
+        @return: DeleteInvalidAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_invalid_address_with_options_async(request, runtime)
 
     def delete_ipfilter_by_edm_id_with_options(
         self,
         request: dm_20151123_models.DeleteIpfilterByEdmIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteIpfilterByEdmIdResponse:
+        """
+        @summary 删除IP保护信息
+        
+        @param request: DeleteIpfilterByEdmIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIpfilterByEdmIdResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.from_type):
             query['FromType'] = request.from_type
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.owner_id):
@@ -1126,14 +1437,21 @@
         )
 
     async def delete_ipfilter_by_edm_id_with_options_async(
         self,
         request: dm_20151123_models.DeleteIpfilterByEdmIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteIpfilterByEdmIdResponse:
+        """
+        @summary 删除IP保护信息
+        
+        @param request: DeleteIpfilterByEdmIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIpfilterByEdmIdResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.from_type):
             query['FromType'] = request.from_type
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.owner_id):
@@ -1161,29 +1479,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_ipfilter_by_edm_id(
         self,
         request: dm_20151123_models.DeleteIpfilterByEdmIdRequest,
     ) -> dm_20151123_models.DeleteIpfilterByEdmIdResponse:
+        """
+        @summary 删除IP保护信息
+        
+        @param request: DeleteIpfilterByEdmIdRequest
+        @return: DeleteIpfilterByEdmIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_ipfilter_by_edm_id_with_options(request, runtime)
 
     async def delete_ipfilter_by_edm_id_async(
         self,
         request: dm_20151123_models.DeleteIpfilterByEdmIdRequest,
     ) -> dm_20151123_models.DeleteIpfilterByEdmIdResponse:
+        """
+        @summary 删除IP保护信息
+        
+        @param request: DeleteIpfilterByEdmIdRequest
+        @return: DeleteIpfilterByEdmIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_ipfilter_by_edm_id_with_options_async(request, runtime)
 
     def delete_mail_address_with_options(
         self,
         request: dm_20151123_models.DeleteMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteMailAddressResponse:
+        """
+        @summary 删除发信地址
+        
+        @param request: DeleteMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -1210,14 +1547,21 @@
         )
 
     async def delete_mail_address_with_options_async(
         self,
         request: dm_20151123_models.DeleteMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteMailAddressResponse:
+        """
+        @summary 删除发信地址
+        
+        @param request: DeleteMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -1243,29 +1587,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mail_address(
         self,
         request: dm_20151123_models.DeleteMailAddressRequest,
     ) -> dm_20151123_models.DeleteMailAddressResponse:
+        """
+        @summary 删除发信地址
+        
+        @param request: DeleteMailAddressRequest
+        @return: DeleteMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mail_address_with_options(request, runtime)
 
     async def delete_mail_address_async(
         self,
         request: dm_20151123_models.DeleteMailAddressRequest,
     ) -> dm_20151123_models.DeleteMailAddressResponse:
+        """
+        @summary 删除发信地址
+        
+        @param request: DeleteMailAddressRequest
+        @return: DeleteMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mail_address_with_options_async(request, runtime)
 
     def delete_receiver_with_options(
         self,
         request: dm_20151123_models.DeleteReceiverRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteReceiverResponse:
+        """
+        @summary 删除收件人列表
+        
+        @param request: DeleteReceiverRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteReceiverResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
             query['ReceiverId'] = request.receiver_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -1292,14 +1655,21 @@
         )
 
     async def delete_receiver_with_options_async(
         self,
         request: dm_20151123_models.DeleteReceiverRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteReceiverResponse:
+        """
+        @summary 删除收件人列表
+        
+        @param request: DeleteReceiverRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteReceiverResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
             query['ReceiverId'] = request.receiver_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -1325,29 +1695,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_receiver(
         self,
         request: dm_20151123_models.DeleteReceiverRequest,
     ) -> dm_20151123_models.DeleteReceiverResponse:
+        """
+        @summary 删除收件人列表
+        
+        @param request: DeleteReceiverRequest
+        @return: DeleteReceiverResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_receiver_with_options(request, runtime)
 
     async def delete_receiver_async(
         self,
         request: dm_20151123_models.DeleteReceiverRequest,
     ) -> dm_20151123_models.DeleteReceiverResponse:
+        """
+        @summary 删除收件人列表
+        
+        @param request: DeleteReceiverRequest
+        @return: DeleteReceiverResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_receiver_with_options_async(request, runtime)
 
     def delete_receiver_detail_with_options(
         self,
         request: dm_20151123_models.DeleteReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteReceiverDetailResponse:
+        """
+        @summary 删除单个收件人
+        
+        @param request: DeleteReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.email):
             query['Email'] = request.email
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
@@ -1376,14 +1765,21 @@
         )
 
     async def delete_receiver_detail_with_options_async(
         self,
         request: dm_20151123_models.DeleteReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteReceiverDetailResponse:
+        """
+        @summary 删除单个收件人
+        
+        @param request: DeleteReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.email):
             query['Email'] = request.email
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
@@ -1411,29 +1807,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_receiver_detail(
         self,
         request: dm_20151123_models.DeleteReceiverDetailRequest,
     ) -> dm_20151123_models.DeleteReceiverDetailResponse:
+        """
+        @summary 删除单个收件人
+        
+        @param request: DeleteReceiverDetailRequest
+        @return: DeleteReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_receiver_detail_with_options(request, runtime)
 
     async def delete_receiver_detail_async(
         self,
         request: dm_20151123_models.DeleteReceiverDetailRequest,
     ) -> dm_20151123_models.DeleteReceiverDetailResponse:
+        """
+        @summary 删除单个收件人
+        
+        @param request: DeleteReceiverDetailRequest
+        @return: DeleteReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_receiver_detail_with_options_async(request, runtime)
 
     def delete_tag_with_options(
         self,
         request: dm_20151123_models.DeleteTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteTagResponse:
+        """
+        @summary 删除标签
+        
+        @param request: DeleteTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1460,14 +1875,21 @@
         )
 
     async def delete_tag_with_options_async(
         self,
         request: dm_20151123_models.DeleteTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DeleteTagResponse:
+        """
+        @summary 删除标签
+        
+        @param request: DeleteTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1493,29 +1915,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_tag(
         self,
         request: dm_20151123_models.DeleteTagRequest,
     ) -> dm_20151123_models.DeleteTagResponse:
+        """
+        @summary 删除标签
+        
+        @param request: DeleteTagRequest
+        @return: DeleteTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_tag_with_options(request, runtime)
 
     async def delete_tag_async(
         self,
         request: dm_20151123_models.DeleteTagRequest,
     ) -> dm_20151123_models.DeleteTagResponse:
+        """
+        @summary 删除标签
+        
+        @param request: DeleteTagRequest
+        @return: DeleteTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_tag_with_options_async(request, runtime)
 
     def desc_account_summary_with_options(
         self,
         request: dm_20151123_models.DescAccountSummaryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DescAccountSummaryResponse:
+        """
+        @param request: DescAccountSummaryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescAccountSummaryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1540,14 +1979,19 @@
         )
 
     async def desc_account_summary_with_options_async(
         self,
         request: dm_20151123_models.DescAccountSummaryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DescAccountSummaryResponse:
+        """
+        @param request: DescAccountSummaryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescAccountSummaryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1571,29 +2015,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def desc_account_summary(
         self,
         request: dm_20151123_models.DescAccountSummaryRequest,
     ) -> dm_20151123_models.DescAccountSummaryResponse:
+        """
+        @param request: DescAccountSummaryRequest
+        @return: DescAccountSummaryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.desc_account_summary_with_options(request, runtime)
 
     async def desc_account_summary_async(
         self,
         request: dm_20151123_models.DescAccountSummaryRequest,
     ) -> dm_20151123_models.DescAccountSummaryResponse:
+        """
+        @param request: DescAccountSummaryRequest
+        @return: DescAccountSummaryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.desc_account_summary_with_options_async(request, runtime)
 
     def desc_domain_with_options(
         self,
         request: dm_20151123_models.DescDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DescDomainResponse:
+        """
+        @summary 获取域名详情
+        
+        @param request: DescDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.require_real_time_dns_records):
@@ -1622,14 +2081,21 @@
         )
 
     async def desc_domain_with_options_async(
         self,
         request: dm_20151123_models.DescDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.DescDomainResponse:
+        """
+        @summary 获取域名详情
+        
+        @param request: DescDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_id):
             query['DomainId'] = request.domain_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.require_real_time_dns_records):
@@ -1657,29 +2123,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def desc_domain(
         self,
         request: dm_20151123_models.DescDomainRequest,
     ) -> dm_20151123_models.DescDomainResponse:
+        """
+        @summary 获取域名详情
+        
+        @param request: DescDomainRequest
+        @return: DescDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.desc_domain_with_options(request, runtime)
 
     async def desc_domain_async(
         self,
         request: dm_20151123_models.DescDomainRequest,
     ) -> dm_20151123_models.DescDomainResponse:
+        """
+        @summary 获取域名详情
+        
+        @param request: DescDomainRequest
+        @return: DescDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.desc_domain_with_options_async(request, runtime)
 
     def get_ip_protection_with_options(
         self,
         request: dm_20151123_models.GetIpProtectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetIpProtectionResponse:
+        """
+        @summary 获取IP保护信息
+        
+        @param request: GetIpProtectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIpProtectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1704,14 +2189,21 @@
         )
 
     async def get_ip_protection_with_options_async(
         self,
         request: dm_20151123_models.GetIpProtectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetIpProtectionResponse:
+        """
+        @summary 获取IP保护信息
+        
+        @param request: GetIpProtectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIpProtectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1735,29 +2227,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ip_protection(
         self,
         request: dm_20151123_models.GetIpProtectionRequest,
     ) -> dm_20151123_models.GetIpProtectionResponse:
+        """
+        @summary 获取IP保护信息
+        
+        @param request: GetIpProtectionRequest
+        @return: GetIpProtectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ip_protection_with_options(request, runtime)
 
     async def get_ip_protection_async(
         self,
         request: dm_20151123_models.GetIpProtectionRequest,
     ) -> dm_20151123_models.GetIpProtectionResponse:
+        """
+        @summary 获取IP保护信息
+        
+        @param request: GetIpProtectionRequest
+        @return: GetIpProtectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ip_protection_with_options_async(request, runtime)
 
     def get_ipfilter_list_with_options(
         self,
         request: dm_20151123_models.GetIpfilterListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetIpfilterListResponse:
+        """
+        @summary 获取IP防护信息
+        
+        @param request: GetIpfilterListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIpfilterListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1782,14 +2293,21 @@
         )
 
     async def get_ipfilter_list_with_options_async(
         self,
         request: dm_20151123_models.GetIpfilterListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetIpfilterListResponse:
+        """
+        @summary 获取IP防护信息
+        
+        @param request: GetIpfilterListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIpfilterListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1813,29 +2331,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ipfilter_list(
         self,
         request: dm_20151123_models.GetIpfilterListRequest,
     ) -> dm_20151123_models.GetIpfilterListResponse:
+        """
+        @summary 获取IP防护信息
+        
+        @param request: GetIpfilterListRequest
+        @return: GetIpfilterListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ipfilter_list_with_options(request, runtime)
 
     async def get_ipfilter_list_async(
         self,
         request: dm_20151123_models.GetIpfilterListRequest,
     ) -> dm_20151123_models.GetIpfilterListResponse:
+        """
+        @summary 获取IP防护信息
+        
+        @param request: GetIpfilterListRequest
+        @return: GetIpfilterListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ipfilter_list_with_options_async(request, runtime)
 
     def get_suppression_list_level_with_options(
         self,
         request: dm_20151123_models.GetSuppressionListLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetSuppressionListLevelResponse:
+        """
+        @summary 获取用户无效地址级别配置
+        
+        @param request: GetSuppressionListLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSuppressionListLevelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1860,14 +2397,21 @@
         )
 
     async def get_suppression_list_level_with_options_async(
         self,
         request: dm_20151123_models.GetSuppressionListLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetSuppressionListLevelResponse:
+        """
+        @summary 获取用户无效地址级别配置
+        
+        @param request: GetSuppressionListLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSuppressionListLevelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -1891,29 +2435,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_suppression_list_level(
         self,
         request: dm_20151123_models.GetSuppressionListLevelRequest,
     ) -> dm_20151123_models.GetSuppressionListLevelResponse:
+        """
+        @summary 获取用户无效地址级别配置
+        
+        @param request: GetSuppressionListLevelRequest
+        @return: GetSuppressionListLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_suppression_list_level_with_options(request, runtime)
 
     async def get_suppression_list_level_async(
         self,
         request: dm_20151123_models.GetSuppressionListLevelRequest,
     ) -> dm_20151123_models.GetSuppressionListLevelResponse:
+        """
+        @summary 获取用户无效地址级别配置
+        
+        @param request: GetSuppressionListLevelRequest
+        @return: GetSuppressionListLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_suppression_list_level_with_options_async(request, runtime)
 
     def get_track_list_with_options(
         self,
         request: dm_20151123_models.GetTrackListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetTrackListResponse:
+        """
+        @summary 获取跟踪信息
+        
+        @param request: GetTrackListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTrackListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.offset):
             query['Offset'] = request.offset
         if not UtilClient.is_unset(request.offset_create_time):
@@ -1954,14 +2517,21 @@
         )
 
     async def get_track_list_with_options_async(
         self,
         request: dm_20151123_models.GetTrackListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetTrackListResponse:
+        """
+        @summary 获取跟踪信息
+        
+        @param request: GetTrackListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTrackListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.offset):
             query['Offset'] = request.offset
         if not UtilClient.is_unset(request.offset_create_time):
@@ -2001,29 +2571,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_track_list(
         self,
         request: dm_20151123_models.GetTrackListRequest,
     ) -> dm_20151123_models.GetTrackListResponse:
+        """
+        @summary 获取跟踪信息
+        
+        @param request: GetTrackListRequest
+        @return: GetTrackListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_track_list_with_options(request, runtime)
 
     async def get_track_list_async(
         self,
         request: dm_20151123_models.GetTrackListRequest,
     ) -> dm_20151123_models.GetTrackListResponse:
+        """
+        @summary 获取跟踪信息
+        
+        @param request: GetTrackListRequest
+        @return: GetTrackListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_track_list_with_options_async(request, runtime)
 
     def get_track_list_by_mail_from_and_tag_name_with_options(
         self,
         request: dm_20151123_models.GetTrackListByMailFromAndTagNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetTrackListByMailFromAndTagNameResponse:
+        """
+        @summary 根据发信地址和Tag名称获取跟踪信息
+        
+        @param request: GetTrackListByMailFromAndTagNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTrackListByMailFromAndTagNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.offset):
@@ -2068,14 +2657,21 @@
         )
 
     async def get_track_list_by_mail_from_and_tag_name_with_options_async(
         self,
         request: dm_20151123_models.GetTrackListByMailFromAndTagNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.GetTrackListByMailFromAndTagNameResponse:
+        """
+        @summary 根据发信地址和Tag名称获取跟踪信息
+        
+        @param request: GetTrackListByMailFromAndTagNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTrackListByMailFromAndTagNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.offset):
@@ -2119,29 +2715,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_track_list_by_mail_from_and_tag_name(
         self,
         request: dm_20151123_models.GetTrackListByMailFromAndTagNameRequest,
     ) -> dm_20151123_models.GetTrackListByMailFromAndTagNameResponse:
+        """
+        @summary 根据发信地址和Tag名称获取跟踪信息
+        
+        @param request: GetTrackListByMailFromAndTagNameRequest
+        @return: GetTrackListByMailFromAndTagNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_track_list_by_mail_from_and_tag_name_with_options(request, runtime)
 
     async def get_track_list_by_mail_from_and_tag_name_async(
         self,
         request: dm_20151123_models.GetTrackListByMailFromAndTagNameRequest,
     ) -> dm_20151123_models.GetTrackListByMailFromAndTagNameResponse:
+        """
+        @summary 根据发信地址和Tag名称获取跟踪信息
+        
+        @param request: GetTrackListByMailFromAndTagNameRequest
+        @return: GetTrackListByMailFromAndTagNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_track_list_by_mail_from_and_tag_name_with_options_async(request, runtime)
 
     def list_user_suppression_with_options(
         self,
         request: dm_20151123_models.ListUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ListUserSuppressionResponse:
+        """
+        @summary 列出用户无效地址
+        
+        @param request: ListUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.end_bounce_time):
             query['EndBounceTime'] = request.end_bounce_time
         if not UtilClient.is_unset(request.end_create_time):
@@ -2180,14 +2795,21 @@
         )
 
     async def list_user_suppression_with_options_async(
         self,
         request: dm_20151123_models.ListUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ListUserSuppressionResponse:
+        """
+        @summary 列出用户无效地址
+        
+        @param request: ListUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.address):
             query['Address'] = request.address
         if not UtilClient.is_unset(request.end_bounce_time):
             query['EndBounceTime'] = request.end_bounce_time
         if not UtilClient.is_unset(request.end_create_time):
@@ -2225,29 +2847,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_suppression(
         self,
         request: dm_20151123_models.ListUserSuppressionRequest,
     ) -> dm_20151123_models.ListUserSuppressionResponse:
+        """
+        @summary 列出用户无效地址
+        
+        @param request: ListUserSuppressionRequest
+        @return: ListUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_suppression_with_options(request, runtime)
 
     async def list_user_suppression_async(
         self,
         request: dm_20151123_models.ListUserSuppressionRequest,
     ) -> dm_20151123_models.ListUserSuppressionResponse:
+        """
+        @summary 列出用户无效地址
+        
+        @param request: ListUserSuppressionRequest
+        @return: ListUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_suppression_with_options_async(request, runtime)
 
     def modify_mail_address_with_options(
         self,
         request: dm_20151123_models.ModifyMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyMailAddressResponse:
+        """
+        @summary 修改发信地址
+        
+        @param request: ModifyMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -2278,14 +2919,21 @@
         )
 
     async def modify_mail_address_with_options_async(
         self,
         request: dm_20151123_models.ModifyMailAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyMailAddressResponse:
+        """
+        @summary 修改发信地址
+        
+        @param request: ModifyMailAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMailAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mail_address_id):
             query['MailAddressId'] = request.mail_address_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -2315,29 +2963,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_mail_address(
         self,
         request: dm_20151123_models.ModifyMailAddressRequest,
     ) -> dm_20151123_models.ModifyMailAddressResponse:
+        """
+        @summary 修改发信地址
+        
+        @param request: ModifyMailAddressRequest
+        @return: ModifyMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_mail_address_with_options(request, runtime)
 
     async def modify_mail_address_async(
         self,
         request: dm_20151123_models.ModifyMailAddressRequest,
     ) -> dm_20151123_models.ModifyMailAddressResponse:
+        """
+        @summary 修改发信地址
+        
+        @param request: ModifyMailAddressRequest
+        @return: ModifyMailAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_mail_address_with_options_async(request, runtime)
 
     def modify_pwby_domain_with_options(
         self,
         request: dm_20151123_models.ModifyPWByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
+        """
+        @summary 修改域级别密码
+        
+        @param request: ModifyPWByDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPWByDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -2366,14 +3033,21 @@
         )
 
     async def modify_pwby_domain_with_options_async(
         self,
         request: dm_20151123_models.ModifyPWByDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
+        """
+        @summary 修改域级别密码
+        
+        @param request: ModifyPWByDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPWByDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.password):
@@ -2401,29 +3075,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_pwby_domain(
         self,
         request: dm_20151123_models.ModifyPWByDomainRequest,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
+        """
+        @summary 修改域级别密码
+        
+        @param request: ModifyPWByDomainRequest
+        @return: ModifyPWByDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_pwby_domain_with_options(request, runtime)
 
     async def modify_pwby_domain_async(
         self,
         request: dm_20151123_models.ModifyPWByDomainRequest,
     ) -> dm_20151123_models.ModifyPWByDomainResponse:
+        """
+        @summary 修改域级别密码
+        
+        @param request: ModifyPWByDomainRequest
+        @return: ModifyPWByDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_pwby_domain_with_options_async(request, runtime)
 
     def modify_tag_with_options(
         self,
         request: dm_20151123_models.ModifyTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyTagResponse:
+        """
+        @summary 修改标签
+        
+        @param request: ModifyTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -2454,14 +3147,21 @@
         )
 
     async def modify_tag_with_options_async(
         self,
         request: dm_20151123_models.ModifyTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ModifyTagResponse:
+        """
+        @summary 修改标签
+        
+        @param request: ModifyTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTagResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -2491,29 +3191,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_tag(
         self,
         request: dm_20151123_models.ModifyTagRequest,
     ) -> dm_20151123_models.ModifyTagResponse:
+        """
+        @summary 修改标签
+        
+        @param request: ModifyTagRequest
+        @return: ModifyTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_tag_with_options(request, runtime)
 
     async def modify_tag_async(
         self,
         request: dm_20151123_models.ModifyTagRequest,
     ) -> dm_20151123_models.ModifyTagResponse:
+        """
+        @summary 修改标签
+        
+        @param request: ModifyTagRequest
+        @return: ModifyTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_tag_with_options_async(request, runtime)
 
     def query_domain_by_param_with_options(
         self,
         request: dm_20151123_models.QueryDomainByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryDomainByParamResponse:
+        """
+        @summary 查询域名信息
+        
+        @param request: QueryDomainByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryDomainByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2546,14 +3265,21 @@
         )
 
     async def query_domain_by_param_with_options_async(
         self,
         request: dm_20151123_models.QueryDomainByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryDomainByParamResponse:
+        """
+        @summary 查询域名信息
+        
+        @param request: QueryDomainByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryDomainByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2585,29 +3311,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_domain_by_param(
         self,
         request: dm_20151123_models.QueryDomainByParamRequest,
     ) -> dm_20151123_models.QueryDomainByParamResponse:
+        """
+        @summary 查询域名信息
+        
+        @param request: QueryDomainByParamRequest
+        @return: QueryDomainByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_domain_by_param_with_options(request, runtime)
 
     async def query_domain_by_param_async(
         self,
         request: dm_20151123_models.QueryDomainByParamRequest,
     ) -> dm_20151123_models.QueryDomainByParamResponse:
+        """
+        @summary 查询域名信息
+        
+        @param request: QueryDomainByParamRequest
+        @return: QueryDomainByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_domain_by_param_with_options_async(request, runtime)
 
     def query_invalid_address_with_options(
         self,
         request: dm_20151123_models.QueryInvalidAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryInvalidAddressResponse:
+        """
+        @summary NextStart修改为string
+        
+        @param request: QueryInvalidAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInvalidAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.length):
@@ -2642,14 +3387,21 @@
         )
 
     async def query_invalid_address_with_options_async(
         self,
         request: dm_20151123_models.QueryInvalidAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryInvalidAddressResponse:
+        """
+        @summary NextStart修改为string
+        
+        @param request: QueryInvalidAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInvalidAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.length):
@@ -2683,29 +3435,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_invalid_address(
         self,
         request: dm_20151123_models.QueryInvalidAddressRequest,
     ) -> dm_20151123_models.QueryInvalidAddressResponse:
+        """
+        @summary NextStart修改为string
+        
+        @param request: QueryInvalidAddressRequest
+        @return: QueryInvalidAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_invalid_address_with_options(request, runtime)
 
     async def query_invalid_address_async(
         self,
         request: dm_20151123_models.QueryInvalidAddressRequest,
     ) -> dm_20151123_models.QueryInvalidAddressResponse:
+        """
+        @summary NextStart修改为string
+        
+        @param request: QueryInvalidAddressRequest
+        @return: QueryInvalidAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_invalid_address_with_options_async(request, runtime)
 
     def query_mail_address_by_param_with_options(
         self,
         request: dm_20151123_models.QueryMailAddressByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryMailAddressByParamResponse:
+        """
+        @param request: QueryMailAddressByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMailAddressByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2738,14 +3507,19 @@
         )
 
     async def query_mail_address_by_param_with_options_async(
         self,
         request: dm_20151123_models.QueryMailAddressByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryMailAddressByParamResponse:
+        """
+        @param request: QueryMailAddressByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMailAddressByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2777,29 +3551,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mail_address_by_param(
         self,
         request: dm_20151123_models.QueryMailAddressByParamRequest,
     ) -> dm_20151123_models.QueryMailAddressByParamResponse:
+        """
+        @param request: QueryMailAddressByParamRequest
+        @return: QueryMailAddressByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mail_address_by_param_with_options(request, runtime)
 
     async def query_mail_address_by_param_async(
         self,
         request: dm_20151123_models.QueryMailAddressByParamRequest,
     ) -> dm_20151123_models.QueryMailAddressByParamResponse:
+        """
+        @param request: QueryMailAddressByParamRequest
+        @return: QueryMailAddressByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mail_address_by_param_with_options_async(request, runtime)
 
     def query_receiver_by_param_with_options(
         self,
         request: dm_20151123_models.QueryReceiverByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryReceiverByParamResponse:
+        """
+        @summary 查询收信人列表详情
+        
+        @param request: QueryReceiverByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryReceiverByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2832,14 +3621,21 @@
         )
 
     async def query_receiver_by_param_with_options_async(
         self,
         request: dm_20151123_models.QueryReceiverByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryReceiverByParamResponse:
+        """
+        @summary 查询收信人列表详情
+        
+        @param request: QueryReceiverByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryReceiverByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -2871,29 +3667,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_receiver_by_param(
         self,
         request: dm_20151123_models.QueryReceiverByParamRequest,
     ) -> dm_20151123_models.QueryReceiverByParamResponse:
+        """
+        @summary 查询收信人列表详情
+        
+        @param request: QueryReceiverByParamRequest
+        @return: QueryReceiverByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_receiver_by_param_with_options(request, runtime)
 
     async def query_receiver_by_param_async(
         self,
         request: dm_20151123_models.QueryReceiverByParamRequest,
     ) -> dm_20151123_models.QueryReceiverByParamResponse:
+        """
+        @summary 查询收信人列表详情
+        
+        @param request: QueryReceiverByParamRequest
+        @return: QueryReceiverByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_receiver_by_param_with_options_async(request, runtime)
 
     def query_receiver_detail_with_options(
         self,
         request: dm_20151123_models.QueryReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryReceiverDetailResponse:
+        """
+        @summary 查询收信人列表详情信息
+        
+        @param request: QueryReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.next_start):
             query['NextStart'] = request.next_start
         if not UtilClient.is_unset(request.owner_id):
@@ -2926,14 +3741,21 @@
         )
 
     async def query_receiver_detail_with_options_async(
         self,
         request: dm_20151123_models.QueryReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryReceiverDetailResponse:
+        """
+        @summary 查询收信人列表详情信息
+        
+        @param request: QueryReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.next_start):
             query['NextStart'] = request.next_start
         if not UtilClient.is_unset(request.owner_id):
@@ -2965,29 +3787,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_receiver_detail(
         self,
         request: dm_20151123_models.QueryReceiverDetailRequest,
     ) -> dm_20151123_models.QueryReceiverDetailResponse:
+        """
+        @summary 查询收信人列表详情信息
+        
+        @param request: QueryReceiverDetailRequest
+        @return: QueryReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_receiver_detail_with_options(request, runtime)
 
     async def query_receiver_detail_async(
         self,
         request: dm_20151123_models.QueryReceiverDetailRequest,
     ) -> dm_20151123_models.QueryReceiverDetailResponse:
+        """
+        @summary 查询收信人列表详情信息
+        
+        @param request: QueryReceiverDetailRequest
+        @return: QueryReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_receiver_detail_with_options_async(request, runtime)
 
     def query_tag_by_param_with_options(
         self,
         request: dm_20151123_models.QueryTagByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryTagByParamResponse:
+        """
+        @param request: QueryTagByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryTagByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -3018,14 +3857,19 @@
         )
 
     async def query_tag_by_param_with_options_async(
         self,
         request: dm_20151123_models.QueryTagByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryTagByParamResponse:
+        """
+        @param request: QueryTagByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryTagByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -3055,29 +3899,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_tag_by_param(
         self,
         request: dm_20151123_models.QueryTagByParamRequest,
     ) -> dm_20151123_models.QueryTagByParamResponse:
+        """
+        @param request: QueryTagByParamRequest
+        @return: QueryTagByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_tag_by_param_with_options(request, runtime)
 
     async def query_tag_by_param_async(
         self,
         request: dm_20151123_models.QueryTagByParamRequest,
     ) -> dm_20151123_models.QueryTagByParamResponse:
+        """
+        @param request: QueryTagByParamRequest
+        @return: QueryTagByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_tag_by_param_with_options_async(request, runtime)
 
     def query_task_by_param_with_options(
         self,
         request: dm_20151123_models.QueryTaskByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryTaskByParamResponse:
+        """
+        @param request: QueryTaskByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryTaskByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -3110,14 +3967,19 @@
         )
 
     async def query_task_by_param_with_options_async(
         self,
         request: dm_20151123_models.QueryTaskByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.QueryTaskByParamResponse:
+        """
+        @param request: QueryTaskByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryTaskByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.key_word):
             query['KeyWord'] = request.key_word
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_no):
@@ -3149,29 +4011,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_task_by_param(
         self,
         request: dm_20151123_models.QueryTaskByParamRequest,
     ) -> dm_20151123_models.QueryTaskByParamResponse:
+        """
+        @param request: QueryTaskByParamRequest
+        @return: QueryTaskByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_task_by_param_with_options(request, runtime)
 
     async def query_task_by_param_async(
         self,
         request: dm_20151123_models.QueryTaskByParamRequest,
     ) -> dm_20151123_models.QueryTaskByParamResponse:
+        """
+        @param request: QueryTaskByParamRequest
+        @return: QueryTaskByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_task_by_param_with_options_async(request, runtime)
 
     def remove_user_suppression_with_options(
         self,
         request: dm_20151123_models.RemoveUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.RemoveUserSuppressionResponse:
+        """
+        @summary 删除用户无效地址
+        
+        @param request: RemoveUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -3198,14 +4075,21 @@
         )
 
     async def remove_user_suppression_with_options_async(
         self,
         request: dm_20151123_models.RemoveUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.RemoveUserSuppressionResponse:
+        """
+        @summary 删除用户无效地址
+        
+        @param request: RemoveUserSuppressionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveUserSuppressionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -3231,29 +4115,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_user_suppression(
         self,
         request: dm_20151123_models.RemoveUserSuppressionRequest,
     ) -> dm_20151123_models.RemoveUserSuppressionResponse:
+        """
+        @summary 删除用户无效地址
+        
+        @param request: RemoveUserSuppressionRequest
+        @return: RemoveUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_user_suppression_with_options(request, runtime)
 
     async def remove_user_suppression_async(
         self,
         request: dm_20151123_models.RemoveUserSuppressionRequest,
     ) -> dm_20151123_models.RemoveUserSuppressionResponse:
+        """
+        @summary 删除用户无效地址
+        
+        @param request: RemoveUserSuppressionRequest
+        @return: RemoveUserSuppressionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_user_suppression_with_options_async(request, runtime)
 
     def save_receiver_detail_with_options(
         self,
         request: dm_20151123_models.SaveReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SaveReceiverDetailResponse:
+        """
+        @summary 建单个收件人
+        
+        @param request: SaveReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SaveReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.detail):
             query['Detail'] = request.detail
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
@@ -3282,14 +4185,21 @@
         )
 
     async def save_receiver_detail_with_options_async(
         self,
         request: dm_20151123_models.SaveReceiverDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SaveReceiverDetailResponse:
+        """
+        @summary 建单个收件人
+        
+        @param request: SaveReceiverDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SaveReceiverDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.detail):
             query['Detail'] = request.detail
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.receiver_id):
@@ -3317,29 +4227,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def save_receiver_detail(
         self,
         request: dm_20151123_models.SaveReceiverDetailRequest,
     ) -> dm_20151123_models.SaveReceiverDetailResponse:
+        """
+        @summary 建单个收件人
+        
+        @param request: SaveReceiverDetailRequest
+        @return: SaveReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.save_receiver_detail_with_options(request, runtime)
 
     async def save_receiver_detail_async(
         self,
         request: dm_20151123_models.SaveReceiverDetailRequest,
     ) -> dm_20151123_models.SaveReceiverDetailResponse:
+        """
+        @summary 建单个收件人
+        
+        @param request: SaveReceiverDetailRequest
+        @return: SaveReceiverDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.save_receiver_detail_with_options_async(request, runtime)
 
     def send_test_by_template_with_options(
         self,
         request: dm_20151123_models.SendTestByTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SendTestByTemplateResponse:
+        """
+        @summary 发送模板测试邮件
+        
+        @param request: SendTestByTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SendTestByTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.birthday):
             query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.email):
@@ -3380,14 +4309,21 @@
         )
 
     async def send_test_by_template_with_options_async(
         self,
         request: dm_20151123_models.SendTestByTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SendTestByTemplateResponse:
+        """
+        @summary 发送模板测试邮件
+        
+        @param request: SendTestByTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SendTestByTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.birthday):
             query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.email):
@@ -3427,29 +4363,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def send_test_by_template(
         self,
         request: dm_20151123_models.SendTestByTemplateRequest,
     ) -> dm_20151123_models.SendTestByTemplateResponse:
+        """
+        @summary 发送模板测试邮件
+        
+        @param request: SendTestByTemplateRequest
+        @return: SendTestByTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.send_test_by_template_with_options(request, runtime)
 
     async def send_test_by_template_async(
         self,
         request: dm_20151123_models.SendTestByTemplateRequest,
     ) -> dm_20151123_models.SendTestByTemplateResponse:
+        """
+        @summary 发送模板测试邮件
+        
+        @param request: SendTestByTemplateRequest
+        @return: SendTestByTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.send_test_by_template_with_options_async(request, runtime)
 
     def sender_statistics_by_tag_name_and_batch_idwith_options(
         self,
         request: dm_20151123_models.SenderStatisticsByTagNameAndBatchIDRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SenderStatisticsByTagNameAndBatchIDResponse:
+        """
+        @summary 获取指定条件下的发送数据
+        
+        @param request: SenderStatisticsByTagNameAndBatchIDRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SenderStatisticsByTagNameAndBatchIDResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.owner_id):
@@ -3482,14 +4437,21 @@
         )
 
     async def sender_statistics_by_tag_name_and_batch_idwith_options_async(
         self,
         request: dm_20151123_models.SenderStatisticsByTagNameAndBatchIDRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SenderStatisticsByTagNameAndBatchIDResponse:
+        """
+        @summary 获取指定条件下的发送数据
+        
+        @param request: SenderStatisticsByTagNameAndBatchIDRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SenderStatisticsByTagNameAndBatchIDResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.owner_id):
@@ -3521,29 +4483,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def sender_statistics_by_tag_name_and_batch_id(
         self,
         request: dm_20151123_models.SenderStatisticsByTagNameAndBatchIDRequest,
     ) -> dm_20151123_models.SenderStatisticsByTagNameAndBatchIDResponse:
+        """
+        @summary 获取指定条件下的发送数据
+        
+        @param request: SenderStatisticsByTagNameAndBatchIDRequest
+        @return: SenderStatisticsByTagNameAndBatchIDResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.sender_statistics_by_tag_name_and_batch_idwith_options(request, runtime)
 
     async def sender_statistics_by_tag_name_and_batch_id_async(
         self,
         request: dm_20151123_models.SenderStatisticsByTagNameAndBatchIDRequest,
     ) -> dm_20151123_models.SenderStatisticsByTagNameAndBatchIDResponse:
+        """
+        @summary 获取指定条件下的发送数据
+        
+        @param request: SenderStatisticsByTagNameAndBatchIDRequest
+        @return: SenderStatisticsByTagNameAndBatchIDResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.sender_statistics_by_tag_name_and_batch_idwith_options_async(request, runtime)
 
     def sender_statistics_detail_by_param_with_options(
         self,
         request: dm_20151123_models.SenderStatisticsDetailByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SenderStatisticsDetailByParamResponse:
+        """
+        @summary 查询投递结果详情
+        
+        @param request: SenderStatisticsDetailByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SenderStatisticsDetailByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.length):
@@ -3584,14 +4565,21 @@
         )
 
     async def sender_statistics_detail_by_param_with_options_async(
         self,
         request: dm_20151123_models.SenderStatisticsDetailByParamRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SenderStatisticsDetailByParamResponse:
+        """
+        @summary 查询投递结果详情
+        
+        @param request: SenderStatisticsDetailByParamRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SenderStatisticsDetailByParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.length):
@@ -3631,29 +4619,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def sender_statistics_detail_by_param(
         self,
         request: dm_20151123_models.SenderStatisticsDetailByParamRequest,
     ) -> dm_20151123_models.SenderStatisticsDetailByParamResponse:
+        """
+        @summary 查询投递结果详情
+        
+        @param request: SenderStatisticsDetailByParamRequest
+        @return: SenderStatisticsDetailByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.sender_statistics_detail_by_param_with_options(request, runtime)
 
     async def sender_statistics_detail_by_param_async(
         self,
         request: dm_20151123_models.SenderStatisticsDetailByParamRequest,
     ) -> dm_20151123_models.SenderStatisticsDetailByParamResponse:
+        """
+        @summary 查询投递结果详情
+        
+        @param request: SenderStatisticsDetailByParamRequest
+        @return: SenderStatisticsDetailByParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.sender_statistics_detail_by_param_with_options_async(request, runtime)
 
     def set_suppression_list_level_with_options(
         self,
         request: dm_20151123_models.SetSuppressionListLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SetSuppressionListLevelResponse:
+        """
+        @summary 设置用户无效地址级别配置
+        
+        @param request: SetSuppressionListLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSuppressionListLevelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -3680,14 +4687,21 @@
         )
 
     async def set_suppression_list_level_with_options_async(
         self,
         request: dm_20151123_models.SetSuppressionListLevelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SetSuppressionListLevelResponse:
+        """
+        @summary 设置用户无效地址级别配置
+        
+        @param request: SetSuppressionListLevelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSuppressionListLevelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
             query['ResourceOwnerAccount'] = request.resource_owner_account
         if not UtilClient.is_unset(request.resource_owner_id):
@@ -3713,29 +4727,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_suppression_list_level(
         self,
         request: dm_20151123_models.SetSuppressionListLevelRequest,
     ) -> dm_20151123_models.SetSuppressionListLevelResponse:
+        """
+        @summary 设置用户无效地址级别配置
+        
+        @param request: SetSuppressionListLevelRequest
+        @return: SetSuppressionListLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_suppression_list_level_with_options(request, runtime)
 
     async def set_suppression_list_level_async(
         self,
         request: dm_20151123_models.SetSuppressionListLevelRequest,
     ) -> dm_20151123_models.SetSuppressionListLevelResponse:
+        """
+        @summary 设置用户无效地址级别配置
+        
+        @param request: SetSuppressionListLevelRequest
+        @return: SetSuppressionListLevelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_suppression_list_level_with_options_async(request, runtime)
 
     def single_send_mail_with_options(
         self,
         request: dm_20151123_models.SingleSendMailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SingleSendMailResponse:
+        """
+        @summary API发信
+        
+        @param request: SingleSendMailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SingleSendMailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.click_trace):
@@ -3788,14 +4821,21 @@
         )
 
     async def single_send_mail_with_options_async(
         self,
         request: dm_20151123_models.SingleSendMailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.SingleSendMailResponse:
+        """
+        @summary API发信
+        
+        @param request: SingleSendMailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SingleSendMailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.address_type):
             query['AddressType'] = request.address_type
         if not UtilClient.is_unset(request.click_trace):
@@ -3847,29 +4887,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def single_send_mail(
         self,
         request: dm_20151123_models.SingleSendMailRequest,
     ) -> dm_20151123_models.SingleSendMailResponse:
+        """
+        @summary API发信
+        
+        @param request: SingleSendMailRequest
+        @return: SingleSendMailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.single_send_mail_with_options(request, runtime)
 
     async def single_send_mail_async(
         self,
         request: dm_20151123_models.SingleSendMailRequest,
     ) -> dm_20151123_models.SingleSendMailResponse:
+        """
+        @summary API发信
+        
+        @param request: SingleSendMailRequest
+        @return: SingleSendMailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.single_send_mail_with_options_async(request, runtime)
 
     def update_ip_protection_with_options(
         self,
         request: dm_20151123_models.UpdateIpProtectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.UpdateIpProtectionResponse:
+        """
+        @summary 更新IP防护API
+        
+        @param request: UpdateIpProtectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateIpProtectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_protection):
             query['IpProtection'] = request.ip_protection
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -3896,14 +4955,21 @@
         )
 
     async def update_ip_protection_with_options_async(
         self,
         request: dm_20151123_models.UpdateIpProtectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.UpdateIpProtectionResponse:
+        """
+        @summary 更新IP防护API
+        
+        @param request: UpdateIpProtectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateIpProtectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_protection):
             query['IpProtection'] = request.ip_protection
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -3929,16 +4995,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_ip_protection(
         self,
         request: dm_20151123_models.UpdateIpProtectionRequest,
     ) -> dm_20151123_models.UpdateIpProtectionResponse:
+        """
+        @summary 更新IP防护API
+        
+        @param request: UpdateIpProtectionRequest
+        @return: UpdateIpProtectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_ip_protection_with_options(request, runtime)
 
     async def update_ip_protection_async(
         self,
         request: dm_20151123_models.UpdateIpProtectionRequest,
     ) -> dm_20151123_models.UpdateIpProtectionResponse:
+        """
+        @summary 更新IP防护API
+        
+        @param request: UpdateIpProtectionRequest
+        @return: UpdateIpProtectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_ip_protection_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123/models.py` & `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     def __init__(
         self,
         ip_address: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.ip_address = ip_address
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -130,14 +131,15 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         ticket: str = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.ticket = ticket
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -249,24 +251,28 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         tag_name: str = None,
         template_name: str = None,
         un_subscribe_filter_level: str = None,
         un_subscribe_link_type: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
+        # This parameter is required.
         self.address_type = address_type
         self.click_trace = click_trace
         self.owner_id = owner_id
+        # This parameter is required.
         self.receivers_name = receivers_name
         self.reply_address = reply_address
         self.reply_address_alias = reply_address_alias
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.tag_name = tag_name
+        # This parameter is required.
         self.template_name = template_name
         self.un_subscribe_filter_level = un_subscribe_filter_level
         self.un_subscribe_link_type = un_subscribe_link_type
 
     def validate(self):
         pass
 
@@ -414,14 +420,16 @@
         self,
         domain_id: int = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the domain name.
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -544,14 +552,15 @@
         mail_address_id: int = None,
         owner_id: int = None,
         region: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.lang = lang
+        # This parameter is required.
         self.mail_address_id = mail_address_id
         self.owner_id = owner_id
         self.region = region
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -666,14 +675,15 @@
     def __init__(
         self,
         domain_name: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.domain_name = domain_name
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -787,19 +797,21 @@
         account_name: str = None,
         owner_id: int = None,
         reply_address: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         sendtype: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
         self.owner_id = owner_id
         self.reply_address = reply_address
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.sendtype = sendtype
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -920,15 +932,17 @@
         receivers_alias: str = None,
         receivers_name: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.desc = desc
         self.owner_id = owner_id
+        # This parameter is required.
         self.receivers_alias = receivers_alias
+        # This parameter is required.
         self.receivers_name = receivers_name
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -1052,14 +1066,15 @@
         tag_description: str = None,
         tag_name: str = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.tag_description = tag_description
+        # This parameter is required.
         self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1291,14 +1306,15 @@
     def __init__(
         self,
         domain_id: int = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.domain_id = domain_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -1636,14 +1652,15 @@
     def __init__(
         self,
         mail_address_id: int = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.mail_address_id = mail_address_id
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -1751,14 +1768,16 @@
         owner_id: int = None,
         receiver_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.owner_id = owner_id
         # The ID of the recipient list.
+        # 
+        # This parameter is required.
         self.receiver_id = receiver_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -1867,14 +1886,15 @@
         owner_id: int = None,
         receiver_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.email = email
         self.owner_id = owner_id
+        # This parameter is required.
         self.receiver_id = receiver_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -1987,14 +2007,16 @@
         resource_owner_id: int = None,
         tag_id: int = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The ID of the tag.
+        # 
+        # This parameter is required.
         self.tag_id = tag_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2302,14 +2324,15 @@
         self,
         domain_id: int = None,
         owner_id: int = None,
         require_real_time_dns_records: bool = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.domain_id = domain_id
         self.owner_id = owner_id
         self.require_real_time_dns_records = require_real_time_dns_records
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -3028,23 +3051,25 @@
         page_number: str = None,
         page_size: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
         total: str = None,
     ):
+        # This parameter is required.
         self.end_time = end_time
         self.offset = offset
         self.offset_create_time = offset_create_time
         self.offset_create_time_desc = offset_create_time_desc
         self.owner_id = owner_id
         self.page_number = page_number
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.start_time = start_time
         self.total = total
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3340,23 +3365,25 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
         tag_name: str = None,
         total: str = None,
     ):
         self.account_name = account_name
+        # This parameter is required.
         self.end_time = end_time
         self.offset = offset
         self.offset_create_time = offset_create_time
         self.offset_create_time_desc = offset_create_time_desc
         self.owner_id = owner_id
         self.page_number = page_number
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.start_time = start_time
         self.tag_name = tag_name
         self.total = total
 
     def validate(self):
         pass
 
@@ -3914,14 +3941,15 @@
         mail_address_id: int = None,
         owner_id: int = None,
         password: str = None,
         reply_address: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.mail_address_id = mail_address_id
         self.owner_id = owner_id
         self.password = password
         self.reply_address = reply_address
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
@@ -4038,16 +4066,18 @@
         self,
         domain_name: str = None,
         owner_id: int = None,
         password: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.domain_name = domain_name
         self.owner_id = owner_id
+        # This parameter is required.
         self.password = password
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -4181,16 +4211,20 @@
         tag_name: str = None,
     ):
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.tag_description = tag_description
         # The ID of the tag.
+        # 
+        # This parameter is required.
         self.tag_id = tag_id
         # The name of the tag.
+        # 
+        # This parameter is required.
         self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5365,14 +5399,15 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.key_word = key_word
         self.next_start = next_start
         self.owner_id = owner_id
         self.page_size = page_size
+        # This parameter is required.
         self.receiver_id = receiver_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -6201,16 +6236,18 @@
         self,
         detail: str = None,
         owner_id: int = None,
         receiver_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.detail = detail
         self.owner_id = owner_id
+        # This parameter is required.
         self.receiver_id = receiver_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -6408,23 +6445,26 @@
         nick_name: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         template_id: int = None,
         user_name: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
         self.birthday = birthday
+        # This parameter is required.
         self.email = email
         self.gender = gender
         self.mobile = mobile
         self.nick_name = nick_name
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.template_id = template_id
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6560,18 +6600,20 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
         tag_name: str = None,
     ):
         self.account_name = account_name
+        # This parameter is required.
         self.end_time = end_time
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.start_time = start_time
         self.tag_name = tag_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7204,28 +7246,33 @@
         subject: str = None,
         tag_name: str = None,
         text_body: str = None,
         to_address: str = None,
         un_subscribe_filter_level: str = None,
         un_subscribe_link_type: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
+        # This parameter is required.
         self.address_type = address_type
         self.click_trace = click_trace
         self.from_alias = from_alias
         self.html_body = html_body
         self.owner_id = owner_id
         self.reply_address = reply_address
         self.reply_address_alias = reply_address_alias
+        # This parameter is required.
         self.reply_to_address = reply_to_address
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.subject = subject
         self.tag_name = tag_name
         self.text_body = text_body
+        # This parameter is required.
         self.to_address = to_address
         self.un_subscribe_filter_level = un_subscribe_filter_level
         self.un_subscribe_link_type = un_subscribe_link_type
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_dm20151123-1.1.0/alibabacloud_dm20151123.egg-info/PKG-INFO` & `alibabacloud_dm20151123-1.1.1/alibabacloud_dm20151123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20151123
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.0/setup.py` & `alibabacloud_dm20151123-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20151123.
 
-Created on 22/04/2024
+Created on 14/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20151123"
 NAME = "alibabacloud_dm20151123" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20151123) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

