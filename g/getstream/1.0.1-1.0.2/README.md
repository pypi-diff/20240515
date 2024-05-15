# Comparing `tmp/getstream-1.0.1.tar.gz` & `tmp/getstream-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getstream-1.0.1.tar", max compression
+gzip compressed data, was "getstream-1.0.2.tar", max compression
```

## Comparing `getstream-1.0.1.tar` & `getstream-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    14204 2024-05-13 12:18:46.349243 getstream-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     3708 2024-05-13 12:18:46.349243 getstream-1.0.1/README.md
--rw-r--r--   0        0        0       50 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/__init__.py
--rw-r--r--   0        0        0     6264 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/base.py
--rw-r--r--   0        0        0        0 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/__init__.py
--rw-r--r--   0        0        0       24 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/channel.py
--rw-r--r--   0        0        0      267 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/client.py
--rw-r--r--   0        0        0    45004 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/chat/rest_client.py
--rw-r--r--   0        0        0        0 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/__init__.py
--rw-r--r--   0        0        0      275 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/client.py
--rw-r--r--   0        0        0    23158 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/common/rest_client.py
--rw-r--r--   0        0        0      925 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/config.py
--rw-r--r--   0        0        0       46 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/generic.py
--rw-r--r--   0        0        0      497 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/meta.py
--rw-r--r--   0        0        0   298794 2024-05-13 12:18:46.349243 getstream-1.0.1/getstream/models/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/rate_limit.py
--rw-r--r--   0        0        0     4489 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/stream.py
--rw-r--r--   0        0        0     1024 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/stream_response.py
--rw-r--r--   0        0        0     3942 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/utils.py
--rw-r--r--   0        0        0       18 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/version.py
--rw-r--r--   0        0        0        0 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/__init__.py
--rw-r--r--   0        0        0    10156 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/call.py
--rw-r--r--   0        0        0      817 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/client.py
--rw-r--r--   0        0        0    18149 2024-05-13 12:18:46.353243 getstream-1.0.1/getstream/video/rest_client.py
--rw-r--r--   0        0        0      696 2024-05-13 12:18:46.353243 getstream-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 getstream-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    14204 2024-05-15 09:38:12.091005 getstream-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3708 2024-05-15 09:38:12.091005 getstream-1.0.2/README.md
+-rw-r--r--   0        0        0       50 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/__init__.py
+-rw-r--r--   0        0        0     6264 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/base.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/chat/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/chat/channel.py
+-rw-r--r--   0        0        0      267 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/chat/client.py
+-rw-r--r--   0        0        0    45004 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/chat/rest_client.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/common/__init__.py
+-rw-r--r--   0        0        0      275 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/common/client.py
+-rw-r--r--   0        0        0    23158 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/common/rest_client.py
+-rw-r--r--   0        0        0      925 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/config.py
+-rw-r--r--   0        0        0       46 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/generic.py
+-rw-r--r--   0        0        0      497 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/meta.py
+-rw-r--r--   0        0        0   299445 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/models/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/rate_limit.py
+-rw-r--r--   0        0        0     4489 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/stream.py
+-rw-r--r--   0        0        0     1024 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/stream_response.py
+-rw-r--r--   0        0        0     3942 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/utils.py
+-rw-r--r--   0        0        0       18 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/version.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:38:12.091005 getstream-1.0.2/getstream/video/__init__.py
+-rw-r--r--   0        0        0    10661 2024-05-15 09:38:12.095005 getstream-1.0.2/getstream/video/call.py
+-rw-r--r--   0        0        0      817 2024-05-15 09:38:12.095005 getstream-1.0.2/getstream/video/client.py
+-rw-r--r--   0        0        0    18823 2024-05-15 09:38:12.095005 getstream-1.0.2/getstream/video/rest_client.py
+-rw-r--r--   0        0        0      696 2024-05-15 09:38:12.095005 getstream-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 getstream-1.0.2/PKG-INFO
```

### Comparing `getstream-1.0.1/LICENSE.md` & `getstream-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/README.md` & `getstream-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/base.py` & `getstream-1.0.2/getstream/base.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/chat/rest_client.py` & `getstream-1.0.2/getstream/chat/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/common/rest_client.py` & `getstream-1.0.2/getstream/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/config.py` & `getstream-1.0.2/getstream/config.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/models/__init__.py` & `getstream-1.0.2/getstream/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2265,14 +2265,19 @@
 
 @dataclass
 class DeleteRecordingResponse(DataClassJsonMixin):
     duration: str = dc_field(metadata=dc_config(field_name="duration"))
 
 
 @dataclass
+class DeleteTranscriptionResponse(DataClassJsonMixin):
+    duration: str = dc_field(metadata=dc_config(field_name="duration"))
+
+
+@dataclass
 class DeleteUsersRequest(DataClassJsonMixin):
     user_ids: List[str] = dc_field(metadata=dc_config(field_name="user_ids"))
     calls: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="calls")
     )
     conversations: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="conversations")
@@ -6057,24 +6062,37 @@
     )
     channel_search_cids: Optional[List[str]] = dc_field(
         default=None, metadata=dc_config(field_name="channel_search_cids")
     )
 
 
 @dataclass
-class SendEventRequest(DataClassJsonMixin):
-    event: "EventRequest" = dc_field(metadata=dc_config(field_name="event"))
+class SendCallEventRequest(DataClassJsonMixin):
+    user_id: Optional[str] = dc_field(
+        default=None, metadata=dc_config(field_name="user_id")
+    )
+    custom: Optional[Dict[str, object]] = dc_field(
+        default=None, metadata=dc_config(field_name="custom")
+    )
+    user: "Optional[UserRequest]" = dc_field(
+        default=None, metadata=dc_config(field_name="user")
+    )
 
 
 @dataclass
-class SendEventResponse(DataClassJsonMixin):
+class SendCallEventResponse(DataClassJsonMixin):
     duration: str = dc_field(metadata=dc_config(field_name="duration"))
 
 
 @dataclass
+class SendEventRequest(DataClassJsonMixin):
+    event: "EventRequest" = dc_field(metadata=dc_config(field_name="event"))
+
+
+@dataclass
 class SendMessageRequest(DataClassJsonMixin):
     message: "MessageRequest" = dc_field(metadata=dc_config(field_name="message"))
     force_moderation: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="force_moderation")
     )
     keep_channel_hidden: Optional[bool] = dc_field(
         default=None, metadata=dc_config(field_name="keep_channel_hidden")
@@ -7880,14 +7898,17 @@
 
 @dataclass
 class UserStats(DataClassJsonMixin):
     session_stats: "List[UserSessionStats]" = dc_field(
         metadata=dc_config(field_name="session_stats")
     )
     info: "UserInfoResponse" = dc_field(metadata=dc_config(field_name="info"))
+    rating: Optional[int] = dc_field(
+        default=None, metadata=dc_config(field_name="rating")
+    )
 
 
 @dataclass
 class VideoQuality(DataClassJsonMixin):
     usage_type: Optional[str] = dc_field(
         default=None, metadata=dc_config(field_name="usage_type")
     )
```

### Comparing `getstream-1.0.1/getstream/rate_limit.py` & `getstream-1.0.2/getstream/rate_limit.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/stream.py` & `getstream-1.0.2/getstream/stream.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/stream_response.py` & `getstream-1.0.2/getstream/stream_response.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/utils.py` & `getstream-1.0.2/getstream/utils.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/video/call.py` & `getstream-1.0.2/getstream/video/call.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,17 +68,22 @@
     def block_user(self, user_id: str) -> StreamResponse[BlockUserResponse]:
         response = self.client.block_user(
             type=self.call_type, id=self.id, user_id=user_id
         )
         self._sync_from_response(response.data)
         return response
 
-    def send_call_event(self, event: EventRequest) -> StreamResponse[SendEventResponse]:
+    def send_call_event(
+        self,
+        user_id: Optional[str] = None,
+        custom: Optional[Dict[str, object]] = None,
+        user: Optional[UserRequest] = None,
+    ) -> StreamResponse[SendCallEventResponse]:
         response = self.client.send_call_event(
-            type=self.call_type, id=self.id, event=event
+            type=self.call_type, id=self.id, user_id=user_id, custom=custom, user=user
         )
         self._sync_from_response(response.data)
         return response
 
     def collect_user_feedback(
         self,
         session: str,
@@ -276,8 +281,17 @@
     ) -> StreamResponse[DeleteRecordingResponse]:
         response = self.client.delete_recording(
             type=self.call_type, id=self.id, session=session, filename=filename
         )
         self._sync_from_response(response.data)
         return response
 
+    def delete_transcription(
+        self, session: str, filename: str
+    ) -> StreamResponse[DeleteTranscriptionResponse]:
+        response = self.client.delete_transcription(
+            type=self.call_type, id=self.id, session=session, filename=filename
+        )
+        self._sync_from_response(response.data)
+        return response
+
     create = get_or_create
```

### Comparing `getstream-1.0.1/getstream/video/client.py` & `getstream-1.0.2/getstream/video/client.py`

 * *Files identical despite different names*

### Comparing `getstream-1.0.1/getstream/video/rest_client.py` & `getstream-1.0.2/getstream/video/rest_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,25 +145,30 @@
             "/api/v2/video/call/{type}/{id}/block",
             BlockUserResponse,
             path_params=path_params,
             json=json,
         )
 
     def send_call_event(
-        self, type: str, id: str, event: EventRequest
-    ) -> StreamResponse[SendEventResponse]:
+        self,
+        type: str,
+        id: str,
+        user_id: Optional[str] = None,
+        custom: Optional[Dict[str, object]] = None,
+        user: Optional[UserRequest] = None,
+    ) -> StreamResponse[SendCallEventResponse]:
         path_params = {
             "type": type,
             "id": id,
         }
-        json = build_body_dict(event=event)
+        json = build_body_dict(user_id=user_id, custom=custom, user=user)
 
         return self.post(
             "/api/v2/video/call/{type}/{id}/event",
-            SendEventResponse,
+            SendCallEventResponse,
             path_params=path_params,
             json=json,
         )
 
     def collect_user_feedback(
         self,
         type: str,
@@ -520,19 +525,35 @@
             "type": type,
             "id": id,
             "session": session,
             "filename": filename,
         }
 
         return self.delete(
-            "/api/v2/video/call/{type}/{id}/{session}/{filename}",
+            "/api/v2/video/call/{type}/{id}/{session}/recordings/{filename}",
             DeleteRecordingResponse,
             path_params=path_params,
         )
 
+    def delete_transcription(
+        self, type: str, id: str, session: str, filename: str
+    ) -> StreamResponse[DeleteTranscriptionResponse]:
+        path_params = {
+            "type": type,
+            "id": id,
+            "session": session,
+            "filename": filename,
+        }
+
+        return self.delete(
+            "/api/v2/video/call/{type}/{id}/{session}/transcriptions/{filename}",
+            DeleteTranscriptionResponse,
+            path_params=path_params,
+        )
+
     def query_calls(
         self,
         limit: Optional[int] = None,
         next: Optional[str] = None,
         prev: Optional[str] = None,
         sort: Optional[List[Optional[SortParam]]] = None,
         filter_conditions: Optional[Dict[str, object]] = None,
```

### Comparing `getstream-1.0.1/pyproject.toml` & `getstream-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getstream"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = [
     "sachaarbonel <sacha.arbonel@hotmail.fr>",
     "tbarbugli <tbarbugli@gmail.com>"
 ]
 readme = "README.md"
```

### Comparing `getstream-1.0.1/PKG-INFO` & `getstream-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getstream
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: sachaarbonel
 Author-email: sacha.arbonel@hotmail.fr
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

