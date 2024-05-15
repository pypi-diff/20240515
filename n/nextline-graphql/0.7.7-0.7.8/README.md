# Comparing `tmp/nextline_graphql-0.7.7.tar.gz` & `tmp/nextline_graphql-0.7.8.tar.gz`

## Comparing `nextline_graphql-0.7.7.tar` & `nextline_graphql-0.7.8.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/__about__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/py.typed
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/config/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/config/default.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/custom/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/custom/strawberry.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/hook/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/hook/spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/__init__.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/__init__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/test.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script2.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/RunAndContinue.gql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/__init__.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/mutation.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/query.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/subscription.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/plugin.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/schema/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/dev/schema/query.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/plugin.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/graphql/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/schema/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/schema/query.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/__init__.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/funcs.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/LICENSE
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/README.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 nextline_graphql-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/__about__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/py.typed
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/config/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/config/default.toml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/custom/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/custom/strawberry.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/hook/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/hook/spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/__init__.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/test.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/script.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/script2.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/mutations/LoadExampleScript.gql
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/mutations/RunAndContinue.gql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/mutation.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/query.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/subscription.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/dev/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/dev/plugin.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/dev/schema/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/dev/schema/query.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/plugin.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/graphql/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/schema/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/schema/query.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/test/__init__.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/test/funcs.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/LICENSE
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/README.md
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 nextline_graphql-0.7.8/PKG-INFO
```

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/factory.py` & `nextline_graphql-0.7.8/nextlinegraphql/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/config/__init__.py` & `nextline_graphql-0.7.8/nextlinegraphql/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/config/default.toml` & `nextline_graphql-0.7.8/nextlinegraphql/config/default.toml`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/custom/strawberry.py` & `nextline_graphql-0.7.8/nextlinegraphql/custom/strawberry.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/hook/__init__.py` & `nextline_graphql-0.7.8/nextlinegraphql/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/hook/spec.py` & `nextline_graphql-0.7.8/nextlinegraphql/hook/spec.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/__init__.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/test.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 from typing import Any, Optional
 
-from async_asgi_testclient import TestClient
 from nextline.utils import agen_with_wait
 
 from nextlinegraphql.plugins.ctrl.graphql import (
     MUTATE_EXEC,
     MUTATE_RESET,
     MUTATE_SEND_PDB_COMMAND,
     QUERY_STATE,
     SUBSCRIBE_PROMPTING,
     SUBSCRIBE_STATE,
     SUBSCRIBE_TRACE_IDS,
 )
-from nextlinegraphql.plugins.graphql.test import gql_request, gql_subscribe
+from nextlinegraphql.plugins.graphql.test import TestClient, gql_request, gql_subscribe
 
 
 async def run_statement(client, statement: Optional[str] = None):
     variables = {"statement": statement}
     data = await gql_request(client, MUTATE_RESET, variables=variables)
     assert data["reset"]
```

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/graphql/__init__.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/graphql/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pwd = Path(__file__).resolve().parent
 
 sub = pwd / 'mutations'
 MUTATE_EXEC = (sub / 'Exec.gql').read_text()
 MUTATE_RESET = (sub / 'Reset.gql').read_text()
 MUTATE_SEND_PDB_COMMAND = (sub / 'SendPdbCommand.gql').read_text()
 MUTATE_RUN_AND_CONTINUE = (sub / 'RunAndContinue.gql').read_text()
+MUTATE_LOAD_EXAMPLE_SCRIPT = (sub / 'LoadExampleScript.gql').read_text()
 
 sub = pwd / 'queries'
 QUERY_STATE = (sub / 'State.gql').read_text()
 QUERY_EXCEPTION = (sub / 'Exception.gql').read_text()
 QUERY_SOURCE = (sub / 'Source.gql').read_text()
 QUERY_SOURCE_LINE = (sub / 'SourceLine.gql').read_text()
```

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/query.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,16 +45,23 @@
 
 def query_continuous_enabled(info: Info) -> bool:
     nextline: Nextline = info.context["nextline"]
     return nextline.continuous_enabled
 
 
 @strawberry.type
-class Query:
+class QueryCtrl:
     hello: str = strawberry.field(resolver=query_hello)
     state: str = strawberry.field(resolver=query_state)
     run_no: int = strawberry.field(resolver=query_run_no)
     trace_ids: tuple[int, ...] = strawberry.field(resolver=query_trace_ids)
     source: list[str] = strawberry.field(resolver=query_source)
     source_line: str = strawberry.field(resolver=query_source_line)
     exception: Optional[str] = strawberry.field(resolver=query_exception)
     continuous_enabled: bool = strawberry.field(resolver=query_continuous_enabled)
+
+
+@strawberry.type
+class Query:
+    @strawberry.field
+    def ctrl(self) -> QueryCtrl:
+        return QueryCtrl()
```

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/ctrl/schema/subscription.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/ctrl/schema/subscription.py`

 * *Files 23% similar despite different names*

```diff
@@ -69,28 +69,28 @@
 def subscribe_continuous_enabled(info: Info) -> AsyncIterator[bool]:
     nextline: Nextline = info.context["nextline"]
     return nextline.subscribe_continuous_enabled()
 
 
 @strawberry.type
 class Subscription:
-    counter: AsyncIterator[int] = strawberry.field(
+    ctrl_counter: AsyncIterator[int] = strawberry.field(
         is_subscription=True, resolver=subscribe_counter
     )
-    state: AsyncIterator[str] = strawberry.field(
+    ctrl_state: AsyncIterator[str] = strawberry.field(
         is_subscription=True, resolver=subscribe_state
     )
-    run_no: AsyncIterator[int] = strawberry.field(
+    ctrl_run_no: AsyncIterator[int] = strawberry.field(
         is_subscription=True, resolver=subscribe_run_no
     )
-    trace_ids: AsyncIterator[tuple[int, ...]] = strawberry.field(
+    ctrl_trace_ids: AsyncIterator[tuple[int, ...]] = strawberry.field(
         is_subscription=True, resolver=subscribe_trace_ids
     )
-    prompting: AsyncIterator[PromptingData] = strawberry.field(
+    ctrl_prompting: AsyncIterator[PromptingData] = strawberry.field(
         is_subscription=True, resolver=subscribe_prompting
     )
-    stdout: AsyncIterator[str] = strawberry.field(
+    ctrl_stdout: AsyncIterator[str] = strawberry.field(
         is_subscription=True, resolver=subscribe_stdout
     )
-    continuous_enabled: AsyncIterator[bool] = strawberry.field(
+    ctrl_continuous_enabled: AsyncIterator[bool] = strawberry.field(
         is_subscription=True, resolver=subscribe_continuous_enabled
     )
```

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/plugin.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/nextlinegraphql/plugins/graphql/test/funcs.py` & `nextline_graphql-0.7.8/nextlinegraphql/plugins/graphql/test/funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,84 +2,84 @@
 from typing import Any, Optional, TypedDict
 
 from async_asgi_testclient import TestClient
 from async_asgi_testclient.response import Response
 
 
 class PostRequest(TypedDict, total=False):
-    """GraphQL POST Request
+    '''GraphQL POST Request
     https://graphql.org/learn/serving-over-http/#post-request
-    """
+    '''
 
     query: str
     variables: dict[str, Any]
     operationName: str
 
 
 class SubscribePayload(TypedDict):
     variables: dict[str, Any]
     extensions: dict[str, Any]
     operationName: Any
     query: str
 
 
 class SubscribeMessage(TypedDict):
-    """GraphQL over WebSocket Protocol
+    '''GraphQL over WebSocket Protocol
 
     The type of the payload might depend on the value of the type.
     SubscribePayload might be only for the type "start".
     https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md#subscribe
     https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md
-    """
+    '''
 
     id: str
     type: str
     payload: SubscribePayload
 
 
 async def gql_request(
     client: TestClient,
     query: str,
     variables: Optional[dict[str, Any]] = None,
 ) -> Any:
     resp = await gql_request_response(client, query, variables)
     result = resp.json()
-    if err := result.get("errors"):
+    if err := result.get('errors'):
         raise Exception(err)
-    return result["data"]
+    return result['data']
 
 
 async def gql_request_response(
     client: TestClient,
     query: str,
     variables: Optional[dict[str, Any]] = None,
 ) -> Response:
     request = PostRequest(query=query)
     if variables:
-        request["variables"] = variables
+        request['variables'] = variables
 
-    headers = {"Content-Type:": "application/json"}
+    headers = {'Content-Type:': 'application/json'}
 
-    return await client.post("/", json=request, headers=headers)
+    return await client.post('/', json=request, headers=headers)
 
 
 async def gql_subscribe(
     client: TestClient,
     query: str,
     variables: Optional[dict[str, Any]] = None,
 ) -> AsyncGenerator[Any, None]:
     payload = SubscribePayload(
         variables=variables or {},
         extensions={},
         operationName=None,
         query=query,
     )
 
-    message = SubscribeMessage(id="1", type="start", payload=payload)
+    message = SubscribeMessage(id='1', type='start', payload=payload)
 
-    async with client.websocket_connect("/") as ws:
+    async with client.websocket_connect('/') as ws:
         await ws.send_json(message)
         while True:
             resp_json = await ws.receive_json()
-            if resp_json["type"] == "complete":
+            if resp_json['type'] == 'complete':
                 break
-            yield resp_json["payload"]["data"]
+            yield resp_json['payload']['data']
```

### Comparing `nextline_graphql-0.7.7/.gitignore` & `nextline_graphql-0.7.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/LICENSE` & `nextline_graphql-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.7.7/README.md` & `nextline_graphql-0.7.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-graphql.svg)](https://pypi.org/project/nextline-graphql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-graphql.svg)](https://pypi.org/project/nextline-graphql)
+
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test-dev.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-graphql/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-graphql)
 
 # nextline-graphql
 
@@ -20,16 +21,14 @@
     - [External plugins](#external-plugins)
   - [Web App](#web-app)
 - [How to run the Nextline backend API server](#how-to-run-the-nextline-backend-api-server)
   - [As a Docker container](#as-a-docker-container)
   - [In a virtual environment](#in-a-virtual-environment)
 - [Configuration](#configuration)
 - [Check out code for development](#check-out-code-for-development)
-- [License](#license)
-- [Contact](#contact)
 
 ## Introduction
 
 _Nextline_ is a DAQ sequencer of the [Observatory Control System
 (OCS)](https://github.com/simonsobs/ocs/). Nextline allows line-by-line
 execution of concurrent Python scripts, which control telescopes, by multiple
 users simultaneously from web browsers.
@@ -149,19 +148,7 @@
 ```
 
 To run
 
 ```bash
 uvicorn --port 8080 --lifespan on --factory --reload --reload-dir nextline-graphql --reload-dir nextline nextlinegraphql:create_app
 ```
-
----
-
-## License
-
-- _Nextline_ is licensed under the MIT license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

### Comparing `nextline_graphql-0.7.7/pyproject.toml` & `nextline_graphql-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "nextline>=0.7.4",
-    "apluggy>=0.9.9",
+    "nextline>=0.7.5",
+    "apluggy>=1.0",
     "dynaconf>=3.2",
     "starlette>=0.31",
     "strawberry-graphql>=0.213",
     "websockets>=12.0",
     "rich>=13.6",
+    "async-asgi-testclient>=1.4",
 ]
 
 [project.optional-dependencies]
 dev = ["black", "flake8", "logging_tree", "mypy", "tox", "twine", "uvicorn"]
 tests = [
-    "async-asgi-testclient>=1.4",
     "pytest-asyncio>=0.21",
     "pytest-cov>=4.1",
     "pytest-timeout>=2.2",
     "pytest>=7.4",
     "syrupy>=4.6",
 ]
```

### Comparing `nextline_graphql-0.7.7/PKG-INFO` & `nextline_graphql-0.7.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.3
 Name: nextline-graphql
-Version: 0.7.7
+Version: 0.7.8
 Summary: A GraphQL API for Nextline
 Project-URL: Homepage, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
-Requires-Dist: apluggy>=0.9.9
+Requires-Dist: apluggy>=1.0
+Requires-Dist: async-asgi-testclient>=1.4
 Requires-Dist: dynaconf>=3.2
-Requires-Dist: nextline>=0.7.4
+Requires-Dist: nextline>=0.7.5
 Requires-Dist: rich>=13.6
 Requires-Dist: starlette>=0.31
 Requires-Dist: strawberry-graphql>=0.213
 Requires-Dist: websockets>=12.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: logging-tree; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Requires-Dist: uvicorn; extra == 'dev'
 Provides-Extra: tests
-Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'tests'
 Requires-Dist: pytest-cov>=4.1; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.2; extra == 'tests'
 Requires-Dist: pytest>=7.4; extra == 'tests'
 Requires-Dist: syrupy>=4.6; extra == 'tests'
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-graphql.svg)](https://pypi.org/project/nextline-graphql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-graphql.svg)](https://pypi.org/project/nextline-graphql)
+
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test-dev.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-graphql/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-graphql/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-graphql/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-graphql)
 
 # nextline-graphql
 
@@ -59,16 +60,14 @@
     - [External plugins](#external-plugins)
   - [Web App](#web-app)
 - [How to run the Nextline backend API server](#how-to-run-the-nextline-backend-api-server)
   - [As a Docker container](#as-a-docker-container)
   - [In a virtual environment](#in-a-virtual-environment)
 - [Configuration](#configuration)
 - [Check out code for development](#check-out-code-for-development)
-- [License](#license)
-- [Contact](#contact)
 
 ## Introduction
 
 _Nextline_ is a DAQ sequencer of the [Observatory Control System
 (OCS)](https://github.com/simonsobs/ocs/). Nextline allows line-by-line
 execution of concurrent Python scripts, which control telescopes, by multiple
 users simultaneously from web browsers.
@@ -188,19 +187,7 @@
 ```
 
 To run
 
 ```bash
 uvicorn --port 8080 --lifespan on --factory --reload --reload-dir nextline-graphql --reload-dir nextline nextlinegraphql:create_app
 ```
-
----
-
-## License
-
-- _Nextline_ is licensed under the MIT license.
-
----
-
-## Contact
-
-- [Tai Sakuma](https://github.com/TaiSakuma) <span itemscope itemtype="https://schema.org/Person"><a itemprop="sameAs" content="https://orcid.org/0000-0003-3225-9861" href="https://orcid.org/0000-0003-3225-9861" target="orcid.widget" rel="me noopener noreferrer" style="vertical-align:text-top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon"></a></span>
```

