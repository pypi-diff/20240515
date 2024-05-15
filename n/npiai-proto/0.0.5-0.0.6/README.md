# Comparing `tmp/npiai_proto-0.0.5.tar.gz` & `tmp/npiai_proto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai_proto-0.0.5.tar", max compression
+gzip compressed data, was "npiai_proto-0.0.6.tar", max compression
```

## Comparing `npiai_proto-0.0.5.tar` & `npiai_proto-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2024-05-02 23:10:36.741357 npiai_proto-0.0.5/README.md
--rw-r--r--   0        0        0     5088 2024-05-10 17:29:39.176654 npiai_proto-0.0.5/npiai_proto/api_pb2.py
--rw-r--r--   0        0        0     6035 2024-05-10 17:29:39.176882 npiai_proto-0.0.5/npiai_proto/api_pb2.pyi
--rw-r--r--   0        0        0     3829 2024-05-10 03:28:07.526306 npiai_proto-0.0.5/npiai_proto/api_pb2_grpc.py
--rw-r--r--   0        0        0      539 2024-05-10 17:30:27.056295 npiai_proto-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 npiai_proto-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-02 23:10:36.741357 npiai_proto-0.0.6/README.md
+-rw-r--r--   0        0        0     6655 2024-05-13 05:57:20.370333 npiai_proto-0.0.6/npiai_proto/api_pb2.py
+-rw-r--r--   0        0        0     7229 2024-05-13 05:57:20.370638 npiai_proto-0.0.6/npiai_proto/api_pb2.pyi
+-rw-r--r--   0        0        0     8526 2024-05-13 05:57:20.370996 npiai_proto-0.0.6/npiai_proto/api_pb2_grpc.py
+-rw-r--r--   0        0        0      531 2024-05-15 20:51:45.460858 npiai_proto-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 npiai_proto-0.0.6/PKG-INFO
```

### Comparing `npiai_proto-0.0.5/npiai_proto/api_pb2.py` & `npiai_proto-0.0.6/npiai_proto/api_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,42 +11,54 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x0cnpi.core.api\x1a\x1bgoogle/protobuf/empty.proto\"\x84\x02\n\x07Request\x12\'\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x19.npi.core.api.RequestCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x31\n\x0c\x63hat_request\x18\n \x01(\x0b\x32\x19.npi.core.api.ChatRequestH\x00\x12\x42\n\x15\x61\x63tion_result_request\x18\x0c \x01(\x0b\x32!.npi.core.api.ActionResultRequestH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\t\n\x07request\"7\n\x10\x41ppSchemaRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\"8\n\x11\x41ppSchemaResponse\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"G\n\x0b\x43hatRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\x12\x13\n\x0binstruction\x18\x02 \x01(\t\"?\n\x13\x41\x63tionResultRequest\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x15\n\raction_result\x18\x02 \x01(\t\"\x86\x02\n\x08Response\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1a.npi.core.api.ResponseCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x33\n\rchat_response\x18\n \x01(\x0b\x32\x1a.npi.core.api.ChatResponseH\x00\x12?\n\x0f\x61\x63tion_response\x18\x0b \x01(\x0b\x32$.npi.core.api.ActionRequiredResponseH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\n\n\x08response\"\x1f\n\x0c\x43hatResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\"u\n\x16\x41\x63tionRequiredResponse\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.npi.core.api.ActionType\x12\x11\n\taction_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x03(\t*J\n\x0bRequestCode\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x08\n\x04\x43HAT\x10\x01\x12\t\n\x05\x46\x45TCH\x10\x02\x12\x11\n\rACTION_RESULT\x10\x03*\x8f\x01\n\x07\x41ppType\x12\x0f\n\x0b\x41PP_UNKNOWN\x10\x00\x12\x10\n\x0cGOOGLE_GMAIL\x10\x01\x12\x13\n\x0fGOOGLE_CALENDAR\x10\x02\x12\n\n\x06GITHUB\x10\x03\x12\t\n\x05SLACK\x10\x04\x12\x0b\n\x07\x44ISCORD\x10\x05\x12\x0b\n\x07TWITTER\x10\x06\x12\x0f\n\x0bWEB_BROWSER\x10\x07\x12\n\n\x06TWILIO\x10\x08*m\n\x0cResponseCode\x12\x14\n\x10RESPONSE_UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\x0b\n\x07MESSAGE\x10\x03\x12\x13\n\x0f\x41\x43TION_REQUIRED\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05*q\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x0f\n\x0bINFORMATION\x10\x01\x12\x14\n\x10SINGLE_SELECTION\x10\x02\x12\x16\n\x12MULTIPLE_SELECTION\x10\x03\x12\x10\n\x0c\x43ONFIRMATION\x10\x04\x32\x93\x01\n\tAppServer\x12\x35\n\x04\x43hat\x12\x15.npi.core.api.Request\x1a\x16.npi.core.api.Response\x12O\n\x0cGetAppSchema\x12\x1e.npi.core.api.AppSchemaRequest\x1a\x1f.npi.core.api.AppSchemaResponseB\x1eZ\x1cgithub.com/npi-ai/npi/serverb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x0cnpi.core.api\x1a\x1bgoogle/protobuf/empty.proto\"\x84\x02\n\x07Request\x12\'\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x19.npi.core.api.RequestCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x31\n\x0c\x63hat_request\x18\n \x01(\x0b\x32\x19.npi.core.api.ChatRequestH\x00\x12\x42\n\x15\x61\x63tion_result_request\x18\x0c \x01(\x0b\x32!.npi.core.api.ActionResultRequestH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\t\n\x07request\"7\n\x10\x41ppSchemaRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\"8\n\x11\x41ppSchemaResponse\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"G\n\x0b\x43hatRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\x12\x13\n\x0binstruction\x18\x02 \x01(\t\"?\n\x13\x41\x63tionResultRequest\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x15\n\raction_result\x18\x02 \x01(\t\"\xb1\x01\n\x10\x41uthorizeRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\x12\x44\n\x0b\x63redentials\x18\x02 \x03(\x0b\x32/.npi.core.api.AuthorizeRequest.CredentialsEntry\x1a\x32\n\x10\x43redentialsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x11\x41uthorizeResponse\x12;\n\x06result\x18\x01 \x03(\x0b\x32+.npi.core.api.AuthorizeResponse.ResultEntry\x1a-\n\x0bResultEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x86\x02\n\x08Response\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1a.npi.core.api.ResponseCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x33\n\rchat_response\x18\n \x01(\x0b\x32\x1a.npi.core.api.ChatResponseH\x00\x12?\n\x0f\x61\x63tion_response\x18\x0b \x01(\x0b\x32$.npi.core.api.ActionRequiredResponseH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\n\n\x08response\"\x1f\n\x0c\x43hatResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\"u\n\x16\x41\x63tionRequiredResponse\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.npi.core.api.ActionType\x12\x11\n\taction_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x03(\t*J\n\x0bRequestCode\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x08\n\x04\x43HAT\x10\x01\x12\t\n\x05\x46\x45TCH\x10\x02\x12\x11\n\rACTION_RESULT\x10\x03*\x8f\x01\n\x07\x41ppType\x12\x0f\n\x0b\x41PP_UNKNOWN\x10\x00\x12\x10\n\x0cGOOGLE_GMAIL\x10\x01\x12\x13\n\x0fGOOGLE_CALENDAR\x10\x02\x12\n\n\x06GITHUB\x10\x03\x12\t\n\x05SLACK\x10\x04\x12\x0b\n\x07\x44ISCORD\x10\x05\x12\x0b\n\x07TWITTER\x10\x06\x12\x0f\n\x0bWEB_BROWSER\x10\x07\x12\n\n\x06TWILIO\x10\x08*m\n\x0cResponseCode\x12\x14\n\x10RESPONSE_UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\x0b\n\x07MESSAGE\x10\x03\x12\x13\n\x0f\x41\x43TION_REQUIRED\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05*q\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x0f\n\x0bINFORMATION\x10\x01\x12\x14\n\x10SINGLE_SELECTION\x10\x02\x12\x16\n\x12MULTIPLE_SELECTION\x10\x03\x12\x10\n\x0c\x43ONFIRMATION\x10\x04\x32\xe7\x02\n\tAppServer\x12\x35\n\x04\x43hat\x12\x15.npi.core.api.Request\x1a\x16.npi.core.api.Response\x12O\n\x0cGetAppSchema\x12\x1e.npi.core.api.AppSchemaRequest\x1a\x1f.npi.core.api.AppSchemaResponse\x12L\n\tAuthorize\x12\x1e.npi.core.api.AuthorizeRequest\x1a\x1f.npi.core.api.AuthorizeResponse\x12L\n\x12GoogleAuthCallback\x12\x1e.npi.core.api.AuthorizeRequest\x1a\x16.google.protobuf.Empty\x12\x36\n\x04Ping\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.EmptyB\x1eZ\x1cgithub.com/npi-ai/npi/serverb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z\034github.com/npi-ai/npi/server'
-  _globals['_REQUESTCODE']._serialized_start=989
-  _globals['_REQUESTCODE']._serialized_end=1063
-  _globals['_APPTYPE']._serialized_start=1066
-  _globals['_APPTYPE']._serialized_end=1209
-  _globals['_RESPONSECODE']._serialized_start=1211
-  _globals['_RESPONSECODE']._serialized_end=1320
-  _globals['_ACTIONTYPE']._serialized_start=1322
-  _globals['_ACTIONTYPE']._serialized_end=1435
+  _globals['_AUTHORIZEREQUEST_CREDENTIALSENTRY']._options = None
+  _globals['_AUTHORIZEREQUEST_CREDENTIALSENTRY']._serialized_options = b'8\001'
+  _globals['_AUTHORIZERESPONSE_RESULTENTRY']._options = None
+  _globals['_AUTHORIZERESPONSE_RESULTENTRY']._serialized_options = b'8\001'
+  _globals['_REQUESTCODE']._serialized_start=1298
+  _globals['_REQUESTCODE']._serialized_end=1372
+  _globals['_APPTYPE']._serialized_start=1375
+  _globals['_APPTYPE']._serialized_end=1518
+  _globals['_RESPONSECODE']._serialized_start=1520
+  _globals['_RESPONSECODE']._serialized_end=1629
+  _globals['_ACTIONTYPE']._serialized_start=1631
+  _globals['_ACTIONTYPE']._serialized_end=1744
   _globals['_REQUEST']._serialized_start=57
   _globals['_REQUEST']._serialized_end=317
   _globals['_APPSCHEMAREQUEST']._serialized_start=319
   _globals['_APPSCHEMAREQUEST']._serialized_end=374
   _globals['_APPSCHEMARESPONSE']._serialized_start=376
   _globals['_APPSCHEMARESPONSE']._serialized_end=432
   _globals['_CHATREQUEST']._serialized_start=434
   _globals['_CHATREQUEST']._serialized_end=505
   _globals['_ACTIONRESULTREQUEST']._serialized_start=507
   _globals['_ACTIONRESULTREQUEST']._serialized_end=570
-  _globals['_RESPONSE']._serialized_start=573
-  _globals['_RESPONSE']._serialized_end=835
-  _globals['_CHATRESPONSE']._serialized_start=837
-  _globals['_CHATRESPONSE']._serialized_end=868
-  _globals['_ACTIONREQUIREDRESPONSE']._serialized_start=870
-  _globals['_ACTIONREQUIREDRESPONSE']._serialized_end=987
-  _globals['_APPSERVER']._serialized_start=1438
-  _globals['_APPSERVER']._serialized_end=1585
+  _globals['_AUTHORIZEREQUEST']._serialized_start=573
+  _globals['_AUTHORIZEREQUEST']._serialized_end=750
+  _globals['_AUTHORIZEREQUEST_CREDENTIALSENTRY']._serialized_start=700
+  _globals['_AUTHORIZEREQUEST_CREDENTIALSENTRY']._serialized_end=750
+  _globals['_AUTHORIZERESPONSE']._serialized_start=752
+  _globals['_AUTHORIZERESPONSE']._serialized_end=879
+  _globals['_AUTHORIZERESPONSE_RESULTENTRY']._serialized_start=834
+  _globals['_AUTHORIZERESPONSE_RESULTENTRY']._serialized_end=879
+  _globals['_RESPONSE']._serialized_start=882
+  _globals['_RESPONSE']._serialized_end=1144
+  _globals['_CHATRESPONSE']._serialized_start=1146
+  _globals['_CHATRESPONSE']._serialized_end=1177
+  _globals['_ACTIONREQUIREDRESPONSE']._serialized_start=1179
+  _globals['_ACTIONREQUIREDRESPONSE']._serialized_end=1296
+  _globals['_APPSERVER']._serialized_start=1747
+  _globals['_APPSERVER']._serialized_end=2106
 # @@protoc_insertion_point(module_scope)
```

### Comparing `npiai_proto-0.0.5/npiai_proto/api_pb2.pyi` & `npiai_proto-0.0.6/npiai_proto/api_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -109,14 +109,42 @@
     __slots__ = ("action_id", "action_result")
     ACTION_ID_FIELD_NUMBER: _ClassVar[int]
     ACTION_RESULT_FIELD_NUMBER: _ClassVar[int]
     action_id: str
     action_result: str
     def __init__(self, action_id: _Optional[str] = ..., action_result: _Optional[str] = ...) -> None: ...
 
+class AuthorizeRequest(_message.Message):
+    __slots__ = ("type", "credentials")
+    class CredentialsEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
+    type: AppType
+    credentials: _containers.ScalarMap[str, str]
+    def __init__(self, type: _Optional[_Union[AppType, str]] = ..., credentials: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
+class AuthorizeResponse(_message.Message):
+    __slots__ = ("result",)
+    class ResultEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    result: _containers.ScalarMap[str, str]
+    def __init__(self, result: _Optional[_Mapping[str, str]] = ...) -> None: ...
+
 class Response(_message.Message):
     __slots__ = ("code", "request_id", "thread_id", "chat_response", "action_response", "empty")
     CODE_FIELD_NUMBER: _ClassVar[int]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
     THREAD_ID_FIELD_NUMBER: _ClassVar[int]
     CHAT_RESPONSE_FIELD_NUMBER: _ClassVar[int]
     ACTION_RESPONSE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `npiai_proto-0.0.5/pyproject.toml` & `npiai_proto-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "npiai-proto"
-version = "v0.0.5"
+version = "v0.0.6"
 description = "The NPI.AI Proto"
 license = "Apache-2.0"
 authors = ["Wells Wang <wells@npi.ai>"]
 readme = "README.md"
-homepage = "https://github.com/npi-ai/npi/proto/python"
-repository = "https://github.com/npi-ai/npi/proto/python"
+homepage = "https://github.com/npi-ai/proto/python"
+repository = "https://github.com/npi-ai/proto/python"
 #in-project = true
 
 [tool.poetry.dependencies]
 python = "^3.10"
 grpcio = "^1.62.1"
 grpcio-tools = "^1.62.2"
```

### Comparing `npiai_proto-0.0.5/PKG-INFO` & `npiai_proto-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: npiai-proto
-Version: 0.0.5
+Version: 0.0.6
 Summary: The NPI.AI Proto
-Home-page: https://github.com/npi-ai/npi/proto/python
+Home-page: https://github.com/npi-ai/proto/python
 License: Apache-2.0
 Author: Wells Wang
 Author-email: wells@npi.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.62.1,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.62.2,<2.0.0)
-Project-URL: Repository, https://github.com/npi-ai/npi/proto/python
+Project-URL: Repository, https://github.com/npi-ai/proto/python
 Description-Content-Type: text/markdown
 
 ## The NPI AI Python Protocol
```

