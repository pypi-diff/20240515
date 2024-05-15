# Comparing `tmp/pysgconnect-1.2-py3-none-any.whl.zip` & `tmp/pysgconnect-2.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7362 bytes, number of entries: 8
--rw-r--r--  2.0 unx      187 b- defN 24-May-07 11:54 pysgconnect/__init__.py
--rw-r--r--  2.0 unx     2001 b- defN 24-May-07 11:54 pysgconnect/sg_connect_auth.py
--rw-r--r--  2.0 unx      629 b- defN 24-May-07 11:54 pysgconnect/token.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-07 11:54 pysgconnect-1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1091 b- defN 24-May-07 11:54 pysgconnect-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 11:54 pysgconnect-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-07 11:54 pysgconnect-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      639 b- defN 24-May-07 11:54 pysgconnect-1.2.dist-info/RECORD
-8 files, 16008 bytes uncompressed, 6248 bytes compressed:  61.0%
+Zip file size: 7383 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      187 b- defN 24-May-15 09:25 pysgconnect/__init__.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-May-15 09:25 pysgconnect/sg_connect_auth.py
+-rw-r--r--  2.0 unx      629 b- defN 24-May-15 09:25 pysgconnect/token.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-15 09:26 pysgconnect-2.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1093 b- defN 24-May-15 09:26 pysgconnect-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 09:26 pysgconnect-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-15 09:26 pysgconnect-2.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      649 b- defN 24-May-15 09:26 pysgconnect-2.2.1.dist-info/RECORD
+8 files, 16037 bytes uncompressed, 6249 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pysgconnect/sg_connect_auth.py
 Comment: 
 
 Filename: pysgconnect/token.py
 Comment: 
 
-Filename: pysgconnect-1.2.dist-info/LICENSE
+Filename: pysgconnect-2.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pysgconnect-1.2.dist-info/METADATA
+Filename: pysgconnect-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pysgconnect-1.2.dist-info/WHEEL
+Filename: pysgconnect-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pysgconnect-1.2.dist-info/top_level.txt
+Filename: pysgconnect-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pysgconnect-1.2.dist-info/RECORD
+Filename: pysgconnect-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pysgconnect/sg_connect_auth.py

```diff
@@ -21,32 +21,32 @@
         self._endpoint: str = f"{get_url(env)}/sgconnect/oauth2/access_token"
         self._session: Session = Session()
         self._token: Token = Token()
 
         self._credentials = (client_id, client_secret)
         self._scopes: list[str] | None = scopes
 
-    def __call__(self, r):
+    def __call__(self, request):
         self._check_token()
-        r.headers["Authorization"] = f"Bearer {self._token.jwt}"
-        return r
+        request.headers["Authorization"] = f"Bearer {self._token.jwt}"
+        return request
 
     def _check_token(self) -> None:
         if self._token.is_not_empty() and not self._token.is_token_expired():
             self._logger.debug("Current token valid until: %s", self._token.expires_at)
             return
 
         if not self._scopes:
             raise ValueError("No scopes were provided")
 
         response: Response = self._session.post(
             self._endpoint,
             verify=True,
             auth=self._credentials,
-            data={"grant_type": "client_credentials", "scopes": " ".join(self._scopes)},
+            data={"grant_type": "client_credentials", "scope": " ".join(self._scopes)},
         )
 
         response.raise_for_status()
 
         body = response.json()
 
         token_value = body["access_token"]
```

## Comparing `pysgconnect-1.2.dist-info/LICENSE` & `pysgconnect-2.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysgconnect-1.2.dist-info/METADATA` & `pysgconnect-2.2.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysgconnect
-Version: 1.2
+Version: 2.2.1
 Summary: Utilities to interact with SGConnect
 Home-page: https://github.com/societe-generale/pysgconnect
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `pysgconnect-1.2.dist-info/RECORD` & `pysgconnect-2.2.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pysgconnect/__init__.py,sha256=Tlgpr9TWANqzrdjMEJyA40sZq9WzD3ckaOjmwZ9VPvA,187
-pysgconnect/sg_connect_auth.py,sha256=y3i8BpEZs42llHR81RHLzNSIYnL5W8BA0pN-WHE7Ze0,2001
+pysgconnect/sg_connect_auth.py,sha256=PIh-es3R5SiqIqiH9I9FRQ7fwtg26yaaDaihPrke9IA,2018
 pysgconnect/token.py,sha256=sQI-VN4A_VPPhiFj5UQ_QGzj-G7J5vFMQwPxhY0xwtk,629
-pysgconnect-1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pysgconnect-1.2.dist-info/METADATA,sha256=3ca3C0B-AJMPLBr8ChwqvkNERZDxRvgW7Ce8a4jd308,1091
-pysgconnect-1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pysgconnect-1.2.dist-info/top_level.txt,sha256=QANQzh-nv5EwLpNuSOlEquL2b4DkOfY0AdifeVHQ9Sw,12
-pysgconnect-1.2.dist-info/RECORD,,
+pysgconnect-2.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pysgconnect-2.2.1.dist-info/METADATA,sha256=2cK-ahiP-6N7q6lACqgWilTOmBkCZjpPu9mY4rOQkA4,1093
+pysgconnect-2.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pysgconnect-2.2.1.dist-info/top_level.txt,sha256=QANQzh-nv5EwLpNuSOlEquL2b4DkOfY0AdifeVHQ9Sw,12
+pysgconnect-2.2.1.dist-info/RECORD,,
```

