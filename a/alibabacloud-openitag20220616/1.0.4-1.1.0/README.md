# Comparing `tmp/alibabacloud_openitag20220616-1.0.4.tar.gz` & `tmp/alibabacloud_openitag20220616-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_openitag20220616-1.0.4.tar", last modified: Fri Mar  1 02:19:12 2024, max compression
+gzip compressed data, was "dist/alibabacloud_openitag20220616-1.1.0.tar", last modified: Wed May 15 17:11:07 2024, max compression
```

## Comparing `alibabacloud_openitag20220616-1.0.4.tar` & `alibabacloud_openitag20220616-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      778 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111947 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/client.py
--rw-r--r--   0 root         (0) root         (0)   263962 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-01 02:19:12.000000 alibabacloud_openitag20220616-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-01 02:19:11.000000 alibabacloud_openitag20220616-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143937 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/client.py
+-rw-r--r--   0 root         (0) root         (0)   270303 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 17:11:07.000000 alibabacloud_openitag20220616-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-15 17:11:05.000000 alibabacloud_openitag20220616-1.1.0/setup.py
```

### Comparing `alibabacloud_openitag20220616-1.0.4/LICENSE` & `alibabacloud_openitag20220616-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.4/PKG-INFO` & `alibabacloud_openitag20220616-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_openitag20220616
-Version: 1.0.4
+Version: 1.1.0
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616-1.0.4/README-CN.md` & `alibabacloud_openitag20220616-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.4/README.md` & `alibabacloud_openitag20220616-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/client.py` & `alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
+        """
+        @summary 增加结点任务人力
+        
+        @param request: AddWorkNodeWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddWorkNodeWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -79,14 +87,22 @@
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
+        """
+        @summary 增加结点任务人力
+        
+        @param request: AddWorkNodeWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddWorkNodeWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -110,36 +126,162 @@
     def add_work_node_workforce(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
     ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
+        """
+        @summary 增加结点任务人力
+        
+        @param request: AddWorkNodeWorkforceRequest
+        @return: AddWorkNodeWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.add_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     async def add_work_node_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.AddWorkNodeWorkforceRequest,
     ) -> open_itag_20220616_models.AddWorkNodeWorkforceResponse:
+        """
+        @summary 增加结点任务人力
+        
+        @param request: AddWorkNodeWorkforceRequest
+        @return: AddWorkNodeWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.add_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
 
+    def append_all_data_to_task_with_options(
+        self,
+        tenant_id: str,
+        task_id: str,
+        request: open_itag_20220616_models.AppendAllDataToTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> open_itag_20220616_models.AppendAllDataToTaskResponse:
+        """
+        @summary 数据追加
+        
+        @param request: AppendAllDataToTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AppendAllDataToTaskResponse
+        """
+        UtilClient.validate_model(request)
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(request.body)
+        )
+        params = open_api_models.Params(
+            action='AppendAllDataToTask',
+            version='2022-06-16',
+            protocol='HTTPS',
+            pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks/{OpenApiUtilClient.get_encode_param(task_id)}/appendAllDataToTask',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            open_itag_20220616_models.AppendAllDataToTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def append_all_data_to_task_with_options_async(
+        self,
+        tenant_id: str,
+        task_id: str,
+        request: open_itag_20220616_models.AppendAllDataToTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> open_itag_20220616_models.AppendAllDataToTaskResponse:
+        """
+        @summary 数据追加
+        
+        @param request: AppendAllDataToTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AppendAllDataToTaskResponse
+        """
+        UtilClient.validate_model(request)
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(request.body)
+        )
+        params = open_api_models.Params(
+            action='AppendAllDataToTask',
+            version='2022-06-16',
+            protocol='HTTPS',
+            pathname=f'/openapi/api/v1/tenants/{OpenApiUtilClient.get_encode_param(tenant_id)}/tasks/{OpenApiUtilClient.get_encode_param(task_id)}/appendAllDataToTask',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            open_itag_20220616_models.AppendAllDataToTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def append_all_data_to_task(
+        self,
+        tenant_id: str,
+        task_id: str,
+        request: open_itag_20220616_models.AppendAllDataToTaskRequest,
+    ) -> open_itag_20220616_models.AppendAllDataToTaskResponse:
+        """
+        @summary 数据追加
+        
+        @param request: AppendAllDataToTaskRequest
+        @return: AppendAllDataToTaskResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.append_all_data_to_task_with_options(tenant_id, task_id, request, headers, runtime)
+
+    async def append_all_data_to_task_async(
+        self,
+        tenant_id: str,
+        task_id: str,
+        request: open_itag_20220616_models.AppendAllDataToTaskRequest,
+    ) -> open_itag_20220616_models.AppendAllDataToTaskResponse:
+        """
+        @summary 数据追加
+        
+        @param request: AppendAllDataToTaskRequest
+        @return: AppendAllDataToTaskResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.append_all_data_to_task_with_options_async(tenant_id, task_id, request, headers, runtime)
+
     def create_task_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTaskResponse:
+        """
+        @summary 创建标注任务
+        
+        @param request: CreateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTaskResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTask',
@@ -160,14 +302,22 @@
     async def create_task_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTaskResponse:
+        """
+        @summary 创建标注任务
+        
+        @param request: CreateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTaskResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTask',
@@ -186,34 +336,54 @@
         )
 
     def create_task(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTaskRequest,
     ) -> open_itag_20220616_models.CreateTaskResponse:
+        """
+        @summary 创建标注任务
+        
+        @param request: CreateTaskRequest
+        @return: CreateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_task_with_options(tenant_id, request, headers, runtime)
 
     async def create_task_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTaskRequest,
     ) -> open_itag_20220616_models.CreateTaskResponse:
+        """
+        @summary 创建标注任务
+        
+        @param request: CreateTaskRequest
+        @return: CreateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_task_with_options_async(tenant_id, request, headers, runtime)
 
     def create_template_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
+        """
+        @summary 创建标注模版
+        
+        @param request: CreateTemplateRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTemplateResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTemplate',
@@ -234,14 +404,22 @@
     async def create_template_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
+        """
+        @summary 创建标注模版
+        
+        @param request: CreateTemplateRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTemplateResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='CreateTemplate',
@@ -260,34 +438,54 @@
         )
 
     def create_template(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTemplateRequest,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
+        """
+        @summary 创建标注模版
+        
+        @param request: CreateTemplateRequest
+        @return: CreateTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_template_with_options(tenant_id, request, headers, runtime)
 
     async def create_template_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateTemplateRequest,
     ) -> open_itag_20220616_models.CreateTemplateResponse:
+        """
+        @summary 创建标注模版
+        
+        @param request: CreateTemplateRequest
+        @return: CreateTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_template_with_options_async(tenant_id, request, headers, runtime)
 
     def create_user_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateUserResponse:
+        """
+        @summary 创建租户内用户
+        
+        @param request: CreateUserRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.account_no):
             body['AccountNo'] = request.account_no
         if not UtilClient.is_unset(request.account_type):
             body['AccountType'] = request.account_type
         if not UtilClient.is_unset(request.role):
@@ -317,14 +515,22 @@
     async def create_user_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.CreateUserResponse:
+        """
+        @summary 创建租户内用户
+        
+        @param request: CreateUserRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.account_no):
             body['AccountNo'] = request.account_no
         if not UtilClient.is_unset(request.account_type):
             body['AccountType'] = request.account_type
         if not UtilClient.is_unset(request.role):
@@ -352,34 +558,53 @@
         )
 
     def create_user(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateUserRequest,
     ) -> open_itag_20220616_models.CreateUserResponse:
+        """
+        @summary 创建租户内用户
+        
+        @param request: CreateUserRequest
+        @return: CreateUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_user_with_options(tenant_id, request, headers, runtime)
 
     async def create_user_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.CreateUserRequest,
     ) -> open_itag_20220616_models.CreateUserResponse:
+        """
+        @summary 创建租户内用户
+        
+        @param request: CreateUserRequest
+        @return: CreateUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_user_with_options_async(tenant_id, request, headers, runtime)
 
     def delete_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteTaskResponse:
+        """
+        @summary 删除任务
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -398,14 +623,21 @@
     async def delete_task_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteTaskResponse:
+        """
+        @summary 删除任务
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -422,34 +654,51 @@
         )
 
     def delete_task(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.DeleteTaskResponse:
+        """
+        @summary 删除任务
+        
+        @return: DeleteTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_task_with_options(tenant_id, task_id, headers, runtime)
 
     async def delete_task_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.DeleteTaskResponse:
+        """
+        @summary 删除任务
+        
+        @return: DeleteTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_task_with_options_async(tenant_id, task_id, headers, runtime)
 
     def delete_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        """
+        @summary 删除租户下的单个模板
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -468,14 +717,21 @@
     async def delete_template_with_options_async(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        """
+        @summary 删除租户下的单个模板
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -492,34 +748,51 @@
         )
 
     def delete_template(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        """
+        @summary 删除租户下的单个模板
+        
+        @return: DeleteTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_template_with_options(tenant_id, template_id, headers, runtime)
 
     async def delete_template_async(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.DeleteTemplateResponse:
+        """
+        @summary 删除租户下的单个模板
+        
+        @return: DeleteTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_template_with_options_async(tenant_id, template_id, headers, runtime)
 
     def delete_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteUserResponse:
+        """
+        @summary 删除用户
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteUser',
             version='2022-06-16',
             protocol='HTTPS',
@@ -538,14 +811,21 @@
     async def delete_user_with_options_async(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.DeleteUserResponse:
+        """
+        @summary 删除用户
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteUser',
             version='2022-06-16',
             protocol='HTTPS',
@@ -562,35 +842,53 @@
         )
 
     def delete_user(
         self,
         tenant_id: str,
         user_id: str,
     ) -> open_itag_20220616_models.DeleteUserResponse:
+        """
+        @summary 删除用户
+        
+        @return: DeleteUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_user_with_options(tenant_id, user_id, headers, runtime)
 
     async def delete_user_async(
         self,
         tenant_id: str,
         user_id: str,
     ) -> open_itag_20220616_models.DeleteUserResponse:
+        """
+        @summary 删除用户
+        
+        @return: DeleteUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_user_with_options_async(tenant_id, user_id, headers, runtime)
 
     def export_annotations_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ExportAnnotationsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        """
+        @summary 获取任务导出结果
+        
+        @param request: ExportAnnotationsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExportAnnotationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.oss_path):
             query['OssPath'] = request.oss_path
         if not UtilClient.is_unset(request.register_dataset):
             query['RegisterDataset'] = request.register_dataset
         if not UtilClient.is_unset(request.target):
@@ -619,14 +917,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ExportAnnotationsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        """
+        @summary 获取任务导出结果
+        
+        @param request: ExportAnnotationsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExportAnnotationsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.oss_path):
             query['OssPath'] = request.oss_path
         if not UtilClient.is_unset(request.register_dataset):
             query['RegisterDataset'] = request.register_dataset
         if not UtilClient.is_unset(request.target):
@@ -653,36 +959,56 @@
 
     def export_annotations(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ExportAnnotationsRequest,
     ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        """
+        @summary 获取任务导出结果
+        
+        @param request: ExportAnnotationsRequest
+        @return: ExportAnnotationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.export_annotations_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def export_annotations_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ExportAnnotationsRequest,
     ) -> open_itag_20220616_models.ExportAnnotationsResponse:
+        """
+        @summary 获取任务导出结果
+        
+        @param request: ExportAnnotationsRequest
+        @return: ExportAnnotationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.export_annotations_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_job_with_options(
         self,
         tenant_id: str,
         job_id: str,
         request: open_itag_20220616_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetJobResponse:
+        """
+        @summary 获取异步任务Job
+        
+        @param request: GetJobRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -707,14 +1033,22 @@
         self,
         tenant_id: str,
         job_id: str,
         request: open_itag_20220616_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetJobResponse:
+        """
+        @summary 获取异步任务Job
+        
+        @param request: GetJobRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -737,36 +1071,55 @@
 
     def get_job(
         self,
         tenant_id: str,
         job_id: str,
         request: open_itag_20220616_models.GetJobRequest,
     ) -> open_itag_20220616_models.GetJobResponse:
+        """
+        @summary 获取异步任务Job
+        
+        @param request: GetJobRequest
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_job_with_options(tenant_id, job_id, request, headers, runtime)
 
     async def get_job_async(
         self,
         tenant_id: str,
         job_id: str,
         request: open_itag_20220616_models.GetJobRequest,
     ) -> open_itag_20220616_models.GetJobResponse:
+        """
+        @summary 获取异步任务Job
+        
+        @param request: GetJobRequest
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_job_with_options_async(tenant_id, job_id, request, headers, runtime)
 
     def get_subtask_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetSubtaskResponse:
+        """
+        @summary 获取单个子任务信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubtaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -786,14 +1139,21 @@
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetSubtaskResponse:
+        """
+        @summary 获取单个子任务信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubtaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -811,37 +1171,54 @@
 
     def get_subtask(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
     ) -> open_itag_20220616_models.GetSubtaskResponse:
+        """
+        @summary 获取单个子任务信息
+        
+        @return: GetSubtaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_subtask_with_options(tenant_id, task_id, subtask_id, headers, runtime)
 
     async def get_subtask_async(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
     ) -> open_itag_20220616_models.GetSubtaskResponse:
+        """
+        @summary 获取单个子任务信息
+        
+        @return: GetSubtaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_subtask_with_options_async(tenant_id, task_id, subtask_id, headers, runtime)
 
     def get_subtask_item_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         item_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+        """
+        @summary 获取子任务单个ITEM信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubtaskItemResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtaskItem',
             version='2022-06-16',
             protocol='HTTPS',
@@ -862,14 +1239,21 @@
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         item_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+        """
+        @summary 获取子任务单个ITEM信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubtaskItemResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetSubtaskItem',
             version='2022-06-16',
             protocol='HTTPS',
@@ -888,36 +1272,53 @@
     def get_subtask_item(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         item_id: str,
     ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+        """
+        @summary 获取子任务单个ITEM信息
+        
+        @return: GetSubtaskItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_subtask_item_with_options(tenant_id, task_id, subtask_id, item_id, headers, runtime)
 
     async def get_subtask_item_async(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         item_id: str,
     ) -> open_itag_20220616_models.GetSubtaskItemResponse:
+        """
+        @summary 获取子任务单个ITEM信息
+        
+        @return: GetSubtaskItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_subtask_item_with_options_async(tenant_id, task_id, subtask_id, item_id, headers, runtime)
 
     def get_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -936,14 +1337,21 @@
     async def get_task_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTask',
             version='2022-06-16',
             protocol='HTTPS',
@@ -960,35 +1368,53 @@
         )
 
     def get_task(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @return: GetTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @return: GetTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_statistics_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskStatisticsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+        """
+        @summary 获取任务统计信息
+        
+        @param request: GetTaskStatisticsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.stat_type):
             query['StatType'] = request.stat_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -1013,14 +1439,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskStatisticsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+        """
+        @summary 获取任务统计信息
+        
+        @param request: GetTaskStatisticsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.stat_type):
             query['StatType'] = request.stat_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -1043,35 +1477,54 @@
 
     def get_task_statistics(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskStatisticsRequest,
     ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+        """
+        @summary 获取任务统计信息
+        
+        @param request: GetTaskStatisticsRequest
+        @return: GetTaskStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_statistics_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def get_task_statistics_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskStatisticsRequest,
     ) -> open_itag_20220616_models.GetTaskStatisticsResponse:
+        """
+        @summary 获取任务统计信息
+        
+        @param request: GetTaskStatisticsRequest
+        @return: GetTaskStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_statistics_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_task_status_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskStatusResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskStatus',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1090,14 +1543,21 @@
     async def get_task_status_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskStatusResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskStatus',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1114,34 +1574,51 @@
         )
 
     def get_task_status(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @return: GetTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_status_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_status_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskStatusResponse:
+        """
+        @summary 获取任务状态信息
+        
+        @return: GetTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_status_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+        """
+        @summary 获取任务模版信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1160,14 +1637,21 @@
     async def get_task_template_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+        """
+        @summary 获取任务模版信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1184,34 +1668,51 @@
         )
 
     def get_task_template(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+        """
+        @summary 获取任务模版信息
+        
+        @return: GetTaskTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_template_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_template_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateResponse:
+        """
+        @summary 获取任务模版信息
+        
+        @return: GetTaskTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_template_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_questions_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateQuestionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateQuestions',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1230,14 +1731,21 @@
     async def get_task_template_questions_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateQuestionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateQuestions',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1254,34 +1762,51 @@
         )
 
     def get_task_template_questions(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @return: GetTaskTemplateQuestionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_template_questions_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_template_questions_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateQuestionsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @return: GetTaskTemplateQuestionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_template_questions_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_template_views_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateViewsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateViews',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1300,14 +1825,21 @@
     async def get_task_template_views_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskTemplateViewsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskTemplateViews',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1324,34 +1856,51 @@
         )
 
     def get_task_template_views(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @return: GetTaskTemplateViewsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_template_views_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_template_views_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskTemplateViewsResponse:
+        """
+        @summary 获取任务题目信息
+        
+        @return: GetTaskTemplateViewsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_template_views_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+        """
+        @summary 获取任务人力
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskWorkforceResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskWorkforce',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1370,14 +1919,21 @@
     async def get_task_workforce_with_options_async(
         self,
         tenant_id: str,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+        """
+        @summary 获取任务人力
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskWorkforceResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskWorkforce',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1394,35 +1950,53 @@
         )
 
     def get_task_workforce(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+        """
+        @summary 获取任务人力
+        
+        @return: GetTaskWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_workforce_with_options(tenant_id, task_id, headers, runtime)
 
     async def get_task_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
     ) -> open_itag_20220616_models.GetTaskWorkforceResponse:
+        """
+        @summary 获取任务人力
+        
+        @return: GetTaskWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_workforce_with_options_async(tenant_id, task_id, headers, runtime)
 
     def get_task_workforce_statistic_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+        """
+        @summary 获取任务人力统计信息
+        
+        @param request: GetTaskWorkforceStatisticRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskWorkforceStatisticResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.stat_type):
@@ -1451,14 +2025,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+        """
+        @summary 获取任务人力统计信息
+        
+        @param request: GetTaskWorkforceStatisticRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskWorkforceStatisticResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.stat_type):
@@ -1485,35 +2067,54 @@
 
     def get_task_workforce_statistic(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
     ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+        """
+        @summary 获取任务人力统计信息
+        
+        @param request: GetTaskWorkforceStatisticRequest
+        @return: GetTaskWorkforceStatisticResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_workforce_statistic_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def get_task_workforce_statistic_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.GetTaskWorkforceStatisticRequest,
     ) -> open_itag_20220616_models.GetTaskWorkforceStatisticResponse:
+        """
+        @summary 获取任务人力统计信息
+        
+        @param request: GetTaskWorkforceStatisticRequest
+        @return: GetTaskWorkforceStatisticResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_workforce_statistic_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def get_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateResponse:
+        """
+        @summary 获取租户下单个模板
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1532,14 +2133,21 @@
     async def get_template_with_options_async(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateResponse:
+        """
+        @summary 获取租户下单个模板
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplate',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1556,34 +2164,51 @@
         )
 
     def get_template(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateResponse:
+        """
+        @summary 获取租户下单个模板
+        
+        @return: GetTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_template_with_options(tenant_id, template_id, headers, runtime)
 
     async def get_template_async(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateResponse:
+        """
+        @summary 获取租户下单个模板
+        
+        @return: GetTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_template_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_template_questions_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+        """
+        @summary 获取租户下单个模板问题
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateQuestionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateQuestions',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1602,14 +2227,21 @@
     async def get_template_questions_with_options_async(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+        """
+        @summary 获取租户下单个模板问题
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateQuestionsResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateQuestions',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1626,34 +2258,51 @@
         )
 
     def get_template_questions(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+        """
+        @summary 获取租户下单个模板问题
+        
+        @return: GetTemplateQuestionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_template_questions_with_options(tenant_id, template_id, headers, runtime)
 
     async def get_template_questions_async(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateQuestionsResponse:
+        """
+        @summary 获取租户下单个模板问题
+        
+        @return: GetTemplateQuestionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_template_questions_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_template_view_with_options(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateViewResponse:
+        """
+        @summary 获取租户下模板视图
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateViewResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateView',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1672,14 +2321,21 @@
     async def get_template_view_with_options_async(
         self,
         tenant_id: str,
         template_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTemplateViewResponse:
+        """
+        @summary 获取租户下模板视图
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTemplateViewResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTemplateView',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1696,33 +2352,50 @@
         )
 
     def get_template_view(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateViewResponse:
+        """
+        @summary 获取租户下模板视图
+        
+        @return: GetTemplateViewResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_template_view_with_options(tenant_id, template_id, headers, runtime)
 
     async def get_template_view_async(
         self,
         tenant_id: str,
         template_id: str,
     ) -> open_itag_20220616_models.GetTemplateViewResponse:
+        """
+        @summary 获取租户下模板视图
+        
+        @return: GetTemplateViewResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_template_view_with_options_async(tenant_id, template_id, headers, runtime)
 
     def get_tenant_with_options(
         self,
         tenant_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTenantResponse:
+        """
+        @summary 获取租户信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTenantResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTenant',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1740,14 +2413,21 @@
 
     async def get_tenant_with_options_async(
         self,
         tenant_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetTenantResponse:
+        """
+        @summary 获取租户信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTenantResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTenant',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1763,33 +2443,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_tenant(
         self,
         tenant_id: str,
     ) -> open_itag_20220616_models.GetTenantResponse:
+        """
+        @summary 获取租户信息
+        
+        @return: GetTenantResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_tenant_with_options(tenant_id, headers, runtime)
 
     async def get_tenant_async(
         self,
         tenant_id: str,
     ) -> open_itag_20220616_models.GetTenantResponse:
+        """
+        @summary 获取租户信息
+        
+        @return: GetTenantResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_tenant_with_options_async(tenant_id, headers, runtime)
 
     def get_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetUserResponse:
+        """
+        @summary 获取用户
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetUser',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1808,14 +2505,21 @@
     async def get_user_with_options_async(
         self,
         tenant_id: str,
         user_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.GetUserResponse:
+        """
+        @summary 获取用户
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetUser',
             version='2022-06-16',
             protocol='HTTPS',
@@ -1832,34 +2536,52 @@
         )
 
     def get_user(
         self,
         tenant_id: str,
         user_id: str,
     ) -> open_itag_20220616_models.GetUserResponse:
+        """
+        @summary 获取用户
+        
+        @return: GetUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_user_with_options(tenant_id, user_id, headers, runtime)
 
     async def get_user_async(
         self,
         tenant_id: str,
         user_id: str,
     ) -> open_itag_20220616_models.GetUserResponse:
+        """
+        @summary 获取用户
+        
+        @return: GetUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_user_with_options_async(tenant_id, user_id, headers, runtime)
 
     def list_jobs_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListJobsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListJobsResponse:
+        """
+        @summary 获取异步任务Job列表
+        
+        @param request: ListJobsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -1887,14 +2609,22 @@
     async def list_jobs_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListJobsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListJobsResponse:
+        """
+        @summary 获取异步任务Job列表
+        
+        @param request: ListJobsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_type):
             query['JobType'] = request.job_type
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -1920,36 +2650,56 @@
         )
 
     def list_jobs(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListJobsRequest,
     ) -> open_itag_20220616_models.ListJobsResponse:
+        """
+        @summary 获取异步任务Job列表
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_jobs_with_options(tenant_id, request, headers, runtime)
 
     async def list_jobs_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListJobsRequest,
     ) -> open_itag_20220616_models.ListJobsResponse:
+        """
+        @summary 获取异步任务Job列表
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_jobs_with_options_async(tenant_id, request, headers, runtime)
 
     def list_subtask_items_with_options(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         request: open_itag_20220616_models.ListSubtaskItemsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        """
+        @summary 获取子任务ITEM列表页信息
+        
+        @param request: ListSubtaskItemsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubtaskItemsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -1977,14 +2727,22 @@
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         request: open_itag_20220616_models.ListSubtaskItemsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        """
+        @summary 获取子任务ITEM列表页信息
+        
+        @param request: ListSubtaskItemsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubtaskItemsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2010,37 +2768,57 @@
     def list_subtask_items(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         request: open_itag_20220616_models.ListSubtaskItemsRequest,
     ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        """
+        @summary 获取子任务ITEM列表页信息
+        
+        @param request: ListSubtaskItemsRequest
+        @return: ListSubtaskItemsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_subtask_items_with_options(tenant_id, task_id, subtask_id, request, headers, runtime)
 
     async def list_subtask_items_async(
         self,
         tenant_id: str,
         task_id: str,
         subtask_id: str,
         request: open_itag_20220616_models.ListSubtaskItemsRequest,
     ) -> open_itag_20220616_models.ListSubtaskItemsResponse:
+        """
+        @summary 获取子任务ITEM列表页信息
+        
+        @param request: ListSubtaskItemsRequest
+        @return: ListSubtaskItemsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_subtask_items_with_options_async(tenant_id, task_id, subtask_id, request, headers, runtime)
 
     def list_subtasks_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ListSubtasksRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListSubtasksResponse:
+        """
+        @summary 获取子任务列表页信息
+        
+        @param request: ListSubtasksRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubtasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2067,14 +2845,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ListSubtasksRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListSubtasksResponse:
+        """
+        @summary 获取子任务列表页信息
+        
+        @param request: ListSubtasksRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubtasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2099,35 +2885,55 @@
 
     def list_subtasks(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ListSubtasksRequest,
     ) -> open_itag_20220616_models.ListSubtasksResponse:
+        """
+        @summary 获取子任务列表页信息
+        
+        @param request: ListSubtasksRequest
+        @return: ListSubtasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_subtasks_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def list_subtasks_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.ListSubtasksRequest,
     ) -> open_itag_20220616_models.ListSubtasksResponse:
+        """
+        @summary 获取子任务列表页信息
+        
+        @param request: ListSubtasksRequest
+        @return: ListSubtasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_subtasks_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def list_tasks_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTasksRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTasksResponse:
+        """
+        @summary 获取任务列表页信息
+        
+        @param request: ListTasksRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2153,14 +2959,22 @@
     async def list_tasks_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTasksRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTasksResponse:
+        """
+        @summary 获取任务列表页信息
+        
+        @param request: ListTasksRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2184,34 +2998,54 @@
         )
 
     def list_tasks(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTasksRequest,
     ) -> open_itag_20220616_models.ListTasksResponse:
+        """
+        @summary 获取任务列表页信息
+        
+        @param request: ListTasksRequest
+        @return: ListTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_tasks_with_options(tenant_id, request, headers, runtime)
 
     async def list_tasks_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTasksRequest,
     ) -> open_itag_20220616_models.ListTasksResponse:
+        """
+        @summary 获取任务列表页信息
+        
+        @param request: ListTasksRequest
+        @return: ListTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_tasks_with_options_async(tenant_id, request, headers, runtime)
 
     def list_templates_with_options(
         self,
         tenant_id: str,
         tmp_req: open_itag_20220616_models.ListTemplatesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTemplatesResponse:
+        """
+        @summary 获取租户模板信息列表
+        
+        @param tmp_req: ListTemplatesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTemplatesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = open_itag_20220616_models.ListTemplatesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.types):
             request.types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.types, 'Types', 'simple')
         query = {}
         if not UtilClient.is_unset(request.page_number):
@@ -2245,14 +3079,22 @@
     async def list_templates_with_options_async(
         self,
         tenant_id: str,
         tmp_req: open_itag_20220616_models.ListTemplatesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTemplatesResponse:
+        """
+        @summary 获取租户模板信息列表
+        
+        @param tmp_req: ListTemplatesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTemplatesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = open_itag_20220616_models.ListTemplatesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.types):
             request.types_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.types, 'Types', 'simple')
         query = {}
         if not UtilClient.is_unset(request.page_number):
@@ -2284,33 +3126,53 @@
         )
 
     def list_templates(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTemplatesRequest,
     ) -> open_itag_20220616_models.ListTemplatesResponse:
+        """
+        @summary 获取租户模板信息列表
+        
+        @param request: ListTemplatesRequest
+        @return: ListTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_templates_with_options(tenant_id, request, headers, runtime)
 
     async def list_templates_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListTemplatesRequest,
     ) -> open_itag_20220616_models.ListTemplatesResponse:
+        """
+        @summary 获取租户模板信息列表
+        
+        @param request: ListTemplatesRequest
+        @return: ListTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_templates_with_options_async(tenant_id, request, headers, runtime)
 
     def list_tenants_with_options(
         self,
         request: open_itag_20220616_models.ListTenantsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTenantsResponse:
+        """
+        @summary 获取租户列表
+        
+        @param request: ListTenantsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTenantsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2335,14 +3197,22 @@
 
     async def list_tenants_with_options_async(
         self,
         request: open_itag_20220616_models.ListTenantsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListTenantsResponse:
+        """
+        @summary 获取租户列表
+        
+        @param request: ListTenantsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTenantsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2365,33 +3235,53 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tenants(
         self,
         request: open_itag_20220616_models.ListTenantsRequest,
     ) -> open_itag_20220616_models.ListTenantsResponse:
+        """
+        @summary 获取租户列表
+        
+        @param request: ListTenantsRequest
+        @return: ListTenantsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_tenants_with_options(request, headers, runtime)
 
     async def list_tenants_async(
         self,
         request: open_itag_20220616_models.ListTenantsRequest,
     ) -> open_itag_20220616_models.ListTenantsResponse:
+        """
+        @summary 获取租户列表
+        
+        @param request: ListTenantsRequest
+        @return: ListTenantsResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_tenants_with_options_async(request, headers, runtime)
 
     def list_users_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListUsersResponse:
+        """
+        @summary 获取用户列表
+        
+        @param request: ListUsersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2417,14 +3307,22 @@
     async def list_users_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.ListUsersResponse:
+        """
+        @summary 获取用户列表
+        
+        @param request: ListUsersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
@@ -2448,36 +3346,56 @@
         )
 
     def list_users(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListUsersRequest,
     ) -> open_itag_20220616_models.ListUsersResponse:
+        """
+        @summary 获取用户列表
+        
+        @param request: ListUsersRequest
+        @return: ListUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_users_with_options(tenant_id, request, headers, runtime)
 
     async def list_users_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.ListUsersRequest,
     ) -> open_itag_20220616_models.ListUsersResponse:
+        """
+        @summary 获取用户列表
+        
+        @param request: ListUsersRequest
+        @return: ListUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_users_with_options_async(tenant_id, request, headers, runtime)
 
     def remove_work_node_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        """
+        @summary 删除结点人力
+        
+        @param request: RemoveWorkNodeWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveWorkNodeWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2503,14 +3421,22 @@
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        """
+        @summary 删除结点人力
+        
+        @param request: RemoveWorkNodeWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveWorkNodeWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_ids):
             body['UserIds'] = request.user_ids
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2534,37 +3460,57 @@
     def remove_work_node_workforce(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
     ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        """
+        @summary 删除结点人力
+        
+        @param request: RemoveWorkNodeWorkforceRequest
+        @return: RemoveWorkNodeWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.remove_work_node_workforce_with_options(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     async def remove_work_node_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
         work_node_id: str,
         request: open_itag_20220616_models.RemoveWorkNodeWorkforceRequest,
     ) -> open_itag_20220616_models.RemoveWorkNodeWorkforceResponse:
+        """
+        @summary 删除结点人力
+        
+        @param request: RemoveWorkNodeWorkforceRequest
+        @return: RemoveWorkNodeWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.remove_work_node_workforce_with_options_async(tenant_id, task_id, work_node_id, request, headers, runtime)
 
     def update_task_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
+        """
+        @summary 更新标注任务基础信息
+        
+        @param request: UpdateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTaskResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTask',
@@ -2586,14 +3532,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
+        """
+        @summary 更新标注任务基础信息
+        
+        @param request: UpdateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTaskResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTask',
@@ -2613,36 +3567,56 @@
 
     def update_task(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskRequest,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
+        """
+        @summary 更新标注任务基础信息
+        
+        @param request: UpdateTaskRequest
+        @return: UpdateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_task_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def update_task_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskRequest,
     ) -> open_itag_20220616_models.UpdateTaskResponse:
+        """
+        @summary 更新标注任务基础信息
+        
+        @param request: UpdateTaskRequest
+        @return: UpdateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_task_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def update_task_workforce_with_options(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        """
+        @summary 更新任务人力
+        
+        @param request: UpdateTaskWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTaskWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.workforce):
             body['Workforce'] = request.workforce
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2667,14 +3641,22 @@
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        """
+        @summary 更新任务人力
+        
+        @param request: UpdateTaskWorkforceRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTaskWorkforceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.workforce):
             body['Workforce'] = request.workforce
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -2697,36 +3679,56 @@
 
     def update_task_workforce(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
     ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        """
+        @summary 更新任务人力
+        
+        @param request: UpdateTaskWorkforceRequest
+        @return: UpdateTaskWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_task_workforce_with_options(tenant_id, task_id, request, headers, runtime)
 
     async def update_task_workforce_async(
         self,
         tenant_id: str,
         task_id: str,
         request: open_itag_20220616_models.UpdateTaskWorkforceRequest,
     ) -> open_itag_20220616_models.UpdateTaskWorkforceResponse:
+        """
+        @summary 更新任务人力
+        
+        @param request: UpdateTaskWorkforceRequest
+        @return: UpdateTaskWorkforceResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_task_workforce_with_options_async(tenant_id, task_id, request, headers, runtime)
 
     def update_template_with_options(
         self,
         tenant_id: str,
         template_id: str,
         request: open_itag_20220616_models.UpdateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        """
+        @summary 更新标注模版
+        
+        @param request: UpdateTemplateRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTemplateResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTemplate',
@@ -2748,14 +3750,22 @@
         self,
         tenant_id: str,
         template_id: str,
         request: open_itag_20220616_models.UpdateTemplateRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        """
+        @summary 更新标注模版
+        
+        @param request: UpdateTemplateRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTemplateResponse
+        """
         UtilClient.validate_model(request)
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(request.body)
         )
         params = open_api_models.Params(
             action='UpdateTemplate',
@@ -2775,35 +3785,55 @@
 
     def update_template(
         self,
         tenant_id: str,
         template_id: str,
         request: open_itag_20220616_models.UpdateTemplateRequest,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        """
+        @summary 更新标注模版
+        
+        @param request: UpdateTemplateRequest
+        @return: UpdateTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_template_with_options(tenant_id, template_id, request, headers, runtime)
 
     async def update_template_async(
         self,
         tenant_id: str,
         template_id: str,
         request: open_itag_20220616_models.UpdateTemplateRequest,
     ) -> open_itag_20220616_models.UpdateTemplateResponse:
+        """
+        @summary 更新标注模版
+        
+        @param request: UpdateTemplateRequest
+        @return: UpdateTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_template_with_options_async(tenant_id, template_id, request, headers, runtime)
 
     def update_tenant_with_options(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.UpdateTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTenantResponse:
+        """
+        @summary 更新租户信息
+        
+        @param request: UpdateTenantRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTenantResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.tenant_name):
             body['TenantName'] = request.tenant_name
         req = open_api_models.OpenApiRequest(
@@ -2829,14 +3859,22 @@
     async def update_tenant_with_options_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.UpdateTenantRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateTenantResponse:
+        """
+        @summary 更新租户信息
+        
+        @param request: UpdateTenantRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTenantResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.tenant_name):
             body['TenantName'] = request.tenant_name
         req = open_api_models.OpenApiRequest(
@@ -2860,35 +3898,55 @@
         )
 
     def update_tenant(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.UpdateTenantRequest,
     ) -> open_itag_20220616_models.UpdateTenantResponse:
+        """
+        @summary 更新租户信息
+        
+        @param request: UpdateTenantRequest
+        @return: UpdateTenantResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_tenant_with_options(tenant_id, request, headers, runtime)
 
     async def update_tenant_async(
         self,
         tenant_id: str,
         request: open_itag_20220616_models.UpdateTenantRequest,
     ) -> open_itag_20220616_models.UpdateTenantResponse:
+        """
+        @summary 更新租户信息
+        
+        @param request: UpdateTenantRequest
+        @return: UpdateTenantResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_tenant_with_options_async(tenant_id, request, headers, runtime)
 
     def update_user_with_options(
         self,
         tenant_id: str,
         user_id: str,
         request: open_itag_20220616_models.UpdateUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateUserResponse:
+        """
+        @summary 更新用户信息
+        
+        @param request: UpdateUserRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.role):
             body['Role'] = request.role
         if not UtilClient.is_unset(request.user_name):
             body['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
@@ -2915,14 +3973,22 @@
         self,
         tenant_id: str,
         user_id: str,
         request: open_itag_20220616_models.UpdateUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> open_itag_20220616_models.UpdateUserResponse:
+        """
+        @summary 更新用户信息
+        
+        @param request: UpdateUserRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.role):
             body['Role'] = request.role
         if not UtilClient.is_unset(request.user_name):
             body['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
@@ -2947,20 +4013,32 @@
 
     def update_user(
         self,
         tenant_id: str,
         user_id: str,
         request: open_itag_20220616_models.UpdateUserRequest,
     ) -> open_itag_20220616_models.UpdateUserResponse:
+        """
+        @summary 更新用户信息
+        
+        @param request: UpdateUserRequest
+        @return: UpdateUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_user_with_options(tenant_id, user_id, request, headers, runtime)
 
     async def update_user_async(
         self,
         tenant_id: str,
         user_id: str,
         request: open_itag_20220616_models.UpdateUserRequest,
     ) -> open_itag_20220616_models.UpdateUserResponse:
+        """
+        @summary 更新用户信息
+        
+        @param request: UpdateUserRequest
+        @return: UpdateUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_user_with_options_async(tenant_id, user_id, request, headers, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616/models.py` & `alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         self,
         dataset_type: str = None,
         source: str = None,
         source_dataset_id: str = None,
     ):
         self.dataset_type = dataset_type
         self.source = source
+        # This parameter is required.
         self.source_dataset_id = source_dataset_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -209,15 +210,17 @@
         key: str = None,
         label: str = None,
         remark: str = None,
         shortcut: str = None,
     ):
         self.children = children
         self.color = color
+        # This parameter is required.
         self.key = key
+        # This parameter is required.
         self.label = label
         self.remark = remark
         self.shortcut = shortcut
 
     def validate(self):
         if self.children:
             for k in self.children:
@@ -425,22 +428,28 @@
         task_workflow: List[CreateTaskDetailTaskWorkflow] = None,
         template_id: str = None,
         uuid: str = None,
         vote_configs: Dict[str, CreateTaskDetailVoteInfo] = None,
     ):
         self.admins = admins
         self.allow_append_data = allow_append_data
+        # This parameter is required.
         self.assign_config = assign_config
+        # This parameter is required.
         self.dataset_proxy_relations = dataset_proxy_relations
         self.exif = exif
         self.tags = tags
+        # This parameter is required.
         self.task_name = task_name
         self.task_template_config = task_template_config
+        # This parameter is required.
         self.task_workflow = task_workflow
+        # This parameter is required.
         self.template_id = template_id
+        # This parameter is required.
         self.uuid = uuid
         self.vote_configs = vote_configs
 
     def validate(self):
         if self.admins:
             self.admins.validate()
         if self.assign_config:
@@ -836,26 +845,32 @@
         select_group: str = None,
         selected: bool = None,
         type: str = None,
     ):
         self.can_select = can_select
         self.children = children
         self.default_result = default_result
+        # This parameter is required.
         self.display = display
         self.exif = exif
         self.hot_key_map = hot_key_map
+        # This parameter is required.
         self.mark_title = mark_title
         self.mark_title_alias = mark_title_alias
+        # This parameter is required.
         self.must_fill = must_fill
+        # This parameter is required.
         self.options = options
         self.pre_options = pre_options
+        # This parameter is required.
         self.question_id = question_id
         self.rule = rule
         self.select_group = select_group
         self.selected = selected
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         if self.children:
             for k in self.children:
                 if k:
                     k.validate()
@@ -2489,22 +2504,26 @@
         exif: Dict[str, Any] = None,
         hide: bool = None,
         plugins: Dict[str, Any] = None,
         relation_question_ids: List[str] = None,
         type: str = None,
         visit_info: ViewPluginVisitInfo = None,
     ):
+        # This parameter is required.
         self.bind_field = bind_field
         self.convertor = convertor
+        # This parameter is required.
         self.cors_proxy = cors_proxy
+        # This parameter is required.
         self.display_ori_img = display_ori_img
         self.exif = exif
         self.hide = hide
         self.plugins = plugins
         self.relation_question_ids = relation_question_ids
+        # This parameter is required.
         self.type = type
         self.visit_info = visit_info
 
     def validate(self):
         if self.visit_info:
             self.visit_info.validate()
 
@@ -2610,20 +2629,23 @@
         template_id: str = None,
         template_name: str = None,
         view_configs: TemplateDTOViewConfigs = None,
     ):
         self.classify = classify
         self.description = description
         self.exif = exif
+        # This parameter is required.
         self.question_configs = question_configs
         self.robot_configs = robot_configs
         self.shared_mode = shared_mode
         self.tags = tags
         self.template_id = template_id
+        # This parameter is required.
         self.template_name = template_name
+        # This parameter is required.
         self.view_configs = view_configs
 
     def validate(self):
         if self.question_configs:
             for k in self.question_configs:
                 if k:
                     k.validate()
@@ -3227,14 +3249,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -3312,19 +3335,149 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddWorkNodeWorkforceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AppendAllDataToTaskRequest(TeaModel):
+    def __init__(
+        self,
+        body: OpenDatasetProxyAppendDataRequest = None,
+    ):
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('body') is not None:
+            temp_model = OpenDatasetProxyAppendDataRequest()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AppendAllDataToTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        details: str = None,
+        error_code: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.details = details
+        self.error_code = error_code
+        # This parameter is required.
+        self.message = message
+        # Id of the request
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.details is not None:
+            result['Details'] = self.details
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Details') is not None:
+            self.details = m.get('Details')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class AppendAllDataToTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AppendAllDataToTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AppendAllDataToTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateTaskRequest(TeaModel):
     def __init__(
         self,
         body: CreateTaskDetail = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -3355,14 +3508,15 @@
         request_id: str = None,
         success: bool = None,
         task_id: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.task_id = task_id
 
     def validate(self):
         pass
@@ -3450,14 +3604,15 @@
 
 
 class CreateTemplateRequest(TeaModel):
     def __init__(
         self,
         body: TemplateDTO = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -3488,14 +3643,15 @@
         request_id: str = None,
         success: bool = None,
         template_id: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.template_id = template_id
 
     def validate(self):
         pass
@@ -3586,16 +3742,19 @@
     def __init__(
         self,
         account_no: str = None,
         account_type: str = None,
         role: str = None,
         user_name: str = None,
     ):
+        # This parameter is required.
         self.account_no = account_no
+        # This parameter is required.
         self.account_type = account_type
+        # This parameter is required.
         self.role = role
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3637,14 +3796,15 @@
         request_id: str = None,
         success: bool = None,
         user_id: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.user_id = user_id
 
     def validate(self):
         pass
@@ -3740,14 +3900,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -3839,14 +4000,15 @@
         request_id: str = None,
         success: bool = None,
         template_id: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.template_id = template_id
 
     def validate(self):
         pass
@@ -3942,14 +4104,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -4034,14 +4197,15 @@
 class ExportAnnotationsRequest(TeaModel):
     def __init__(
         self,
         oss_path: str = None,
         register_dataset: str = None,
         target: str = None,
     ):
+        # This parameter is required.
         self.oss_path = oss_path
         self.register_dataset = register_dataset
         self.target = target
 
     def validate(self):
         pass
 
@@ -4081,14 +4245,15 @@
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
         self.flow_job = flow_job
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         if self.flow_job:
             self.flow_job.validate()
@@ -4214,14 +4379,15 @@
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
         self.job = job
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         if self.job:
             self.job.validate()
@@ -4319,14 +4485,15 @@
         request_id: str = None,
         subtask: SimpleSubtask = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.subtask = subtask
         self.success = success
 
     def validate(self):
         if self.subtask:
@@ -4426,14 +4593,15 @@
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
         self.item = item
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         if self.item:
             self.item.validate()
@@ -4531,14 +4699,15 @@
         request_id: str = None,
         success: bool = None,
         task: TaskDetail = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.task = task
 
     def validate(self):
         if self.task:
@@ -4664,14 +4833,15 @@
         request_id: str = None,
         success: bool = None,
         task_statistics: TaskStatistic = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.task_statistics = task_statistics
 
     def validate(self):
         if self.task_statistics:
@@ -4770,14 +4940,15 @@
         request_id: str = None,
         success: bool = None,
         task_status: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.task_status = task_status
 
     def validate(self):
         pass
@@ -4874,14 +5045,15 @@
         request_id: str = None,
         success: bool = None,
         template: TemplateDetail = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.template = template
 
     def validate(self):
         if self.template:
@@ -4980,14 +5152,15 @@
         questions: List[QuestionPlugin] = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.questions = questions
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         if self.questions:
@@ -5127,14 +5300,15 @@
         request_id: str = None,
         success: bool = None,
         views: GetTaskTemplateViewsResponseBodyViews = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.views = views
 
     def validate(self):
         if self.views:
@@ -5233,14 +5407,15 @@
         request_id: str = None,
         success: bool = None,
         workforce: List[Workforce] = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.workforce = workforce
 
     def validate(self):
         if self.workforce:
@@ -5388,14 +5563,15 @@
         total_count: int = None,
         total_page: int = None,
         users_statistic: List[UserStatistic] = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.total_count = total_count
         self.total_page = total_page
@@ -5520,14 +5696,15 @@
         request_id: str = None,
         success: bool = None,
         template: TemplateDetail = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.template = template
 
     def validate(self):
         if self.template:
@@ -5626,14 +5803,15 @@
         question_configs: List[QuestionPlugin] = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.question_configs = question_configs
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         if self.question_configs:
@@ -5773,14 +5951,15 @@
         request_id: str = None,
         success: bool = None,
         view_configs: GetTemplateViewResponseBodyViewConfigs = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.view_configs = view_configs
 
     def validate(self):
         if self.view_configs:
@@ -5879,14 +6058,15 @@
         request_id: str = None,
         success: bool = None,
         tenant: SingleTenant = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.tenant = tenant
 
     def validate(self):
         if self.tenant:
@@ -5985,14 +6165,15 @@
         request_id: str = None,
         success: bool = None,
         user: SimpleUser = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.user = user
 
     def validate(self):
         if self.user:
@@ -6135,14 +6316,15 @@
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
         self.jobs = jobs
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.total_count = total_count
         self.total_page = total_page
@@ -6304,14 +6486,15 @@
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
         self.items = items
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.total_count = total_count
         self.total_page = total_page
@@ -6472,14 +6655,15 @@
         success: bool = None,
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.subtasks = subtasks
         self.success = success
         self.total_count = total_count
@@ -6641,14 +6825,15 @@
         tasks: List[SimpleTask] = None,
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.tasks = tasks
         self.total_count = total_count
@@ -6867,14 +7052,15 @@
         templates: List[SimpleTemplate] = None,
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.templates = templates
         self.total_count = total_count
@@ -7036,14 +7222,15 @@
         tenants: List[SimpleTenant] = None,
         total_count: int = None,
         total_page: int = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.tenants = tenants
         self.total_count = total_count
@@ -7205,14 +7392,15 @@
         total_count: int = None,
         total_page: int = None,
         users: List[SimpleUser] = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.page_number = page_number
         self.page_size = page_size
         self.request_id = request_id
         self.success = success
         self.total_count = total_count
         self.total_page = total_page
@@ -7363,14 +7551,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -7453,14 +7642,15 @@
 
 
 class UpdateTaskRequest(TeaModel):
     def __init__(
         self,
         body: UpdateTaskDTO = None,
     ):
+        # This parameter is required.
         self.body = body
 
     def validate(self):
         if self.body:
             self.body.validate()
 
     def to_map(self):
@@ -7490,14 +7680,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -7623,14 +7814,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -7751,14 +7943,15 @@
         request_id: str = None,
         success: bool = None,
         template_id: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.template_id = template_id
 
     def validate(self):
         pass
@@ -7887,14 +8080,15 @@
         message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
@@ -7978,15 +8172,17 @@
 
 class UpdateUserRequest(TeaModel):
     def __init__(
         self,
         role: str = None,
         user_name: str = None,
     ):
+        # This parameter is required.
         self.role = role
+        # This parameter is required.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8019,14 +8215,15 @@
         request_id: str = None,
         success: bool = None,
         user_id: str = None,
     ):
         self.code = code
         self.details = details
         self.error_code = error_code
+        # This parameter is required.
         self.message = message
         self.request_id = request_id
         self.success = success
         self.user_id = user_id
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_openitag20220616-1.0.4/alibabacloud_openitag20220616.egg-info/PKG-INFO` & `alibabacloud_openitag20220616-1.1.0/alibabacloud_openitag20220616.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-openitag20220616
-Version: 1.0.4
+Version: 1.1.0
 Summary: Alibaba Cloud OpenITag (20220616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_openitag20220616-1.0.4/setup.py` & `alibabacloud_openitag20220616-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_openitag20220616.
 
-Created on 01/03/2024
+Created on 15/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_openitag20220616"
 NAME = "alibabacloud_openitag20220616" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OpenITag (20220616) SDK Library for Python"
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

