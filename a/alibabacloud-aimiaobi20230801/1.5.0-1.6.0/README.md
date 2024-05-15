# Comparing `tmp/alibabacloud_aimiaobi20230801-1.5.0.tar.gz` & `tmp/alibabacloud_aimiaobi20230801-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.5.0.tar", last modified: Mon May 13 17:15:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.6.0.tar", last modified: Wed May 15 02:03:47 2024, max compression
```

## Comparing `alibabacloud_aimiaobi20230801-1.5.0.tar` & `alibabacloud_aimiaobi20230801-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     1187 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224740 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/client.py
--rw-r--r--   0 root         (0) root         (0)   387261 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-05-13 17:15:09.000000 alibabacloud_aimiaobi20230801-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1549 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229176 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/client.py
+-rw-r--r--   0 root         (0) root         (0)   394960 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/setup.py
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/ChangeLog.md` & `alibabacloud_aimiaobi20230801-1.6.0/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+2024-05-13 Version: 1.5.0
+- Support API DeleteCustomText.
+- Support API GetCustomText.
+- Support API ListCustomText.
+- Support API SaveCustomText.
+- Support API UpdateCustomText.
+
+
+2024-05-13 Version: 1.5.0
+- Support API DeleteCustomText.
+- Support API GetCustomText.
+- Support API ListCustomText.
+- Support API SaveCustomText.
+- Support API UpdateCustomText.
+
+
 2024-03-12 Version: 1.4.0
 - Support API ClearIntervenes.
 - Support API DeleteInterveneRule.
 - Support API ExportIntervenes.
 - Support API GetInterveneGlobalReply.
 - Support API GetInterveneImportTaskInfo.
 - Support API GetInterveneRuleDetail.
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/LICENSE` & `alibabacloud_aimiaobi20230801-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aimiaobi20230801
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/README-CN.md` & `alibabacloud_aimiaobi20230801-1.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/README.md` & `alibabacloud_aimiaobi20230801-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/client.py` & `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -893,14 +893,126 @@
         
         @param request: DeleteMaterialByIdRequest
         @return: DeleteMaterialByIdResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_material_by_id_with_options_async(request, runtime)
 
+    def document_extraction_with_options(
+        self,
+        tmp_req: ai_miao_bi_20230801_models.DocumentExtractionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ai_miao_bi_20230801_models.DocumentExtractionResponse:
+        """
+        @summary 从链接中提取文档内容
+        
+        @param tmp_req: DocumentExtractionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DocumentExtractionResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = ai_miao_bi_20230801_models.DocumentExtractionShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.urls):
+            request.urls_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.urls, 'Urls', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.agent_key):
+            query['AgentKey'] = request.agent_key
+        body = {}
+        if not UtilClient.is_unset(request.urls_shrink):
+            body['Urls'] = request.urls_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DocumentExtraction',
+            version='2023-08-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ai_miao_bi_20230801_models.DocumentExtractionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def document_extraction_with_options_async(
+        self,
+        tmp_req: ai_miao_bi_20230801_models.DocumentExtractionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ai_miao_bi_20230801_models.DocumentExtractionResponse:
+        """
+        @summary 从链接中提取文档内容
+        
+        @param tmp_req: DocumentExtractionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DocumentExtractionResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = ai_miao_bi_20230801_models.DocumentExtractionShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.urls):
+            request.urls_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.urls, 'Urls', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.agent_key):
+            query['AgentKey'] = request.agent_key
+        body = {}
+        if not UtilClient.is_unset(request.urls_shrink):
+            body['Urls'] = request.urls_shrink
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DocumentExtraction',
+            version='2023-08-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ai_miao_bi_20230801_models.DocumentExtractionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def document_extraction(
+        self,
+        request: ai_miao_bi_20230801_models.DocumentExtractionRequest,
+    ) -> ai_miao_bi_20230801_models.DocumentExtractionResponse:
+        """
+        @summary 从链接中提取文档内容
+        
+        @param request: DocumentExtractionRequest
+        @return: DocumentExtractionResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.document_extraction_with_options(request, runtime)
+
+    async def document_extraction_async(
+        self,
+        request: ai_miao_bi_20230801_models.DocumentExtractionRequest,
+    ) -> ai_miao_bi_20230801_models.DocumentExtractionResponse:
+        """
+        @summary 从链接中提取文档内容
+        
+        @param request: DocumentExtractionRequest
+        @return: DocumentExtractionResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.document_extraction_with_options_async(request, runtime)
+
     def export_generated_content_with_options(
         self,
         request: ai_miao_bi_20230801_models.ExportGeneratedContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ai_miao_bi_20230801_models.ExportGeneratedContentResponse:
         """
         @summary 文档管理-导出。
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801/models.py` & `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1282,14 +1282,271 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteMaterialByIdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DocumentExtractionRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        urls: List[str] = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        # This parameter is required.
+        self.urls = urls
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
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.urls is not None:
+            result['Urls'] = self.urls
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('Urls') is not None:
+            self.urls = m.get('Urls')
+        return self
+
+
+class DocumentExtractionShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        agent_key: str = None,
+        urls_shrink: str = None,
+    ):
+        # This parameter is required.
+        self.agent_key = agent_key
+        # This parameter is required.
+        self.urls_shrink = urls_shrink
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
+        if self.agent_key is not None:
+            result['AgentKey'] = self.agent_key
+        if self.urls_shrink is not None:
+            result['Urls'] = self.urls_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AgentKey') is not None:
+            self.agent_key = m.get('AgentKey')
+        if m.get('Urls') is not None:
+            self.urls_shrink = m.get('Urls')
+        return self
+
+
+class DocumentExtractionResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        author: str = None,
+        content: str = None,
+        doc_id: str = None,
+        doc_uuid: str = None,
+        pub_time: str = None,
+        source: str = None,
+        summary: str = None,
+        tag: str = None,
+        title: str = None,
+        url: str = None,
+    ):
+        self.author = author
+        self.content = content
+        self.doc_id = doc_id
+        self.doc_uuid = doc_uuid
+        self.pub_time = pub_time
+        self.source = source
+        self.summary = summary
+        self.tag = tag
+        self.title = title
+        self.url = url
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
+        if self.author is not None:
+            result['Author'] = self.author
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.doc_id is not None:
+            result['DocId'] = self.doc_id
+        if self.doc_uuid is not None:
+            result['DocUuid'] = self.doc_uuid
+        if self.pub_time is not None:
+            result['PubTime'] = self.pub_time
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.summary is not None:
+            result['Summary'] = self.summary
+        if self.tag is not None:
+            result['Tag'] = self.tag
+        if self.title is not None:
+            result['Title'] = self.title
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Author') is not None:
+            self.author = m.get('Author')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('DocId') is not None:
+            self.doc_id = m.get('DocId')
+        if m.get('DocUuid') is not None:
+            self.doc_uuid = m.get('DocUuid')
+        if m.get('PubTime') is not None:
+            self.pub_time = m.get('PubTime')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('Summary') is not None:
+            self.summary = m.get('Summary')
+        if m.get('Tag') is not None:
+            self.tag = m.get('Tag')
+        if m.get('Title') is not None:
+            self.title = m.get('Title')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class DocumentExtractionResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: List[DocumentExtractionResponseBodyData] = None,
+        http_status_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.data = data
+        self.http_status_code = http_status_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
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
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DocumentExtractionResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DocumentExtractionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DocumentExtractionResponseBody = None,
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
+            temp_model = DocumentExtractionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ExportGeneratedContentRequest(TeaModel):
     def __init__(
         self,
         agent_key: str = None,
         id: int = None,
     ):
         # This parameter is required.
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aimiaobi20230801
-Version: 1.5.0
+Version: 1.6.0
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.5.0/setup.py` & `alibabacloud_aimiaobi20230801-1.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aimiaobi20230801.
 
-Created on 13/05/2024
+Created on 14/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aimiaobi20230801"
 NAME = "alibabacloud_aimiaobi20230801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.12, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

