# Comparing `tmp/npiai-0.0.5.tar.gz` & `tmp/npiai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai-0.0.5.tar", max compression
+gzip compressed data, was "npiai-0.0.6.tar", max compression
```

## Comparing `npiai-0.0.5.tar` & `npiai-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0    11356 2024-05-02 23:10:36.742561 npiai-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2024-05-02 21:49:09.883864 npiai-0.0.5/README.md
--rw-r--r--   0        0        0      151 2024-05-02 21:49:09.884168 npiai-0.0.5/npiai/__init__.py
--rw-r--r--   0        0        0      209 2024-05-02 21:49:09.884353 npiai-0.0.5/npiai/app/__init__.py
--rw-r--r--   0        0        0      278 2024-05-02 21:49:09.884486 npiai-0.0.5/npiai/app/discord.py
--rw-r--r--   0        0        0      275 2024-05-02 21:49:09.884617 npiai-0.0.5/npiai/app/github.py
--rw-r--r--   0        0        0      510 2024-05-02 21:49:09.884749 npiai-0.0.5/npiai/app/google.py
--rw-r--r--   0        0        0     1073 2024-05-02 21:49:09.884889 npiai-0.0.5/npiai/app/human_feedback.py
--rw-r--r--   0        0        0       92 2024-05-02 21:49:09.885063 npiai-0.0.5/npiai/browser_app/__init__.py
--rw-r--r--   0        0        0      282 2024-05-02 21:49:09.885203 npiai-0.0.5/npiai/browser_app/browser.py
--rw-r--r--   0        0        0      278 2024-05-02 21:49:09.885330 npiai-0.0.5/npiai/browser_app/twitter.py
--rw-r--r--   0        0        0       57 2024-05-02 21:49:09.885499 npiai-0.0.5/npiai/core/__init__.py
--rw-r--r--   0        0        0     7978 2024-05-10 17:29:39.177868 npiai-0.0.5/npiai/core/base.py
--rw-r--r--   0        0        0     2137 2024-05-10 17:29:39.178174 npiai-0.0.5/npiai/core/hitl.py
--rw-r--r--   0        0        0     1771 2024-05-10 17:29:39.178322 npiai-0.0.5/npiai/tools/hitl/console.py
--rw-r--r--   0        0        0     2185 2024-05-10 17:29:39.178460 npiai-0.0.5/npiai/tools/hitl/twilio.py
--rw-r--r--   0        0        0       49 2024-05-02 21:49:09.885976 npiai-0.0.5/npiai/utils/__init__.py
--rw-r--r--   0        0        0      152 2024-05-02 21:49:09.886103 npiai-0.0.5/npiai/utils/logger.py
--rw-r--r--   0        0        0      380 2024-05-10 17:32:12.965041 npiai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 npiai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-02 23:10:36.742561 npiai-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-02 21:49:09.883864 npiai-0.0.6/README.md
+-rw-r--r--   0        0        0      151 2024-05-02 21:49:09.884168 npiai-0.0.6/npiai/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-02 21:49:09.884353 npiai-0.0.6/npiai/app/__init__.py
+-rw-r--r--   0        0        0      278 2024-05-02 21:49:09.884486 npiai-0.0.6/npiai/app/discord.py
+-rw-r--r--   0        0        0      490 2024-05-15 20:45:46.705901 npiai-0.0.6/npiai/app/github.py
+-rw-r--r--   0        0        0      622 2024-05-13 05:57:20.371400 npiai-0.0.6/npiai/app/google.py
+-rw-r--r--   0        0        0     1073 2024-05-02 21:49:09.884889 npiai-0.0.6/npiai/app/human_feedback.py
+-rw-r--r--   0        0        0       92 2024-05-02 21:49:09.885063 npiai-0.0.6/npiai/browser_app/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-02 21:49:09.885203 npiai-0.0.6/npiai/browser_app/browser.py
+-rw-r--r--   0        0        0      278 2024-05-02 21:49:09.885330 npiai-0.0.6/npiai/browser_app/twitter.py
+-rw-r--r--   0        0        0       57 2024-05-02 21:49:09.885499 npiai-0.0.6/npiai/core/__init__.py
+-rw-r--r--   0        0        0     9191 2024-05-15 20:45:46.706198 npiai-0.0.6/npiai/core/base.py
+-rw-r--r--   0        0        0     2137 2024-05-10 17:29:39.178174 npiai-0.0.6/npiai/core/hitl.py
+-rw-r--r--   0        0        0     1092 2024-05-15 20:45:46.706434 npiai-0.0.6/npiai/core/toolset.py
+-rw-r--r--   0        0        0     1627 2024-05-15 20:45:46.706630 npiai-0.0.6/npiai/integration/oai.py
+-rw-r--r--   0        0        0      164 2024-05-15 20:45:46.706887 npiai-0.0.6/npiai/tools/hitl/__init__.py
+-rw-r--r--   0        0        0     1771 2024-05-10 17:29:39.178322 npiai-0.0.6/npiai/tools/hitl/console.py
+-rw-r--r--   0        0        0      824 2024-05-15 20:45:46.707137 npiai-0.0.6/npiai/tools/hitl/empty.py
+-rw-r--r--   0        0        0     2185 2024-05-10 17:29:39.178460 npiai-0.0.6/npiai/tools/hitl/twilio.py
+-rw-r--r--   0        0        0       49 2024-05-02 21:49:09.885976 npiai-0.0.6/npiai/utils/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-02 21:49:09.886103 npiai-0.0.6/npiai/utils/logger.py
+-rw-r--r--   0        0        0      380 2024-05-15 20:53:49.366635 npiai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 npiai-0.0.6/PKG-INFO
```

### Comparing `npiai-0.0.5/LICENSE` & `npiai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `npiai-0.0.5/npiai/app/human_feedback.py` & `npiai-0.0.6/npiai/app/human_feedback.py`

 * *Files identical despite different names*

### Comparing `npiai-0.0.5/npiai/core/base.py` & `npiai-0.0.6/npiai/core/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,134 @@
 import json
 import threading
 import traceback
-from typing import Union, List
+from typing import List
 import grpc
 import uuid
+from abc import ABC, abstractmethod
 
 from openai import OpenAI
 from openai.types.chat import (
     ChatCompletionSystemMessageParam,
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionToolParam,
     ChatCompletionUserMessageParam,
 )
 
 from npiai_proto import api_pb2_grpc, api_pb2
 from npiai.utils import logger
 from npiai.core import hitl
 
 
-class App:
+class App(ABC):
     __app_name: str
     __app_type: api_pb2.AppType
     __npi_endpoint: str
     stub: api_pb2_grpc.AppServerStub
     hitl_handler: hitl.HITLHandler = None
 
     def __init__(
-        self,
-        app_name: str,
-        app_type: api_pb2.AppType,
-        endpoint: str = "localhost:9140",
-        hitl_handler: hitl.HITLHandler = None,
+            self,
+            app_name: str,
+            app_type: api_pb2.AppType,
+            endpoint: str = "localhost:9140",
+            hitl_handler: hitl.HITLHandler = None,
+            npi_token: str = None,
+            insecure: bool = True,
     ):
         self.__app_name = app_name
         if endpoint is None:
             endpoint = "localhost:9140"
         self.__npi_endpoint = endpoint
         self.__app_type = app_type
-        channel = grpc.insecure_channel(self.__npi_endpoint)
+        if insecure:
+            channel = grpc.insecure_channel(self.__npi_endpoint)
+        else:
+            channel = grpc.secure_channel(target=self.__npi_endpoint, credentials=grpc.ssl_channel_credentials())
         self.stub = api_pb2_grpc.AppServerStub(channel)
         self.hitl_handler = hitl_handler
+        self.__npi_token = npi_token
 
     def tool_name(self):
         return self.__app_name
 
     def schema(self):
         try:
             resp = self.stub.GetAppSchema(
-                api_pb2.AppSchemaRequest(
+                request=api_pb2.AppSchemaRequest(
                     type=self.__app_type
-                )
+                ),
+                metadata=self.__get_metadata(),
             )
         except Exception as e:
             logger.error(e)
             return None
         return json.loads(resp.schema)
 
     def chat(self, msg: str) -> str:
         resp = self.stub.Chat(
-            api_pb2.Request(
+            request=api_pb2.Request(
                 code=api_pb2.RequestCode.CHAT,
                 chat_request=api_pb2.ChatRequest(
                     type=self.__app_type,
                     instruction=msg
-                )
-            )
+                ),
+            ),
+            metadata=self.__get_metadata(),
         )
         while True:
             match resp.code:
                 case api_pb2.ResponseCode.FINISHED:
                     return resp.chat_response.message
                 case api_pb2.ResponseCode.MESSAGE:
                     logger.info(f'[{self.__app_name}]: Received message: {resp.chat_response.message}')
                     resp = self.stub.Chat(
-                        api_pb2.Request(
+                        request=api_pb2.Request(
                             code=api_pb2.RequestCode.FETCH,
                             request_id=str(uuid.uuid4()),
                             thread_id=resp.thread_id,
                             chat_request=api_pb2.ChatRequest(
                                 type=self.__app_type,
                             )
-                        )
+                        ),
+                        metadata=self.__get_metadata(),
                     )
                 case api_pb2.ResponseCode.SUCCESS:
                     resp = self.stub.Chat(
-                        api_pb2.Request(
+                        request=api_pb2.Request(
                             code=api_pb2.RequestCode.FETCH,
                             request_id=str(uuid.uuid4()),
                             thread_id=resp.thread_id,
                             chat_request=api_pb2.ChatRequest(
                                 type=self.__app_type,
                             )
-                        )
+                        ),
+                        metadata=self.__get_metadata(),
                     )
                 case api_pb2.ResponseCode.ACTION_REQUIRED:
-                    resp = self.stub.Chat(self.__call_human(resp))
+                    resp = self.stub.Chat(request=self.__call_human(resp), metadata=self.__get_metadata())
                 case _:
+                    logger.error(f'[{self.__app_name}]: Error: failed to call function, unknown response code {resp.code}')
                     raise Exception("Error: failed to call function")
 
     def hitl(self, handler: hitl.HITLHandler):
         self.hitl_handler = handler
 
+    def authorize(self):
+        pass
+
+    def _authorize(self, credentials: dict[str, str]):
+        self.stub.Authorize(
+            request=api_pb2.AuthorizeRequest(
+                type=self.__app_type,
+                credentials=credentials,
+            ),
+        )
+        logger.info(f'[{self.__app_name}]: Authorized')
+
     def __call_human(self, resp: api_pb2.Response) -> api_pb2.Request:
         human_resp = self.hitl_handler.handle(
             hitl.convert_to_hitl_request(
                 req=resp.action_response,
                 app_name=self.__app_name
             )
         )
@@ -118,33 +142,37 @@
             thread_id=resp.thread_id,
             action_result_request=api_pb2.ActionResultRequest(
                 action_id=resp.action_response.action_id,
                 action_result=result,
             )
         )
 
+    def __get_metadata(self):
+        return (('x-host', 'test.playground.npi.ai'),
+                ('x-npi-token', self.__npi_token))
+
 
 class Agent:
     __agent_name: str
     __npi_endpoint: str
     __prompt: str
     __description: str
     __llm: OpenAI
     tool_choice: ChatCompletionToolChoiceOptionParam = "auto"
     fn_map: dict = {}
     hitl_handler: hitl.HITLHandler = None
 
     def __init__(
-        self,
-        agent_name: str,
-        description: str,
-        prompt: str,
-        endpoint: str = None,
-        llm: OpenAI = None,
-        hitl_handler: hitl.HITLHandler = None,
+            self,
+            agent_name: str,
+            description: str,
+            prompt: str,
+            endpoint: str = None,
+            llm: OpenAI = None,
+            hitl_handler: hitl.HITLHandler = None,
     ):
         self.__agent_name = agent_name
         self.__description = description
         self.__prompt = prompt
         self.__npi_endpoint = endpoint
         self.__llm = llm
         self.hitl_handler = hitl_handler
```

### Comparing `npiai-0.0.5/npiai/core/hitl.py` & `npiai-0.0.6/npiai/core/hitl.py`

 * *Files identical despite different names*

### Comparing `npiai-0.0.5/npiai/tools/hitl/console.py` & `npiai-0.0.6/npiai/tools/hitl/console.py`

 * *Files identical despite different names*

### Comparing `npiai-0.0.5/npiai/tools/hitl/twilio.py` & `npiai-0.0.6/npiai/tools/hitl/twilio.py`

 * *Files identical despite different names*

### Comparing `npiai-0.0.5/PKG-INFO` & `npiai-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: npiai
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: wenfeng
 Author-email: w@npi.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: npiai-proto (==v0.0.5)
+Requires-Dist: npiai-proto (==v0.0.6)
 Requires-Dist: openai (>=1.23.2,<2.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: twilio (>=9.0.5,<10.0.0)
 Description-Content-Type: text/markdown
```

