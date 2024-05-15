# Comparing `tmp/yellowbox_snowglobe-0.2.4.tar.gz` & `tmp/yellowbox_snowglobe-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowbox_snowglobe-0.2.4.tar", max compression
+gzip compressed data, was "yellowbox_snowglobe-0.2.5.tar", max compression
```

## Comparing `yellowbox_snowglobe-0.2.4.tar` & `yellowbox_snowglobe-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/LICENSE
--rw-r--r--   0        0        0      522 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      157 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/__init__.py
--rw-r--r--   0        0        0       22 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/_version.py
--rw-r--r--   0        0        0     7532 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/api.py
--rw-r--r--   0        0        0     1426 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/case_mode.py
--rw-r--r--   0        0        0      508 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/schema_init.py
--rw-r--r--   0        0        0     1834 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/service.py
--rw-r--r--   0        0        0     6423 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/session.py
--rw-r--r--   0        0        0     6810 2024-01-24 08:13:37.817092 yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/snow_to_post.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 yellowbox_snowglobe-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2348 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-15 10:33:22.791842 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/_version.py
+-rw-r--r--   0        0        0     7738 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/api.py
+-rw-r--r--   0        0        0     1427 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/case_mode.py
+-rw-r--r--   0        0        0      508 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/schema_init.py
+-rw-r--r--   0        0        0     1961 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/service.py
+-rw-r--r--   0        0        0     6506 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/session.py
+-rw-r--r--   0        0        0     6688 2024-05-15 10:32:46.959349 yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/snow_to_post.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 yellowbox_snowglobe-0.2.5/PKG-INFO
```

### Comparing `yellowbox_snowglobe-0.2.4/LICENSE` & `yellowbox_snowglobe-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/api.py` & `yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,169 +1,177 @@
 from __future__ import annotations
 
 import gzip
 import json
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from traceback import print_exc
-from typing import Any, Callable, Container, Dict, List, Optional, Sequence
+from typing import Any, Callable, Container, Dict, Optional, Sequence
 from uuid import uuid4
 
 from sqlalchemy.engine import Row
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 from yellowbox.extras.postgresql import PostgreSQLService
 from yellowbox.extras.webserver import WebServer, class_http_endpoint
 
 from yellowbox_snowglobe.case_mode import CaseMode
 from yellowbox_snowglobe.session import SnowGlobeSession
 from yellowbox_snowglobe.snow_to_post import snow_to_post, split_sql_to_statements
 
 
-async def unpack_request_body(request: Request):
+async def unpack_request_body(request: Request) -> dict:
     body = await request.body()
     uz = gzip.decompress(body)
     return json.loads(uz)
 
 
 @dataclass
 class SnowType:
     """
     A column type that can be returned to the connector
     """
+
     name: str
     connector_converter: Optional[Callable[[Any], Any]] = None
     """
     This converter is used to convert the python value to a value the connector can use (currently only used for bools)
     """
 
 
 PY_TYPE_TO_SNOW_TYPE = {
-    int: SnowType('NUMBER'),
-    str: SnowType('TEXT'),
-    float: SnowType('FLOAT'),
-    bool: SnowType('BOOLEAN', lambda x: str(int(x))),
-    datetime: SnowType('TIMESTAMP_NTZ', lambda x: str(x.replace(tzinfo=timezone.utc).timestamp()))
+    int: SnowType("NUMBER"),
+    str: SnowType("TEXT"),
+    float: SnowType("FLOAT"),
+    bool: SnowType("BOOLEAN", lambda x: str(int(x))),
+    datetime: SnowType("TIMESTAMP_NTZ", lambda x: str(x.replace(tzinfo=timezone.utc).timestamp())),
 }  # todo there are a lot more
 
-OBJECT = SnowType('OBJECT')  # this will be the default snow type for when we can't handle the result type
+OBJECT = SnowType("OBJECT")  # this will be the default snow type for when we can't handle the result type
 
 
 class SnowGlobeAPI(WebServer):
     def __init__(self, *args, sql_service: PostgreSQLService, metadata_table_name: str, case_mode: CaseMode, **kwargs):
-        super().__init__('snowglobe', *args, **kwargs)
+        super().__init__("snowglobe", *args, **kwargs)
         self.sql_service = sql_service
         self.case_mode = case_mode
 
         self.sessions: Dict[str, SnowGlobeSession] = {}  # stores all the live sessions
         self.metadata_table_name = metadata_table_name
 
         self.query_results: Dict[str, Sequence[Row] | None] = {}  # stores all the async query results
 
-    def sql_alchemy_result_to_snowglobe_result(self, result: List[Row], known_columns: Container[str])\
-            -> Dict[str, Any]:
+    def sql_alchemy_result_to_snowglobe_result(
+        self, result: Sequence[Row], known_columns: Container[str]
+    ) -> Dict[str, Any]:
         col_names = result[0]._fields
-        columns = [{'name': self.case_mode.convert(col_name, known_columns), "length": 0, "precision": 0, "scale": 0,
-                    "nullable": False} for col_name in col_names]
+        columns = [
+            {
+                "name": self.case_mode.convert(col_name, known_columns),
+                "length": 0,
+                "precision": 0,
+                "scale": 0,
+                "nullable": False,
+            }
+            for col_name in col_names
+        ]
         rows = [list(row) for row in result]
         for i, col in enumerate(columns):
             t = None
             for row in rows:
                 if row[i] is None:
-                    col['nullable'] = True
+                    col["nullable"] = True
                 else:
                     proposed_type = PY_TYPE_TO_SNOW_TYPE.get(type(row[i]))
                     if proposed_type is None:
                         # unrecognized type, call it a variant and be done with it
                         t = OBJECT
                     elif t is None:
                         t = proposed_type
                     elif t != proposed_type:
                         # type conflict (I don't know if this can even happen), call it a variant
                         t = OBJECT
             if t is None:
                 # if no type was found, we default the column type to variant, AFAICT this will only happen for a result
                 # without rows
                 t = OBJECT
-            col['type'] = t.name
+            col["type"] = t.name
             if t.connector_converter is not None:
                 for row in rows:
                     row[i] = t.connector_converter(row[i]) if row[i] is not None else None
-        return {'rowtype': columns, 'rowset': rows}
+        return {"rowtype": columns, "rowset": rows}
 
-    def session_from_request(self, request):
+    def session_from_request(self, request: Request) -> SnowGlobeSession:
         """
         Get a request's relevant session
         """
-        auth = request.headers.get('Authorization')
+        auth = request.headers.get("Authorization")
         if not auth:
-            raise HTTPException(status_code=401, detail='No Authorization header')
+            raise HTTPException(status_code=401, detail="No Authorization header")
         if not auth.startswith('Snowflake Token="'):
-            raise HTTPException(status_code=401, detail='Invalid Authorization header')
+            raise HTTPException(status_code=401, detail="Invalid Authorization header")
         token = auth[17:-1]
         if token not in self.sessions:
-            raise HTTPException(status_code=401, detail='Invalid Authorization header')
+            raise HTTPException(status_code=401, detail="Invalid Authorization header")
         return self.sessions[token]
 
-    @class_http_endpoint(['POST'], '/session/v1/login-request')  # type: ignore[arg-type]
-    async def login_request(self, request: Request):
-        db = request.query_params.get('databaseName')
-        schema = request.query_params.get('schemaName', 'public')
+    @class_http_endpoint(["POST"], "/session/v1/login-request")  # type: ignore[arg-type]
+    async def login_request(self, request: Request) -> JSONResponse:
+        db = request.query_params.get("databaseName")
+        schema = request.query_params.get("schemaName", "public")
         session = SnowGlobeSession(self, db, schema)
         self.sessions[session.token] = session
-        return JSONResponse({'data': {'token': session.token, 'masterToken': 'SwordFish'}, 'success': True})
+        return JSONResponse({"data": {"token": session.token, "masterToken": "SwordFish"}, "success": True})
 
-    @class_http_endpoint(['POST'], '/session')  # type: ignore[arg-type]
-    async def delete_session(self, request: Request):
-        if request.query_params.get('delete') == 'true':
+    @class_http_endpoint(["POST"], "/session")  # type: ignore[arg-type]
+    async def delete_session(self, request: Request) -> JSONResponse | Response:
+        if request.query_params.get("delete") == "true":
             session = self.session_from_request(request)
             del self.sessions[session.token]
             session.close()
-            return JSONResponse({'success': True})
+            return JSONResponse({"success": True})
         return Response(status_code=404)
 
-    @class_http_endpoint(['POST'], '/queries/v1/query-request')  # type: ignore[arg-type]
-    async def query_request(self, request: Request):
+    @class_http_endpoint(["POST"], "/queries/v1/query-request")  # type: ignore[arg-type]
+    async def query_request(self, request: Request) -> JSONResponse:
         try:
             session = self.session_from_request(request)
             body = await unpack_request_body(request)
-            query = body['sqlText']
-            if query.endswith(';'):
+            query = body["sqlText"]
+            if query.endswith(";"):
                 query = query[:-1]
             post = snow_to_post(query)  # note that this query might well now have multiple statements, but only the
             # last one counts
             stmts = list(split_sql_to_statements(post))
             if not stmts:
-                return JSONResponse({'success': False, 'message': 'no query provided'})
+                return JSONResponse({"success": False, "message": "no query provided"})
             result = None
             for stmt in stmts:
                 result = session.do_query(stmt)
             query_id = str(uuid4())
-            data = {
-                'finalDatabaseName': session.db,
-                'finalSchemaName': session.schema,
+            data: dict = {
+                "finalDatabaseName": session.db,
+                "finalSchemaName": session.schema,
                 "rowtype": [],
                 "rowset": [],
                 "queryId": query_id,
             }
-            if body.get('asyncExec', False):
+            if body.get("asyncExec", False):
                 # we should store the result in the server for when it gets retrieved
                 self.query_results[query_id] = result
             if not result:
-                return JSONResponse({'data': data, 'success': True})
+                return JSONResponse({"data": data, "success": True})
             data.update(self.sql_alchemy_result_to_snowglobe_result(result, session.known_columns))
-            return JSONResponse({'data': data, 'success': True})
+            return JSONResponse({"data": data, "success": True})
         except Exception as e:
             print_exc()  # we print exec here because the connector + webservice combo doesn't always do a good job of
             # telling us what the error is (or that it's happening)
-            return JSONResponse({'success': False, 'message': str(e)})
+            return JSONResponse({"success": False, "message": str(e)})
 
-    @class_http_endpoint(['GET'], '/monitoring/queries/{query_id:str}')  # type: ignore[arg-type]
-    async def query_monitoring_query(self, request: Request):
-        query_id = request.path_params['query_id']
+    @class_http_endpoint(["GET"], "/monitoring/queries/{query_id:str}")  # type: ignore[arg-type]
+    async def query_monitoring_query(self, request: Request) -> JSONResponse:
+        query_id = request.path_params["query_id"]
         if query_id not in self.query_results:
-            return JSONResponse({'success': False, 'message': 'query not found'})
+            return JSONResponse({"success": False, "message": "query not found"})
         # note that we always execute synchronously, so we can just return a static success
-        return JSONResponse({'data': {
-            'queries': [{"status": 'SUCCESS'}]
-        }, 'success': True})
+        return JSONResponse({"data": {"queries": [{"status": "SUCCESS"}]}, "success": True})
```

### Comparing `yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/case_mode.py` & `yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/case_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 
 @dataclass
 class AutoCase(CaseMode):
     """
     Will dynamically fetch all column names from the database and convert them to uppercase
     """
+
     force_ignore: Container[str] = ()
     """
     These column names will not be changed even if they appear in the database
     """
     force_upper: Container[str] = ()
     """
     These column names will be converted to uppercase even if they do not appear in the database
```

### Comparing `yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/service.py` & `yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,62 @@
+from __future__ import annotations
+
+from typing import Any
+
 from yellowbox import AsyncRunMixin, RunMixin, YellowService
 from yellowbox.extras.postgresql import PostgreSQLService
 from yellowbox.utils import docker_host_name
 
 from yellowbox_snowglobe.api import SnowGlobeAPI
 from yellowbox_snowglobe.case_mode import CaseMode, IgnoreAll
 
 
 class SnowGlobeService(YellowService, RunMixin, AsyncRunMixin):
-    def __init__(self, *args, metadata_table_name: str = '__snowglobe_md', case_mode: CaseMode = IgnoreAll(), **kwargs):
+    def __init__(self, *args, metadata_table_name: str = "__snowglobe_md", case_mode: CaseMode = IgnoreAll(), **kwargs):
         super().__init__()
         self.sql_service = PostgreSQLService(*args, **kwargs)
-        self.api = SnowGlobeAPI(sql_service=self.sql_service, metadata_table_name=metadata_table_name,
-                                case_mode=case_mode)
+        self.api = SnowGlobeAPI(
+            sql_service=self.sql_service, metadata_table_name=metadata_table_name, case_mode=case_mode
+        )
 
     @property
-    def api_port(self):
+    def api_port(self) -> int:
         # the http port snowflake connectors should use to connect
         return self.api.port
 
-    def start(self, *args, **kwargs):
+    def start(self, *args, **kwargs) -> SnowGlobeService:
         self.sql_service.start(*args, **kwargs)
         self.api.start()
         return self
 
-    async def astart(self, *args, **kwargs):
+    async def astart(self, *args, **kwargs) -> Any:
         await self.sql_service.astart(*args, **kwargs)
         self.api.start()
         return self
 
-    def stop(self, *args):
+    def stop(self, *args) -> None:
         self.api.stop()
         self.sql_service.stop(*args)
 
     def is_alive(self) -> bool:
         return self.api.is_alive() and self.sql_service.is_alive()
 
-    def _base_connection_kwargs(self):
-        return dict(
-            port=self.api_port,
-            user='MyUser',
-            password='MyPass',
-            account='MyAccount',
-            protocol='http',
-        )
+    def _base_connection_kwargs(self) -> dict:
+        return {
+            "port": self.api_port,
+            "user": "MyUser",
+            "password": "MyPass",
+            "account": "MyAccount",
+            "protocol": "http",
+        }
 
-    def local_connection_kwargs(self):
+    def local_connection_kwargs(self) -> dict:
         return {
-            'host': 'localhost',
+            "host": "localhost",
             **self._base_connection_kwargs(),
         }
 
-    def container_connection_kwargs(self):
+    def container_connection_kwargs(self) -> dict:
         return {
-            'host': docker_host_name,
+            "host": docker_host_name,
             **self._base_connection_kwargs(),
         }
```

### Comparing `yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/session.py` & `yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     @property
     def transaction(self) -> Transaction:
         if not self._transaction:
             raise Exception("No connection exists, make sure to use a database first")
         return self._transaction
 
-    def switch_db(self, db_name: str, schema_name: str = 'public'):
+    def switch_db(self, db_name: str, schema_name: str = "public"):
         if self.db == db_name:
             return
         if self.engine:
             self.engine.dispose()
         self.db = db_name
         conn_string = self.owner.sql_service.database(db_name).local_connection_string()
         self.engine = create_engine(conn_string)
@@ -61,20 +61,24 @@
 
     def _initialize_schema(self):
         """
         create all the necessary snowglobe conversions in the current schema
         """
         with self.connection.begin_nested():
             # right now, the only indicator of initialization is the presence of the metadata table
-            exists = self.connection.execute(text(f"SELECT EXISTS(SELECT FROM information_schema.tables"
-                                                  f" WHERE  table_schema = '{self.schema}'"
-                                                  f" AND table_name = '{self.owner.metadata_table_name}')")).scalar()
+            exists = self.connection.execute(
+                text(
+                    f"SELECT EXISTS(SELECT FROM information_schema.tables"
+                    f" WHERE  table_schema = '{self.schema}'"
+                    f" AND table_name = '{self.owner.metadata_table_name}')"
+                )
+            ).scalar()
             if exists:
                 return
-            self.connection.execute(text(f'SET search_path TO {self.schema};'))
+            self.connection.execute(text(f"SET search_path TO {self.schema};"))
             self.connection.execute(SCHEMA_INITIALIZE_SCRIPT)
             self.connection.execute(text(f"CREATE TABLE IF NOT EXISTS {self.owner.metadata_table_name}()"))
 
     def do_query(self, query: str) -> QUERY_RESPONSE:
         # queries are always normalized to be without a semicolon
         query_lower = query.lower()
         prefix_search_root: Any = self.FUNC_BY_PREFIX
@@ -86,55 +90,57 @@
             prefix_search_root = prefix_search_root.get(word) or prefix_search_root.get(None)
             if not prefix_search_root:
                 print(f"Unknown query: {query}")
                 return None
         return prefix_search_root(self, query)
 
     # region handlers
-    def _do_ignore(self, query) -> QUERY_RESPONSE:
+    def _do_ignore(self, query: str) -> QUERY_RESPONSE:
         return None
 
-    def _do_commit(self, query) -> QUERY_RESPONSE:
+    def _do_commit(self, query: str) -> QUERY_RESPONSE:
         self.transaction.commit()
         return None
 
-    def _do_rollback(self, query) -> QUERY_RESPONSE:
+    def _do_rollback(self, query: str) -> QUERY_RESPONSE:
         self.transaction.rollback()
         return None
 
-    def _do_use_database(self, query) -> QUERY_RESPONSE:
+    def _do_use_database(self, query: str) -> QUERY_RESPONSE:
         _, _, db_name = query.rpartition(" ")
         self.switch_db(db_name)
         return None
 
-    def _do_set_schema(self, query) -> QUERY_RESPONSE:
+    def _do_set_schema(self, query: str) -> QUERY_RESPONSE:
         _, _, schema_name = query.rpartition(" ")
         # todo assert the schema exists
         self.schema = schema_name
         self._initialize_schema()
         return None
 
-    def _do_retrieve(self, query) -> QUERY_RESPONSE:
+    def _do_retrieve(self, query: str) -> QUERY_RESPONSE:
         _, _, query_id = query.rpartition(" ")
         res = self.owner.query_results.pop(query_id, None)
         if res is None:
             return None  # todo some better handling here?
         return res
 
-    def _do_select(self, query) -> QUERY_RESPONSE:
+    def _do_select(self, query: str) -> QUERY_RESPONSE:
         result = self.connection.execute(text(query)).all()
         return result
 
-    def _do_mutating_noresponse(self, query) -> QUERY_RESPONSE:
+    def _do_mutating_noresponse(self, query: str) -> QUERY_RESPONSE:
         self.connection.execute(text(query))
         # we need to update the known columns here
-        result = self.connection.execute(text(
-            "select column_name from information_schema.columns c where c.table_schema <> 'pg_catalog'"
-            "AND c.table_schema <> 'information_schema';"
-        ))
+        result = self.connection.execute(
+            text(
+                "select column_name from information_schema.columns c where c.table_schema <> 'pg_catalog'"
+                "AND c.table_schema <> 'information_schema';"
+            )
+        )
         self.known_columns = set(result.scalars().fetchall())
         return None
 
     # endregion
 
     # here we map SQL keywords to whichever handler we want to use on queries with them
     # think of this like a prefix trie, with NONE as a fallback
@@ -144,15 +150,15 @@
         "!rollback": _do_rollback,
         "!switch_db": _do_use_database,
         "!set_schema": _do_set_schema,
         "!retrieve": _do_retrieve,
         "select": _do_select,
         "insert": _do_mutating_noresponse,
         "create": {
-            'database': _do_ignore,
+            "database": _do_ignore,
             None: _do_mutating_noresponse,
         },
         "set": _do_mutating_noresponse,
         "delete": _do_mutating_noresponse,
         "update": _do_mutating_noresponse,
         "alter": {
             "table": _do_mutating_noresponse,
@@ -160,8 +166,9 @@
     }
 
     def close(self):
         if self.engine:
             self.connection.close()
             self.engine.dispose()
 
+
 # todo data types
```

### Comparing `yellowbox_snowglobe-0.2.4/yellowbox_snowglobe/snow_to_post.py` & `yellowbox_snowglobe-0.2.5/yellowbox_snowglobe/snow_to_post.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,35 +28,35 @@
                 # unterminated string literal, we treat everything after the starter as a literal and let the caller
                 # deal with it
                 terminator_ind = len(query)
             if len(query) <= (terminator_ind + 1) or query[terminator_ind + 1] != "'":
                 break
             search_start = terminator_ind + 2
         yield query[:next_str_ind]
-        yield TextLiteral(query[next_str_ind:terminator_ind + 1])
-        query = query[terminator_ind + 1:]
+        yield TextLiteral(query[next_str_ind : terminator_ind + 1])
+        query = query[terminator_ind + 1 :]
 
 
 def split_sql_to_statements(query: str) -> Iterator[str]:
     # splits a compound query to multiple statements, splitting on non-literal ";"
     buffer = []
     for part in split_literals(query):
         if isinstance(part, TextLiteral):
             buffer.append(part.value)
             continue
         while True:
-            sep_index = part.find(';')
+            sep_index = part.find(";")
             if sep_index == -1:
                 buffer.append(part)
                 break
             buffer.append(part[:sep_index])
-            yield ''.join(buffer)
+            yield "".join(buffer)
             buffer.clear()
-            part = part[sep_index + 1:]
-    last_bit = ''.join(buffer)
+            part = part[sep_index + 1 :]
+    last_bit = "".join(buffer)
     if last_bit:
         yield last_bit
 
 
 """
 A Rule is replacement rule that converts a snowflake-dialect query to a postgresql query.
 for example there's a rule that will turn "a..b" into "a.public.b"
@@ -77,94 +77,97 @@
 
 # note that all commands starting with ! are special non-postgres commands for the session to handle specially
 
 # these are special rules that are run before the split_literals, as such they should be used sparingly (you almost
 # always want to add a "^" to the beginning of the pattern)
 PRE_SPLIT_RULES = [
     # retrieved stored asynchronous result
-    Rule(re.compile(r"(?i)^select\s+\*\s+from\s+table\(result_scan\('([a-f0-9-]+)'\)\)"),
-         r"!retrieve \1"),
+    Rule(re.compile(r"(?i)^select\s+\*\s+from\s+table\(result_scan\('([a-f0-9-]+)'\)\)"), r"!retrieve \1"),
 ]
 
 RULES = [
     # commit/rollback
-    Rule(re.compile(r"(?i)^(commit|rollback)"), r'!\1'),
+    Rule(re.compile(r"(?i)^(commit|rollback)"), r"!\1"),
     # use database
-    Rule(re.compile(r"(?i)use(\s+database)?\s+(" + NAME_PATTERN + r")"), r'!switch_db \2'),
+    Rule(re.compile(r"(?i)use(\s+database)?\s+(" + NAME_PATTERN + r")"), r"!switch_db \2"),
     # use schema
-    Rule(re.compile(r"(?i)use\s+schema\s+(" + NAME_PATTERN + r")"), r'SET search_path TO \1;!set_schema \1'),
-    Rule(re.compile(r"(?i)use(\s+schema)?\s+(" + NAME_PATTERN + r")\.(" + NAME_PATTERN + r")$"),
-         r'USE DATABASE \2;use schema \3'),
+    Rule(re.compile(r"(?i)use\s+schema\s+(" + NAME_PATTERN + r")"), r"SET search_path TO \1;!set_schema \1"),
+    Rule(
+        re.compile(r"(?i)use(\s+schema)?\s+(" + NAME_PATTERN + r")\.(" + NAME_PATTERN + r")$"),
+        r"USE DATABASE \2;use schema \3",
+    ),
     # flatten(?) as ?
-    Rule(re.compile(r"(?ix)\b"
-                    r"flatten\("
-                    r"("
-                    + OBJ_PATTERN
-                    + ")"
-                      r"\)\s+as\s+"
-                      r"(" + NAME_PATTERN + r")\b"), replacement=r"unnest(\1) as \2(value)"),
+    Rule(
+        re.compile(r"(?ix)\b" r"flatten\(" r"(" + OBJ_PATTERN + ")" r"\)\s+as\s+" r"(" + NAME_PATTERN + r")\b"),
+        replacement=r"unnest(\1) as \2(value)",
+    ),
     # db..table
-    Rule(re.compile(r"(?ix)\b"
-                    r"(" + NAME_PATTERN + r")\.\.(" + NAME_PATTERN + ")"
-                    + r"\b"), replacement=r"\1.public.\2"),
-
+    Rule(
+        re.compile(r"(?ix)\b" r"(" + NAME_PATTERN + r")\.\.(" + NAME_PATTERN + ")" + r"\b"), replacement=r"\1.public.\2"
+    ),
     # json query string
-    Rule(re.compile(r"(?ix)\b"
-                    r"(" + NAME_PATTERN + r"):(" + NAME_PATTERN + ")" + "::string"
-                    + r"\b"), replacement=r"\1->>'\2'"),
-
+    Rule(
+        re.compile(r"(?ix)\b" r"(" + NAME_PATTERN + r"):(" + NAME_PATTERN + ")" + "::string" + r"\b"),
+        replacement=r"\1->>'\2'",
+    ),
     # json query int
-    Rule(re.compile(r"(?ix)\b"
-                    r"(" + NAME_PATTERN + r"):(" + NAME_PATTERN + ")" + "::number"
-                    + r"\b"), replacement=r"cast(\1->>'\2' as integer)"),
-
+    Rule(
+        re.compile(r"(?ix)\b" r"(" + NAME_PATTERN + r"):(" + NAME_PATTERN + ")" + "::number" + r"\b"),
+        replacement=r"cast(\1->>'\2' as integer)",
+    ),
     # show schemas
-    Rule(re.compile(r"(?i)show\s+schemas"),
-         "select null as created_on, schema_name as name, null as is_default, null as is_current, "
-         "null as database_name, null as owner, null as comment, null as options, null as retention_time "
-         "FROM information_schema.schemata"),
+    Rule(
+        re.compile(r"(?i)show\s+schemas"),
+        "select null as created_on, schema_name as name, null as is_default, null as is_current, "
+        "null as database_name, null as owner, null as comment, null as options, null as retention_time "
+        "FROM information_schema.schemata",
+    ),
     # show tables
-    Rule(re.compile(r"(?i)show\s+tables"),
-         "select null as created_on, table_name as name, table_catalog as database_name, table_schema as schema_name,"
-         " 'TABLE' as kind, NULL as comment, NULL as cluster_by, NULL as rows, NULL as bytes, NULL as owner,"
-         " NULL as retention_time, NULL as change_tracking, NULL as search_optimization,"
-         " NULL as search_optimization_progress, NULL as search_optimization_bytes, NULL as is_external"
-         " FROM information_schema.tables WHERE table_type = 'BASE TABLE'"),
+    Rule(
+        re.compile(r"(?i)show\s+tables"),
+        "select null as created_on, table_name as name, table_catalog as database_name, table_schema as schema_name,"
+        " 'TABLE' as kind, NULL as comment, NULL as cluster_by, NULL as rows, NULL as bytes, NULL as owner,"
+        " NULL as retention_time, NULL as change_tracking, NULL as search_optimization,"
+        " NULL as search_optimization_progress, NULL as search_optimization_bytes, NULL as is_external"
+        " FROM information_schema.tables WHERE table_type = 'BASE TABLE'",
+    ),
     # describe table
-    Rule(re.compile(r"(?i)(describe|desc)\s+table\s+(" + NAME_PATTERN + r")"),
-         "SELECT column_name as name, data_type as type, 'COLUMN' as kind, is_nullable as \"null?\","
-         " column_default as default, NULL as primary_key, NULL as unique_key, NULL as check,"
-         " NULL as expression, NULL as comment, NULL as \"policy name\" FROM information_schema.columns"
-         r" WHERE table_name = '\2'"),
+    Rule(
+        re.compile(r"(?i)(describe|desc)\s+table\s+(" + NAME_PATTERN + r")"),
+        "SELECT column_name as name, data_type as type, 'COLUMN' as kind, is_nullable as \"null?\","
+        " column_default as default, NULL as primary_key, NULL as unique_key, NULL as check,"
+        ' NULL as expression, NULL as comment, NULL as "policy name" FROM information_schema.columns'
+        r" WHERE table_name = '\2'",
+    ),
     # Ignore sample in queries
     Rule(re.compile(r"(?i)\bsample\s+\(([0-9\.]+)\s+rows\)"), replacement=r"order by random() limit \1"),
 ]
 
 
 def repl_part(part: Union[str, TextLiteral], rules: Iterable[Rule]) -> str:
     if isinstance(part, TextLiteral):
         return part.value
     ret_parts = []
     while part:
         best_match = None
-        best_match_key = (float('inf'), 0)  # matches are ranked by position (shorter is better),
+        best_match_key = (float("inf"), 0)  # matches are ranked by position (shorter is better),
         # then by length (longer is better, stored as negative)
         for rule in rules:
             match = rule.pattern.search(part)
             if match:
                 match_key = (match.start(), -len(match.group()))
                 if match_key < best_match_key:
                     best_match = (rule, match)
                     best_match_key = match_key
         if best_match:
             rule, match = best_match
-            ret_parts.append(part[:match.start()])
-            part = match.expand(rule.replacement) + part[match.end():]
+            ret_parts.append(part[: match.start()])
+            part = match.expand(rule.replacement) + part[match.end() :]
         else:
             ret_parts.append(part)
             break
-    return ''.join(ret_parts)
+    return "".join(ret_parts)
 
 
 def snow_to_post(query: str) -> str:
     query = repl_part(query, PRE_SPLIT_RULES)
-    return ''.join(repl_part(part, RULES) for part in split_literals(query))
+    return "".join(repl_part(part, RULES) for part in split_literals(query))
```

### Comparing `yellowbox_snowglobe-0.2.4/PKG-INFO` & `yellowbox_snowglobe-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: yellowbox-snowglobe
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 License: MIT
 Author: Biocatch LTD
 Author-email: serverteam@biocatch.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: yellowbox[postgresql,webserver] (>=0.7.0)
```

