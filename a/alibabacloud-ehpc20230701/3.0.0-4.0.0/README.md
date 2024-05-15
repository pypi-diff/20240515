# Comparing `tmp/alibabacloud_ehpc20230701-3.0.0.tar.gz` & `tmp/alibabacloud_ehpc20230701-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ehpc20230701-3.0.0.tar", last modified: Tue Apr 16 03:01:01 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ehpc20230701-4.0.0.tar", last modified: Wed May 15 07:06:45 2024, max compression
```

## Comparing `alibabacloud_ehpc20230701-3.0.0.tar` & `alibabacloud_ehpc20230701-4.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43481 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/client.py
--rw-r--r--   0 root         (0) root         (0)   139430 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-04-16 03:01:01.000000 alibabacloud_ehpc20230701-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52747 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/client.py
+-rw-r--r--   0 root         (0) root         (0)   140254 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-05-15 07:06:45.000000 alibabacloud_ehpc20230701-4.0.0/setup.py
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/ChangeLog.md` & `alibabacloud_ehpc20230701-4.0.0/ChangeLog.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2024-04-16 Version: 3.0.0
+- Support API DescribeJobMetricData.
+- Support API DescribeJobMetricLast.
+- Update API CreateJob: update param Tasks.
+- Update API ListExecutors: update response param.
+
+
 2024-03-15 Version: 2.2.0
 - Support API ListExecutors.
 - Update API DeleteJobs: add param ExecutorIds.
 
 
 2024-03-13 Version: 2.1.0
 - Support API ListJobExecutors.
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/LICENSE` & `alibabacloud_ehpc20230701-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-3.0.0/PKG-INFO` & `alibabacloud_ehpc20230701-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ehpc20230701
-Version: 3.0.0
+Version: 4.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/README-CN.md` & `alibabacloud_ehpc20230701-4.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-3.0.0/README.md` & `alibabacloud_ehpc20230701-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/client.py` & `alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,32 +42,39 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_image_with_options(
         self,
         tmp_req: ehpc20230701_models.AddImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.AddImageResponse:
+        """
+        @summary 添加托管侧用户自定义镜像
+        
+        @param tmp_req: AddImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddImageResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.AddImageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.container_image_spec):
             request.container_image_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.container_image_spec, 'ContainerImageSpec', 'json')
         if not UtilClient.is_unset(tmp_req.vmimage_spec):
             request.vmimage_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.vmimage_spec, 'VMImageSpec', 'json')
         query = {}
         if not UtilClient.is_unset(request.container_image_spec_shrink):
             query['ContainerImageSpec'] = request.container_image_spec_shrink
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.image_version):
+            query['ImageVersion'] = request.image_version
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.vmimage_spec_shrink):
             query['VMImageSpec'] = request.vmimage_spec_shrink
-        if not UtilClient.is_unset(request.version):
-            query['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='AddImage',
             version='2023-07-01',
             protocol='HTTPS',
@@ -84,32 +91,39 @@
         )
 
     async def add_image_with_options_async(
         self,
         tmp_req: ehpc20230701_models.AddImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.AddImageResponse:
+        """
+        @summary 添加托管侧用户自定义镜像
+        
+        @param tmp_req: AddImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddImageResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.AddImageShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.container_image_spec):
             request.container_image_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.container_image_spec, 'ContainerImageSpec', 'json')
         if not UtilClient.is_unset(tmp_req.vmimage_spec):
             request.vmimage_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.vmimage_spec, 'VMImageSpec', 'json')
         query = {}
         if not UtilClient.is_unset(request.container_image_spec_shrink):
             query['ContainerImageSpec'] = request.container_image_spec_shrink
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.image_version):
+            query['ImageVersion'] = request.image_version
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.vmimage_spec_shrink):
             query['VMImageSpec'] = request.vmimage_spec_shrink
-        if not UtilClient.is_unset(request.version):
-            query['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='AddImage',
             version='2023-07-01',
             protocol='HTTPS',
@@ -125,29 +139,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_image(
         self,
         request: ehpc20230701_models.AddImageRequest,
     ) -> ehpc20230701_models.AddImageResponse:
+        """
+        @summary 添加托管侧用户自定义镜像
+        
+        @param request: AddImageRequest
+        @return: AddImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_image_with_options(request, runtime)
 
     async def add_image_async(
         self,
         request: ehpc20230701_models.AddImageRequest,
     ) -> ehpc20230701_models.AddImageResponse:
+        """
+        @summary 添加托管侧用户自定义镜像
+        
+        @param request: AddImageRequest
+        @return: AddImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_image_with_options_async(request, runtime)
 
     def create_job_with_options(
         self,
         tmp_req: ehpc20230701_models.CreateJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.CreateJobResponse:
+        """
+        @summary 提交任务
+        
+        @param tmp_req: CreateJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateJobResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.CreateJobShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.deployment_policy):
             request.deployment_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.deployment_policy, 'DeploymentPolicy', 'json')
         if not UtilClient.is_unset(tmp_req.tasks):
             request.tasks_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tasks, 'Tasks', 'json')
@@ -180,14 +213,21 @@
         )
 
     async def create_job_with_options_async(
         self,
         tmp_req: ehpc20230701_models.CreateJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.CreateJobResponse:
+        """
+        @summary 提交任务
+        
+        @param tmp_req: CreateJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateJobResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.CreateJobShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.deployment_policy):
             request.deployment_policy_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.deployment_policy, 'DeploymentPolicy', 'json')
         if not UtilClient.is_unset(tmp_req.tasks):
             request.tasks_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tasks, 'Tasks', 'json')
@@ -219,29 +259,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_job(
         self,
         request: ehpc20230701_models.CreateJobRequest,
     ) -> ehpc20230701_models.CreateJobResponse:
+        """
+        @summary 提交任务
+        
+        @param request: CreateJobRequest
+        @return: CreateJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_job_with_options(request, runtime)
 
     async def create_job_async(
         self,
         request: ehpc20230701_models.CreateJobRequest,
     ) -> ehpc20230701_models.CreateJobResponse:
+        """
+        @summary 提交任务
+        
+        @param request: CreateJobRequest
+        @return: CreateJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_job_with_options_async(request, runtime)
 
     def delete_jobs_with_options(
         self,
         tmp_req: ehpc20230701_models.DeleteJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DeleteJobsResponse:
+        """
+        @summary 删除作业
+        
+        @param tmp_req: DeleteJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteJobsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DeleteJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.executor_ids):
             request.executor_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.executor_ids, 'ExecutorIds', 'json')
         if not UtilClient.is_unset(tmp_req.job_spec):
             request.job_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.job_spec, 'JobSpec', 'json')
@@ -270,14 +329,21 @@
         )
 
     async def delete_jobs_with_options_async(
         self,
         tmp_req: ehpc20230701_models.DeleteJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DeleteJobsResponse:
+        """
+        @summary 删除作业
+        
+        @param tmp_req: DeleteJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteJobsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DeleteJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.executor_ids):
             request.executor_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.executor_ids, 'ExecutorIds', 'json')
         if not UtilClient.is_unset(tmp_req.job_spec):
             request.job_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.job_spec, 'JobSpec', 'json')
@@ -305,29 +371,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_jobs(
         self,
         request: ehpc20230701_models.DeleteJobsRequest,
     ) -> ehpc20230701_models.DeleteJobsResponse:
+        """
+        @summary 删除作业
+        
+        @param request: DeleteJobsRequest
+        @return: DeleteJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_jobs_with_options(request, runtime)
 
     async def delete_jobs_async(
         self,
         request: ehpc20230701_models.DeleteJobsRequest,
     ) -> ehpc20230701_models.DeleteJobsResponse:
+        """
+        @summary 删除作业
+        
+        @param request: DeleteJobsRequest
+        @return: DeleteJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_jobs_with_options_async(request, runtime)
 
     def describe_job_metric_data_with_options(
         self,
         tmp_req: ehpc20230701_models.DescribeJobMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        """
+        @summary 查询作业性能数据
+        
+        @param tmp_req: DescribeJobMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMetricDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DescribeJobMetricDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.array_index):
             request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
         query = {}
         if not UtilClient.is_unset(request.array_index_shrink):
@@ -358,14 +443,21 @@
         )
 
     async def describe_job_metric_data_with_options_async(
         self,
         tmp_req: ehpc20230701_models.DescribeJobMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        """
+        @summary 查询作业性能数据
+        
+        @param tmp_req: DescribeJobMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMetricDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DescribeJobMetricDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.array_index):
             request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
         query = {}
         if not UtilClient.is_unset(request.array_index_shrink):
@@ -395,29 +487,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_job_metric_data(
         self,
         request: ehpc20230701_models.DescribeJobMetricDataRequest,
     ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        """
+        @summary 查询作业性能数据
+        
+        @param request: DescribeJobMetricDataRequest
+        @return: DescribeJobMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_job_metric_data_with_options(request, runtime)
 
     async def describe_job_metric_data_async(
         self,
         request: ehpc20230701_models.DescribeJobMetricDataRequest,
     ) -> ehpc20230701_models.DescribeJobMetricDataResponse:
+        """
+        @summary 查询作业性能数据
+        
+        @param request: DescribeJobMetricDataRequest
+        @return: DescribeJobMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_job_metric_data_with_options_async(request, runtime)
 
     def describe_job_metric_last_with_options(
         self,
         tmp_req: ehpc20230701_models.DescribeJobMetricLastRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        """
+        @summary 查询作业即时监控项
+        
+        @param tmp_req: DescribeJobMetricLastRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMetricLastResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DescribeJobMetricLastShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.array_index):
             request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
         query = {}
         if not UtilClient.is_unset(request.array_index_shrink):
@@ -446,14 +557,21 @@
         )
 
     async def describe_job_metric_last_with_options_async(
         self,
         tmp_req: ehpc20230701_models.DescribeJobMetricLastRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        """
+        @summary 查询作业即时监控项
+        
+        @param tmp_req: DescribeJobMetricLastRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMetricLastResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.DescribeJobMetricLastShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.array_index):
             request.array_index_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.array_index, 'ArrayIndex', 'json')
         query = {}
         if not UtilClient.is_unset(request.array_index_shrink):
@@ -481,29 +599,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_job_metric_last(
         self,
         request: ehpc20230701_models.DescribeJobMetricLastRequest,
     ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        """
+        @summary 查询作业即时监控项
+        
+        @param request: DescribeJobMetricLastRequest
+        @return: DescribeJobMetricLastResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_job_metric_last_with_options(request, runtime)
 
     async def describe_job_metric_last_async(
         self,
         request: ehpc20230701_models.DescribeJobMetricLastRequest,
     ) -> ehpc20230701_models.DescribeJobMetricLastResponse:
+        """
+        @summary 查询作业即时监控项
+        
+        @param request: DescribeJobMetricLastRequest
+        @return: DescribeJobMetricLastResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_job_metric_last_with_options_async(request, runtime)
 
     def get_image_with_options(
         self,
         request: ehpc20230701_models.GetImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.GetImageResponse:
+        """
+        @summary 查询托管侧镜像详情。
+        
+        @param request: GetImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetImageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -524,14 +661,21 @@
         )
 
     async def get_image_with_options_async(
         self,
         request: ehpc20230701_models.GetImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.GetImageResponse:
+        """
+        @summary 查询托管侧镜像详情。
+        
+        @param request: GetImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetImageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -551,29 +695,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_image(
         self,
         request: ehpc20230701_models.GetImageRequest,
     ) -> ehpc20230701_models.GetImageResponse:
+        """
+        @summary 查询托管侧镜像详情。
+        
+        @param request: GetImageRequest
+        @return: GetImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_image_with_options(request, runtime)
 
     async def get_image_async(
         self,
         request: ehpc20230701_models.GetImageRequest,
     ) -> ehpc20230701_models.GetImageResponse:
+        """
+        @summary 查询托管侧镜像详情。
+        
+        @param request: GetImageRequest
+        @return: GetImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_image_with_options_async(request, runtime)
 
     def get_job_with_options(
         self,
         request: ehpc20230701_models.GetJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.GetJobResponse:
+        """
+        @summary 查询作业详情
+        
+        @param request: GetJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -594,14 +757,21 @@
         )
 
     async def get_job_with_options_async(
         self,
         request: ehpc20230701_models.GetJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.GetJobResponse:
+        """
+        @summary 查询作业详情
+        
+        @param request: GetJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -621,29 +791,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_job(
         self,
         request: ehpc20230701_models.GetJobRequest,
     ) -> ehpc20230701_models.GetJobResponse:
+        """
+        @summary 查询作业详情
+        
+        @param request: GetJobRequest
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_job_with_options(request, runtime)
 
     async def get_job_async(
         self,
         request: ehpc20230701_models.GetJobRequest,
     ) -> ehpc20230701_models.GetJobResponse:
+        """
+        @summary 查询作业详情
+        
+        @param request: GetJobRequest
+        @return: GetJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_job_with_options_async(request, runtime)
 
     def list_executors_with_options(
         self,
         tmp_req: ehpc20230701_models.ListExecutorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListExecutorsResponse:
+        """
+        @summary 查询全局Executor信息
+        
+        @param tmp_req: ListExecutorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExecutorsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListExecutorsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.filter):
             request.filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter, 'Filter', 'json')
         query = {}
         if not UtilClient.is_unset(request.filter_shrink):
@@ -672,14 +861,21 @@
         )
 
     async def list_executors_with_options_async(
         self,
         tmp_req: ehpc20230701_models.ListExecutorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListExecutorsResponse:
+        """
+        @summary 查询全局Executor信息
+        
+        @param tmp_req: ListExecutorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExecutorsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListExecutorsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.filter):
             request.filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter, 'Filter', 'json')
         query = {}
         if not UtilClient.is_unset(request.filter_shrink):
@@ -707,29 +903,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_executors(
         self,
         request: ehpc20230701_models.ListExecutorsRequest,
     ) -> ehpc20230701_models.ListExecutorsResponse:
+        """
+        @summary 查询全局Executor信息
+        
+        @param request: ListExecutorsRequest
+        @return: ListExecutorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_executors_with_options(request, runtime)
 
     async def list_executors_async(
         self,
         request: ehpc20230701_models.ListExecutorsRequest,
     ) -> ehpc20230701_models.ListExecutorsResponse:
+        """
+        @summary 查询全局Executor信息
+        
+        @param request: ListExecutorsRequest
+        @return: ListExecutorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_executors_with_options_async(request, runtime)
 
     def list_images_with_options(
         self,
         tmp_req: ehpc20230701_models.ListImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListImagesResponse:
+        """
+        @summary 查看托管侧镜像列表
+        
+        @param tmp_req: ListImagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListImagesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListImagesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.image_ids):
             request.image_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_ids, 'ImageIds', 'json')
         if not UtilClient.is_unset(tmp_req.image_names):
             request.image_names_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_names, 'ImageNames', 'json')
@@ -762,14 +977,21 @@
         )
 
     async def list_images_with_options_async(
         self,
         tmp_req: ehpc20230701_models.ListImagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListImagesResponse:
+        """
+        @summary 查看托管侧镜像列表
+        
+        @param tmp_req: ListImagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListImagesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListImagesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.image_ids):
             request.image_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_ids, 'ImageIds', 'json')
         if not UtilClient.is_unset(tmp_req.image_names):
             request.image_names_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.image_names, 'ImageNames', 'json')
@@ -801,29 +1023,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_images(
         self,
         request: ehpc20230701_models.ListImagesRequest,
     ) -> ehpc20230701_models.ListImagesResponse:
+        """
+        @summary 查看托管侧镜像列表
+        
+        @param request: ListImagesRequest
+        @return: ListImagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_images_with_options(request, runtime)
 
     async def list_images_async(
         self,
         request: ehpc20230701_models.ListImagesRequest,
     ) -> ehpc20230701_models.ListImagesResponse:
+        """
+        @summary 查看托管侧镜像列表
+        
+        @param request: ListImagesRequest
+        @return: ListImagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_images_with_options_async(request, runtime)
 
     def list_job_executors_with_options(
         self,
         request: ehpc20230701_models.ListJobExecutorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListJobExecutorsResponse:
+        """
+        @summary 查询作业Executor信息
+        
+        @param request: ListJobExecutorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobExecutorsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -850,14 +1091,21 @@
         )
 
     async def list_job_executors_with_options_async(
         self,
         request: ehpc20230701_models.ListJobExecutorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListJobExecutorsResponse:
+        """
+        @summary 查询作业Executor信息
+        
+        @param request: ListJobExecutorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobExecutorsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -883,29 +1131,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_job_executors(
         self,
         request: ehpc20230701_models.ListJobExecutorsRequest,
     ) -> ehpc20230701_models.ListJobExecutorsResponse:
+        """
+        @summary 查询作业Executor信息
+        
+        @param request: ListJobExecutorsRequest
+        @return: ListJobExecutorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_job_executors_with_options(request, runtime)
 
     async def list_job_executors_async(
         self,
         request: ehpc20230701_models.ListJobExecutorsRequest,
     ) -> ehpc20230701_models.ListJobExecutorsResponse:
+        """
+        @summary 查询作业Executor信息
+        
+        @param request: ListJobExecutorsRequest
+        @return: ListJobExecutorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_job_executors_with_options_async(request, runtime)
 
     def list_jobs_with_options(
         self,
         tmp_req: ehpc20230701_models.ListJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListJobsResponse:
+        """
+        @summary 查询作业列表
+        
+        @param tmp_req: ListJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.filter):
             request.filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter, 'Filter', 'json')
         if not UtilClient.is_unset(tmp_req.sort_by):
             request.sort_by_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.sort_by, 'SortBy', 'json')
@@ -938,14 +1205,21 @@
         )
 
     async def list_jobs_with_options_async(
         self,
         tmp_req: ehpc20230701_models.ListJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.ListJobsResponse:
+        """
+        @summary 查询作业列表
+        
+        @param tmp_req: ListJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListJobsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = ehpc20230701_models.ListJobsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.filter):
             request.filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter, 'Filter', 'json')
         if not UtilClient.is_unset(tmp_req.sort_by):
             request.sort_by_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.sort_by, 'SortBy', 'json')
@@ -977,29 +1251,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_jobs(
         self,
         request: ehpc20230701_models.ListJobsRequest,
     ) -> ehpc20230701_models.ListJobsResponse:
+        """
+        @summary 查询作业列表
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_jobs_with_options(request, runtime)
 
     async def list_jobs_async(
         self,
         request: ehpc20230701_models.ListJobsRequest,
     ) -> ehpc20230701_models.ListJobsResponse:
+        """
+        @summary 查询作业列表
+        
+        @param request: ListJobsRequest
+        @return: ListJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_jobs_with_options_async(request, runtime)
 
     def remove_image_with_options(
         self,
         request: ehpc20230701_models.RemoveImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.RemoveImageResponse:
+        """
+        @summary 移除托管侧镜像信息。
+        
+        @param request: RemoveImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveImageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1020,14 +1313,21 @@
         )
 
     async def remove_image_with_options_async(
         self,
         request: ehpc20230701_models.RemoveImageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ehpc20230701_models.RemoveImageResponse:
+        """
+        @summary 移除托管侧镜像信息。
+        
+        @param request: RemoveImageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveImageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.image_id):
             query['ImageId'] = request.image_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1047,16 +1347,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_image(
         self,
         request: ehpc20230701_models.RemoveImageRequest,
     ) -> ehpc20230701_models.RemoveImageResponse:
+        """
+        @summary 移除托管侧镜像信息。
+        
+        @param request: RemoveImageRequest
+        @return: RemoveImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_image_with_options(request, runtime)
 
     async def remove_image_async(
         self,
         request: ehpc20230701_models.RemoveImageRequest,
     ) -> ehpc20230701_models.RemoveImageResponse:
+        """
+        @summary 移除托管侧镜像信息。
+        
+        @param request: RemoveImageRequest
+        @return: RemoveImageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_image_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701/models.py` & `alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,22 @@
         system_disk: AddonNodeTemplateSystemDisk = None,
     ):
         self.auto_renew = auto_renew
         self.auto_renew_period = auto_renew_period
         self.data_disks = data_disks
         self.duration = duration
         self.enable_ht = enable_ht
+        # This parameter is required.
         self.image_id = image_id
         self.instance_charge_type = instance_charge_type
+        # This parameter is required.
         self.instance_type = instance_type
+        # This parameter is required.
         self.os_name = os_name
+        # This parameter is required.
         self.os_name_en = os_name_en
         self.period = period
         self.period_unit = period_unit
         self.spot_price_limit = spot_price_limit
         self.spot_strategy = spot_strategy
         self.system_disk = system_disk
 
@@ -431,14 +435,15 @@
         self.hostname_suffix = hostname_suffix
         self.initial_count = initial_count
         self.inter_connect = inter_connect
         self.keep_alive_nodes = keep_alive_nodes
         self.max_count = max_count
         self.max_count_per_cycle = max_count_per_cycle
         self.min_count = min_count
+        # This parameter is required.
         self.name = name
         self.ram_role = ram_role
         self.v_switch_ids = v_switch_ids
 
     def validate(self):
         if self.compute_nodes:
             for k in self.compute_nodes:
@@ -700,23 +705,24 @@
 
 
 class AddImageRequest(TeaModel):
     def __init__(
         self,
         container_image_spec: AddImageRequestContainerImageSpec = None,
         description: str = None,
+        image_version: str = None,
         name: str = None,
         vmimage_spec: AddImageRequestVMImageSpec = None,
-        version: str = None,
     ):
         self.container_image_spec = container_image_spec
         self.description = description
+        self.image_version = image_version
+        # This parameter is required.
         self.name = name
         self.vmimage_spec = vmimage_spec
-        self.version = version
 
     def validate(self):
         if self.container_image_spec:
             self.container_image_spec.validate()
         if self.vmimage_spec:
             self.vmimage_spec.validate()
 
@@ -726,87 +732,88 @@
             return _map
 
         result = dict()
         if self.container_image_spec is not None:
             result['ContainerImageSpec'] = self.container_image_spec.to_map()
         if self.description is not None:
             result['Description'] = self.description
+        if self.image_version is not None:
+            result['ImageVersion'] = self.image_version
         if self.name is not None:
             result['Name'] = self.name
         if self.vmimage_spec is not None:
             result['VMImageSpec'] = self.vmimage_spec.to_map()
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ContainerImageSpec') is not None:
             temp_model = AddImageRequestContainerImageSpec()
             self.container_image_spec = temp_model.from_map(m['ContainerImageSpec'])
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('ImageVersion') is not None:
+            self.image_version = m.get('ImageVersion')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('VMImageSpec') is not None:
             temp_model = AddImageRequestVMImageSpec()
             self.vmimage_spec = temp_model.from_map(m['VMImageSpec'])
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class AddImageShrinkRequest(TeaModel):
     def __init__(
         self,
         container_image_spec_shrink: str = None,
         description: str = None,
+        image_version: str = None,
         name: str = None,
         vmimage_spec_shrink: str = None,
-        version: str = None,
     ):
         self.container_image_spec_shrink = container_image_spec_shrink
         self.description = description
+        self.image_version = image_version
+        # This parameter is required.
         self.name = name
         self.vmimage_spec_shrink = vmimage_spec_shrink
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.container_image_spec_shrink is not None:
             result['ContainerImageSpec'] = self.container_image_spec_shrink
         if self.description is not None:
             result['Description'] = self.description
+        if self.image_version is not None:
+            result['ImageVersion'] = self.image_version
         if self.name is not None:
             result['Name'] = self.name
         if self.vmimage_spec_shrink is not None:
             result['VMImageSpec'] = self.vmimage_spec_shrink
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ContainerImageSpec') is not None:
             self.container_image_spec_shrink = m.get('ContainerImageSpec')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('ImageVersion') is not None:
+            self.image_version = m.get('ImageVersion')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('VMImageSpec') is not None:
             self.vmimage_spec_shrink = m.get('VMImageSpec')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class AddImageResponseBody(TeaModel):
     def __init__(
         self,
         image_id: str = None,
@@ -1141,14 +1148,15 @@
         command: List[str] = None,
         environment_vars: List[CreateJobRequestTasksTaskSpecTaskExecutorContainerEnvironmentVars] = None,
         image: str = None,
         working_dir: str = None,
     ):
         self.command = command
         self.environment_vars = environment_vars
+        # This parameter is required.
         self.image = image
         self.working_dir = working_dir
 
     def validate(self):
         if self.environment_vars:
             for k in self.environment_vars:
                 if k:
@@ -1191,14 +1199,15 @@
 class CreateJobRequestTasksTaskSpecTaskExecutorVM(TeaModel):
     def __init__(
         self,
         image: str = None,
         prolog_script: str = None,
         script: str = None,
     ):
+        # This parameter is required.
         self.image = image
         self.prolog_script = prolog_script
         self.script = script
 
     def validate(self):
         pass
 
@@ -1308,14 +1317,15 @@
     def __init__(
         self,
         resource: CreateJobRequestTasksTaskSpecResource = None,
         task_executor: List[CreateJobRequestTasksTaskSpecTaskExecutor] = None,
         volume_mount: List[CreateJobRequestTasksTaskSpecVolumeMount] = None,
     ):
         self.resource = resource
+        # This parameter is required.
         self.task_executor = task_executor
         self.volume_mount = volume_mount
 
     def validate(self):
         if self.resource:
             self.resource.validate()
         if self.task_executor:
@@ -1419,15 +1429,17 @@
         deployment_policy: CreateJobRequestDeploymentPolicy = None,
         job_description: str = None,
         job_name: str = None,
         tasks: List[CreateJobRequestTasks] = None,
     ):
         self.deployment_policy = deployment_policy
         self.job_description = job_description
+        # This parameter is required.
         self.job_name = job_name
+        # This parameter is required.
         self.tasks = tasks
 
     def validate(self):
         if self.deployment_policy:
             self.deployment_policy.validate()
         if self.tasks:
             for k in self.tasks:
@@ -1475,15 +1487,17 @@
         deployment_policy_shrink: str = None,
         job_description: str = None,
         job_name: str = None,
         tasks_shrink: str = None,
     ):
         self.deployment_policy_shrink = deployment_policy_shrink
         self.job_description = job_description
+        # This parameter is required.
         self.job_name = job_name
+        # This parameter is required.
         self.tasks_shrink = tasks_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2170,14 +2184,15 @@
 
 
 class GetImageRequest(TeaModel):
     def __init__(
         self,
         image_id: str = None,
     ):
+        # This parameter is required.
         self.image_id = image_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2344,14 +2359,15 @@
         size: str = None,
         vmimage_spec: GetImageResponseBodyImageVMImageSpec = None,
         version: str = None,
     ):
         self.container_image_spec = container_image_spec
         self.create_time = create_time
         self.description = description
+        # This parameter is required.
         self.image_type = image_type
         self.name = name
         self.size = size
         self.vmimage_spec = vmimage_spec
         self.version = version
 
     def validate(self):
@@ -3551,15 +3567,17 @@
         image_id: str = None,
         image_type: str = None,
         name: str = None,
         version: str = None,
     ):
         self.create_time = create_time
         self.description = description
+        # This parameter is required.
         self.image_id = image_id
+        # This parameter is required.
         self.image_type = image_type
         self.name = name
         self.version = version
 
     def validate(self):
         pass
 
@@ -4296,14 +4314,15 @@
 
 
 class RemoveImageRequest(TeaModel):
     def __init__(
         self,
         image_id: str = None,
     ):
+        # This parameter is required.
         self.image_id = image_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO` & `alibabacloud_ehpc20230701-4.0.0/alibabacloud_ehpc20230701.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ehpc20230701
-Version: 3.0.0
+Version: 4.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20230701-3.0.0/setup.py` & `alibabacloud_ehpc20230701-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ehpc20230701.
 
-Created on 16/04/2024
+Created on 15/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ehpc20230701"
 NAME = "alibabacloud_ehpc20230701" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elastic High Performance Computing (20230701) SDK Library for Python"
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

