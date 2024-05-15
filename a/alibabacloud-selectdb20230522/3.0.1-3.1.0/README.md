# Comparing `tmp/alibabacloud_selectdb20230522-3.0.1.tar.gz` & `tmp/alibabacloud_selectdb20230522-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_selectdb20230522-3.0.1.tar", last modified: Fri Mar 15 17:13:57 2024, max compression
+gzip compressed data, was "dist/alibabacloud_selectdb20230522-3.1.0.tar", last modified: Wed May 15 17:11:41 2024, max compression
```

## Comparing `alibabacloud_selectdb20230522-3.0.1.tar` & `alibabacloud_selectdb20230522-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/
--rw-r--r--   0 root         (0) root         (0)      284 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83390 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522/client.py
--rw-r--r--   0 root         (0) root         (0)   131259 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-15 17:13:57.000000 alibabacloud_selectdb20230522-3.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-15 17:13:56.000000 alibabacloud_selectdb20230522-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122590 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522/client.py
+-rw-r--r--   0 root         (0) root         (0)   173402 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-15 17:11:41.000000 alibabacloud_selectdb20230522-3.1.0/setup.py
```

### Comparing `alibabacloud_selectdb20230522-3.0.1/LICENSE` & `alibabacloud_selectdb20230522-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_selectdb20230522-3.0.1/PKG-INFO` & `alibabacloud_selectdb20230522-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_selectdb20230522
-Version: 3.0.1
+Version: 3.1.0
 Summary: Alibaba Cloud selectdb (20230522) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_selectdb20230522-3.0.1/README-CN.md` & `alibabacloud_selectdb20230522-3.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_selectdb20230522-3.0.1/README.md` & `alibabacloud_selectdb20230522-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522/models.py` & `alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,21 @@
         self,
         connection_string_prefix: str = None,
         dbinstance_id: str = None,
         net_type: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.connection_string_prefix = connection_string_prefix
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.net_type = net_type
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -152,31 +156,40 @@
         resource_owner_id: int = None,
         security_iplist: str = None,
         used_time: int = None,
         v_switch_id: str = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
+        # This parameter is required.
         self.cache_size = cache_size
+        # This parameter is required.
         self.charge_type = charge_type
         self.client_token = client_token
         self.connection_string = connection_string
+        # This parameter is required.
         self.dbinstance_class = dbinstance_class
         self.dbinstance_description = dbinstance_description
         self.engine = engine
+        # This parameter is required.
         self.engine_version = engine_version
         self.period = period
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
         self.security_iplist = security_iplist
         self.used_time = used_time
+        # This parameter is required.
         self.v_switch_id = v_switch_id
         # VPC ID。
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
+        # This parameter is required.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -449,31 +462,43 @@
         resource_group_id: str = None,
         resource_owner_id: int = None,
         used_time: str = None,
         v_switch_id: str = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
+        # This parameter is required.
         self.cache_size = cache_size
+        # This parameter is required.
         self.charge_type = charge_type
+        # This parameter is required.
         self.dbcluster_class = dbcluster_class
+        # This parameter is required.
         self.dbcluster_description = dbcluster_description
         # 代表资源一级ID的资源属性字段
+        # 
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
         self.engine = engine
+        # This parameter is required.
         self.engine_version = engine_version
         self.period = period
+        # This parameter is required.
         self.region_id = region_id
         # 代表资源组的资源属性字段
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
         self.used_time = used_time
+        # This parameter is required.
         self.v_switch_id = v_switch_id
         # VPC ID。
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
+        # This parameter is required.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -674,32 +699,41 @@
         resource_owner_id: int = None,
         security_iplist: str = None,
         used_time: int = None,
         v_switch_id: str = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
+        # This parameter is required.
         self.cache_size = cache_size
+        # This parameter is required.
         self.charge_type = charge_type
         self.client_token = client_token
         self.connection_string = connection_string
+        # This parameter is required.
         self.dbinstance_class = dbinstance_class
         self.dbinstance_description = dbinstance_description
         self.engine = engine
+        # This parameter is required.
         self.engine_version = engine_version
         self.period = period
+        # This parameter is required.
         self.region_id = region_id
         # 代表资源组的资源属性字段
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
         self.security_iplist = security_iplist
         self.used_time = used_time
+        # This parameter is required.
         self.v_switch_id = v_switch_id
         # VPC ID。
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
+        # This parameter is required.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -997,17 +1031,21 @@
         self,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # 代表资源一级ID的资源属性字段
+        # 
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         # 代表资源组的资源属性字段
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -1157,15 +1195,17 @@
 class DeleteDBInstanceRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1257,22 +1297,573 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDBInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDBClusterConfigRequest(TeaModel):
+    def __init__(
+        self,
+        config_key: str = None,
+        dbcluster_id: str = None,
+        dbinstance_id: str = None,
+        region_id: str = None,
+    ):
+        # This parameter is required.
+        self.config_key = config_key
+        # This parameter is required.
+        self.dbcluster_id = dbcluster_id
+        # This parameter is required.
+        self.dbinstance_id = dbinstance_id
+        self.region_id = region_id
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
+        if self.config_key is not None:
+            result['ConfigKey'] = self.config_key
+        if self.dbcluster_id is not None:
+            result['DBClusterId'] = self.dbcluster_id
+        if self.dbinstance_id is not None:
+            result['DBInstanceId'] = self.dbinstance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConfigKey') is not None:
+            self.config_key = m.get('ConfigKey')
+        if m.get('DBClusterId') is not None:
+            self.dbcluster_id = m.get('DBClusterId')
+        if m.get('DBInstanceId') is not None:
+            self.dbinstance_id = m.get('DBInstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DescribeDBClusterConfigResponseBodyDataParams(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        default_value: str = None,
+        is_dynamic: int = None,
+        is_user_modifiable: int = None,
+        name: str = None,
+        optional: str = None,
+        param_category: str = None,
+        value: str = None,
+    ):
+        self.comment = comment
+        self.default_value = default_value
+        self.is_dynamic = is_dynamic
+        self.is_user_modifiable = is_user_modifiable
+        self.name = name
+        self.optional = optional
+        self.param_category = param_category
+        self.value = value
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
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.default_value is not None:
+            result['DefaultValue'] = self.default_value
+        if self.is_dynamic is not None:
+            result['IsDynamic'] = self.is_dynamic
+        if self.is_user_modifiable is not None:
+            result['IsUserModifiable'] = self.is_user_modifiable
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.optional is not None:
+            result['Optional'] = self.optional
+        if self.param_category is not None:
+            result['ParamCategory'] = self.param_category
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DefaultValue') is not None:
+            self.default_value = m.get('DefaultValue')
+        if m.get('IsDynamic') is not None:
+            self.is_dynamic = m.get('IsDynamic')
+        if m.get('IsUserModifiable') is not None:
+            self.is_user_modifiable = m.get('IsUserModifiable')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Optional') is not None:
+            self.optional = m.get('Optional')
+        if m.get('ParamCategory') is not None:
+            self.param_category = m.get('ParamCategory')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDBClusterConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        db_cluster_id: str = None,
+        db_instance_id: str = None,
+        db_instance_name: str = None,
+        params: List[DescribeDBClusterConfigResponseBodyDataParams] = None,
+        task_id: int = None,
+    ):
+        self.db_cluster_id = db_cluster_id
+        self.db_instance_id = db_instance_id
+        self.db_instance_name = db_instance_name
+        self.params = params
+        self.task_id = task_id
+
+    def validate(self):
+        if self.params:
+            for k in self.params:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_cluster_id is not None:
+            result['DbClusterId'] = self.db_cluster_id
+        if self.db_instance_id is not None:
+            result['DbInstanceId'] = self.db_instance_id
+        if self.db_instance_name is not None:
+            result['DbInstanceName'] = self.db_instance_name
+        result['Params'] = []
+        if self.params is not None:
+            for k in self.params:
+                result['Params'].append(k.to_map() if k else None)
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbClusterId') is not None:
+            self.db_cluster_id = m.get('DbClusterId')
+        if m.get('DbInstanceId') is not None:
+            self.db_instance_id = m.get('DbInstanceId')
+        if m.get('DbInstanceName') is not None:
+            self.db_instance_name = m.get('DbInstanceName')
+        self.params = []
+        if m.get('Params') is not None:
+            for k in m.get('Params'):
+                temp_model = DescribeDBClusterConfigResponseBodyDataParams()
+                self.params.append(temp_model.from_map(k))
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class DescribeDBClusterConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_denied_detail: str = None,
+        data: DescribeDBClusterConfigResponseBodyData = None,
+        dynamic_code: str = None,
+        dynamic_message: str = None,
+        request_id: str = None,
+    ):
+        self.access_denied_detail = access_denied_detail
+        self.data = data
+        self.dynamic_code = dynamic_code
+        self.dynamic_message = dynamic_message
+        self.request_id = request_id
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
+        if self.access_denied_detail is not None:
+            result['AccessDeniedDetail'] = self.access_denied_detail
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.dynamic_code is not None:
+            result['DynamicCode'] = self.dynamic_code
+        if self.dynamic_message is not None:
+            result['DynamicMessage'] = self.dynamic_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessDeniedDetail') is not None:
+            self.access_denied_detail = m.get('AccessDeniedDetail')
+        if m.get('Data') is not None:
+            temp_model = DescribeDBClusterConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('DynamicCode') is not None:
+            self.dynamic_code = m.get('DynamicCode')
+        if m.get('DynamicMessage') is not None:
+            self.dynamic_message = m.get('DynamicMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeDBClusterConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDBClusterConfigResponseBody = None,
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
+            temp_model = DescribeDBClusterConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDBClusterConfigChangeLogsRequest(TeaModel):
+    def __init__(
+        self,
+        config_key: str = None,
+        dbcluster_id: str = None,
+        dbinstance_id: str = None,
+        end_time: str = None,
+        region_id: str = None,
+        start_time: str = None,
+    ):
+        # This parameter is required.
+        self.config_key = config_key
+        # This parameter is required.
+        self.dbcluster_id = dbcluster_id
+        # This parameter is required.
+        self.dbinstance_id = dbinstance_id
+        # This parameter is required.
+        self.end_time = end_time
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.start_time = start_time
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
+        if self.config_key is not None:
+            result['ConfigKey'] = self.config_key
+        if self.dbcluster_id is not None:
+            result['DBClusterId'] = self.dbcluster_id
+        if self.dbinstance_id is not None:
+            result['DBInstanceId'] = self.dbinstance_id
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConfigKey') is not None:
+            self.config_key = m.get('ConfigKey')
+        if m.get('DBClusterId') is not None:
+            self.dbcluster_id = m.get('DBClusterId')
+        if m.get('DBInstanceId') is not None:
+            self.dbinstance_id = m.get('DBInstanceId')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeDBClusterConfigChangeLogsResponseBodyDataParamChangeLogs(TeaModel):
+    def __init__(
+        self,
+        gmt_created: str = None,
+        gmt_modified: str = None,
+        id: int = None,
+        is_applied: bool = None,
+        name: str = None,
+        new_value: str = None,
+        old_value: str = None,
+    ):
+        self.gmt_created = gmt_created
+        self.gmt_modified = gmt_modified
+        self.id = id
+        self.is_applied = is_applied
+        self.name = name
+        self.new_value = new_value
+        self.old_value = old_value
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
+        if self.gmt_created is not None:
+            result['GmtCreated'] = self.gmt_created
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.is_applied is not None:
+            result['IsApplied'] = self.is_applied
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.new_value is not None:
+            result['NewValue'] = self.new_value
+        if self.old_value is not None:
+            result['OldValue'] = self.old_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GmtCreated') is not None:
+            self.gmt_created = m.get('GmtCreated')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IsApplied') is not None:
+            self.is_applied = m.get('IsApplied')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('NewValue') is not None:
+            self.new_value = m.get('NewValue')
+        if m.get('OldValue') is not None:
+            self.old_value = m.get('OldValue')
+        return self
+
+
+class DescribeDBClusterConfigChangeLogsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        db_cluster_id: str = None,
+        db_instance_id: str = None,
+        db_instance_name: str = None,
+        param_change_logs: List[DescribeDBClusterConfigChangeLogsResponseBodyDataParamChangeLogs] = None,
+        task_id: int = None,
+    ):
+        self.db_cluster_id = db_cluster_id
+        self.db_instance_id = db_instance_id
+        self.db_instance_name = db_instance_name
+        self.param_change_logs = param_change_logs
+        self.task_id = task_id
+
+    def validate(self):
+        if self.param_change_logs:
+            for k in self.param_change_logs:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_cluster_id is not None:
+            result['DbClusterId'] = self.db_cluster_id
+        if self.db_instance_id is not None:
+            result['DbInstanceId'] = self.db_instance_id
+        if self.db_instance_name is not None:
+            result['DbInstanceName'] = self.db_instance_name
+        result['ParamChangeLogs'] = []
+        if self.param_change_logs is not None:
+            for k in self.param_change_logs:
+                result['ParamChangeLogs'].append(k.to_map() if k else None)
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbClusterId') is not None:
+            self.db_cluster_id = m.get('DbClusterId')
+        if m.get('DbInstanceId') is not None:
+            self.db_instance_id = m.get('DbInstanceId')
+        if m.get('DbInstanceName') is not None:
+            self.db_instance_name = m.get('DbInstanceName')
+        self.param_change_logs = []
+        if m.get('ParamChangeLogs') is not None:
+            for k in m.get('ParamChangeLogs'):
+                temp_model = DescribeDBClusterConfigChangeLogsResponseBodyDataParamChangeLogs()
+                self.param_change_logs.append(temp_model.from_map(k))
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class DescribeDBClusterConfigChangeLogsResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_denied_detail: str = None,
+        data: DescribeDBClusterConfigChangeLogsResponseBodyData = None,
+        dynamic_code: str = None,
+        dynamic_message: str = None,
+        request_id: str = None,
+    ):
+        self.access_denied_detail = access_denied_detail
+        self.data = data
+        self.dynamic_code = dynamic_code
+        self.dynamic_message = dynamic_message
+        self.request_id = request_id
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
+        if self.access_denied_detail is not None:
+            result['AccessDeniedDetail'] = self.access_denied_detail
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.dynamic_code is not None:
+            result['DynamicCode'] = self.dynamic_code
+        if self.dynamic_message is not None:
+            result['DynamicMessage'] = self.dynamic_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessDeniedDetail') is not None:
+            self.access_denied_detail = m.get('AccessDeniedDetail')
+        if m.get('Data') is not None:
+            temp_model = DescribeDBClusterConfigChangeLogsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('DynamicCode') is not None:
+            self.dynamic_code = m.get('DynamicCode')
+        if m.get('DynamicMessage') is not None:
+            self.dynamic_message = m.get('DynamicMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeDBClusterConfigChangeLogsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDBClusterConfigChangeLogsResponseBody = None,
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
+            temp_model = DescribeDBClusterConfigChangeLogsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDBInstanceAttributeRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1604,15 +2195,17 @@
 class DescribeDBInstanceNetInfoRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1983,14 +2576,15 @@
         resource_owner_id: int = None,
     ):
         self.dbinstance_description = dbinstance_description
         self.dbinstance_ids = dbinstance_ids
         self.dbinstance_status = dbinstance_status
         self.page_number = page_number
         self.page_size = page_size
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -2433,15 +3027,17 @@
 class DescribeSecurityIPListRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2604,29 +3200,443 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSecurityIPListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetCreateBEClusterInquiryRequest(TeaModel):
+    def __init__(
+        self,
+        cache_size: int = None,
+        charge_type: str = None,
+        commodity_code: str = None,
+        compute_size: int = None,
+        db_instance_id: str = None,
+        pre_cache_size: int = None,
+        pre_compute_size: int = None,
+        pricing_cycle: str = None,
+        quantity: int = None,
+        region_id: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.cache_size = cache_size
+        # This parameter is required.
+        self.charge_type = charge_type
+        self.commodity_code = commodity_code
+        self.compute_size = compute_size
+        # This parameter is required.
+        self.db_instance_id = db_instance_id
+        self.pre_cache_size = pre_cache_size
+        self.pre_compute_size = pre_compute_size
+        # This parameter is required.
+        self.pricing_cycle = pricing_cycle
+        # This parameter is required.
+        self.quantity = quantity
+        # This parameter is required.
+        self.region_id = region_id
+        self.resource_owner_id = resource_owner_id
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
+        if self.cache_size is not None:
+            result['CacheSize'] = self.cache_size
+        if self.charge_type is not None:
+            result['ChargeType'] = self.charge_type
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.compute_size is not None:
+            result['ComputeSize'] = self.compute_size
+        if self.db_instance_id is not None:
+            result['DbInstanceId'] = self.db_instance_id
+        if self.pre_cache_size is not None:
+            result['PreCacheSize'] = self.pre_cache_size
+        if self.pre_compute_size is not None:
+            result['PreComputeSize'] = self.pre_compute_size
+        if self.pricing_cycle is not None:
+            result['PricingCycle'] = self.pricing_cycle
+        if self.quantity is not None:
+            result['Quantity'] = self.quantity
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CacheSize') is not None:
+            self.cache_size = m.get('CacheSize')
+        if m.get('ChargeType') is not None:
+            self.charge_type = m.get('ChargeType')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('ComputeSize') is not None:
+            self.compute_size = m.get('ComputeSize')
+        if m.get('DbInstanceId') is not None:
+            self.db_instance_id = m.get('DbInstanceId')
+        if m.get('PreCacheSize') is not None:
+            self.pre_cache_size = m.get('PreCacheSize')
+        if m.get('PreComputeSize') is not None:
+            self.pre_compute_size = m.get('PreComputeSize')
+        if m.get('PricingCycle') is not None:
+            self.pricing_cycle = m.get('PricingCycle')
+        if m.get('Quantity') is not None:
+            self.quantity = m.get('Quantity')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class GetCreateBEClusterInquiryResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        currency: str = None,
+        trade_amount: str = None,
+    ):
+        self.currency = currency
+        self.trade_amount = trade_amount
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
+        if self.currency is not None:
+            result['Currency'] = self.currency
+        if self.trade_amount is not None:
+            result['TradeAmount'] = self.trade_amount
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Currency') is not None:
+            self.currency = m.get('Currency')
+        if m.get('TradeAmount') is not None:
+            self.trade_amount = m.get('TradeAmount')
+        return self
+
+
+class GetCreateBEClusterInquiryResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: GetCreateBEClusterInquiryResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
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
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetCreateBEClusterInquiryResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetCreateBEClusterInquiryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetCreateBEClusterInquiryResponseBody = None,
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
+            temp_model = GetCreateBEClusterInquiryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetModifyBEClusterInquiryRequest(TeaModel):
+    def __init__(
+        self,
+        cache_size: int = None,
+        charge_type: str = None,
+        cluster_id: str = None,
+        commodity_code: str = None,
+        compute_size: int = None,
+        db_instance_id: str = None,
+        pre_cache_size: int = None,
+        pre_compute_size: int = None,
+        pricing_cycle: str = None,
+        quantity: int = None,
+        region_id: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.cache_size = cache_size
+        # This parameter is required.
+        self.charge_type = charge_type
+        self.cluster_id = cluster_id
+        # This parameter is required.
+        self.commodity_code = commodity_code
+        self.compute_size = compute_size
+        # This parameter is required.
+        self.db_instance_id = db_instance_id
+        self.pre_cache_size = pre_cache_size
+        self.pre_compute_size = pre_compute_size
+        # This parameter is required.
+        self.pricing_cycle = pricing_cycle
+        # This parameter is required.
+        self.quantity = quantity
+        # This parameter is required.
+        self.region_id = region_id
+        self.resource_owner_id = resource_owner_id
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
+        if self.cache_size is not None:
+            result['CacheSize'] = self.cache_size
+        if self.charge_type is not None:
+            result['ChargeType'] = self.charge_type
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.compute_size is not None:
+            result['ComputeSize'] = self.compute_size
+        if self.db_instance_id is not None:
+            result['DbInstanceId'] = self.db_instance_id
+        if self.pre_cache_size is not None:
+            result['PreCacheSize'] = self.pre_cache_size
+        if self.pre_compute_size is not None:
+            result['PreComputeSize'] = self.pre_compute_size
+        if self.pricing_cycle is not None:
+            result['PricingCycle'] = self.pricing_cycle
+        if self.quantity is not None:
+            result['Quantity'] = self.quantity
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CacheSize') is not None:
+            self.cache_size = m.get('CacheSize')
+        if m.get('ChargeType') is not None:
+            self.charge_type = m.get('ChargeType')
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('ComputeSize') is not None:
+            self.compute_size = m.get('ComputeSize')
+        if m.get('DbInstanceId') is not None:
+            self.db_instance_id = m.get('DbInstanceId')
+        if m.get('PreCacheSize') is not None:
+            self.pre_cache_size = m.get('PreCacheSize')
+        if m.get('PreComputeSize') is not None:
+            self.pre_compute_size = m.get('PreComputeSize')
+        if m.get('PricingCycle') is not None:
+            self.pricing_cycle = m.get('PricingCycle')
+        if m.get('Quantity') is not None:
+            self.quantity = m.get('Quantity')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class GetModifyBEClusterInquiryResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        currency: str = None,
+        trade_amount: str = None,
+    ):
+        self.currency = currency
+        self.trade_amount = trade_amount
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
+        if self.currency is not None:
+            result['Currency'] = self.currency
+        if self.trade_amount is not None:
+            result['TradeAmount'] = self.trade_amount
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Currency') is not None:
+            self.currency = m.get('Currency')
+        if m.get('TradeAmount') is not None:
+            self.trade_amount = m.get('TradeAmount')
+        return self
+
+
+class GetModifyBEClusterInquiryResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: GetModifyBEClusterInquiryResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
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
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetModifyBEClusterInquiryResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetModifyBEClusterInquiryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetModifyBEClusterInquiryResponseBody = None,
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
+            temp_model = GetModifyBEClusterInquiryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyBEClusterAttributeRequest(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         instance_attribute_type: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
         value: str = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.instance_attribute_type = instance_attribute_type
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2739,18 +3749,22 @@
         dbcluster_class: str = None,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         engine: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_class = dbcluster_class
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
         self.engine = engine
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2908,27 +3922,231 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDBClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDBClusterConfigRequest(TeaModel):
+    def __init__(
+        self,
+        config_key: str = None,
+        dbcluster_id: str = None,
+        dbinstance_id: str = None,
+        parameters: str = None,
+        region_id: str = None,
+        switch_time_mode: str = None,
+    ):
+        # This parameter is required.
+        self.config_key = config_key
+        # This parameter is required.
+        self.dbcluster_id = dbcluster_id
+        # This parameter is required.
+        self.dbinstance_id = dbinstance_id
+        # This parameter is required.
+        self.parameters = parameters
+        self.region_id = region_id
+        self.switch_time_mode = switch_time_mode
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
+        if self.config_key is not None:
+            result['ConfigKey'] = self.config_key
+        if self.dbcluster_id is not None:
+            result['DBClusterId'] = self.dbcluster_id
+        if self.dbinstance_id is not None:
+            result['DBInstanceId'] = self.dbinstance_id
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.switch_time_mode is not None:
+            result['SwitchTimeMode'] = self.switch_time_mode
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConfigKey') is not None:
+            self.config_key = m.get('ConfigKey')
+        if m.get('DBClusterId') is not None:
+            self.dbcluster_id = m.get('DBClusterId')
+        if m.get('DBInstanceId') is not None:
+            self.dbinstance_id = m.get('DBInstanceId')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SwitchTimeMode') is not None:
+            self.switch_time_mode = m.get('SwitchTimeMode')
+        return self
+
+
+class ModifyDBClusterConfigResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        db_cluster_id: str = None,
+        db_instance_id: str = None,
+        db_instance_name: str = None,
+        task_id: int = None,
+    ):
+        self.db_cluster_id = db_cluster_id
+        self.db_instance_id = db_instance_id
+        self.db_instance_name = db_instance_name
+        self.task_id = task_id
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
+        if self.db_cluster_id is not None:
+            result['DbClusterId'] = self.db_cluster_id
+        if self.db_instance_id is not None:
+            result['DbInstanceId'] = self.db_instance_id
+        if self.db_instance_name is not None:
+            result['DbInstanceName'] = self.db_instance_name
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbClusterId') is not None:
+            self.db_cluster_id = m.get('DbClusterId')
+        if m.get('DbInstanceId') is not None:
+            self.db_instance_id = m.get('DbInstanceId')
+        if m.get('DbInstanceName') is not None:
+            self.db_instance_name = m.get('DbInstanceName')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class ModifyDBClusterConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_denied_detail: str = None,
+        data: ModifyDBClusterConfigResponseBodyData = None,
+        dynamic_code: str = None,
+        dynamic_message: str = None,
+        request_id: str = None,
+    ):
+        self.access_denied_detail = access_denied_detail
+        self.data = data
+        self.dynamic_code = dynamic_code
+        self.dynamic_message = dynamic_message
+        self.request_id = request_id
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
+        if self.access_denied_detail is not None:
+            result['AccessDeniedDetail'] = self.access_denied_detail
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.dynamic_code is not None:
+            result['DynamicCode'] = self.dynamic_code
+        if self.dynamic_message is not None:
+            result['DynamicMessage'] = self.dynamic_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessDeniedDetail') is not None:
+            self.access_denied_detail = m.get('AccessDeniedDetail')
+        if m.get('Data') is not None:
+            temp_model = ModifyDBClusterConfigResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('DynamicCode') is not None:
+            self.dynamic_code = m.get('DynamicCode')
+        if m.get('DynamicMessage') is not None:
+            self.dynamic_message = m.get('DynamicMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDBClusterConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyDBClusterConfigResponseBody = None,
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
+            temp_model = ModifyDBClusterConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyDBInstanceAttributeRequest(TeaModel):
     def __init__(
         self,
         dbinstance_id: str = None,
         instance_attribute_type: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
         value: str = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.instance_attribute_type = instance_attribute_type
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3037,19 +4255,24 @@
         dbinstance_id: str = None,
         group_name: str = None,
         modify_mode: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
         security_iplist: str = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.group_name = group_name
+        # This parameter is required.
         self.modify_mode = modify_mode
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.security_iplist = security_iplist
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3202,16 +4425,19 @@
     def __init__(
         self,
         connection_string: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.connection_string = connection_string
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3316,17 +4542,21 @@
         self,
         account_name: str = None,
         account_password: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
+        # This parameter is required.
         self.account_password = account_password
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3435,18 +4665,23 @@
         self,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # 代表资源一级ID的资源属性字段
+        # 
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
         # 地域
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # 资源组id
         self.resource_group_id = resource_group_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
@@ -3597,16 +4832,19 @@
     def __init__(
         self,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3710,16 +4948,19 @@
     def __init__(
         self,
         dbcluster_id: str = None,
         dbinstance_id: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3824,16 +5065,19 @@
         self,
         dbinstance_id: str = None,
         engine_version: str = None,
         region_id: str = None,
         resource_owner_id: int = None,
         switch_time_mode: str = None,
     ):
+        # This parameter is required.
         self.dbinstance_id = dbinstance_id
+        # This parameter is required.
         self.engine_version = engine_version
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_id = resource_owner_id
         self.switch_time_mode = switch_time_mode
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_selectdb20230522-3.0.1/alibabacloud_selectdb20230522.egg-info/PKG-INFO` & `alibabacloud_selectdb20230522-3.1.0/alibabacloud_selectdb20230522.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-selectdb20230522
-Version: 3.0.1
+Version: 3.1.0
 Summary: Alibaba Cloud selectdb (20230522) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_selectdb20230522-3.0.1/setup.py` & `alibabacloud_selectdb20230522-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_selectdb20230522.
 
-Created on 15/03/2024
+Created on 15/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_selectdb20230522"
 NAME = "alibabacloud_selectdb20230522" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud selectdb (20230522) SDK Library for Python"
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

