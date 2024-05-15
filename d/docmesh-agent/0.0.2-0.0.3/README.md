# Comparing `tmp/docmesh_agent-0.0.2.tar.gz` & `tmp/docmesh_agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.2.tar` & `docmesh_agent-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.2/README.md
--rw-r--r--   0        0        0       22 2024-05-13 03:47:40.246354 docmesh_agent-0.0.2/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     4050 2024-05-13 02:12:42.888413 docmesh_agent-0.0.2/docmesh_agent/main.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.2/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      857 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/prompt.py
--rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.2/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0      787 2024-05-11 04:38:52.647986 docmesh_agent-0.0.2/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.2/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      741 2024-05-13 03:31:34.698480 docmesh_agent-0.0.2/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0     2299 2024-05-10 11:18:58.249989 docmesh_agent-0.0.2/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3926 2024-05-10 11:19:24.922119 docmesh_agent-0.0.2/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     5226 2024-05-11 05:02:21.234649 docmesh_agent-0.0.2/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     4598 2024-05-13 03:40:24.188988 docmesh_agent-0.0.2/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      718 2024-05-13 03:47:45.210415 docmesh_agent-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 docmesh_agent-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-14 06:51:36.696812 docmesh_agent-0.0.3/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     1785 2024-05-14 06:44:33.137143 docmesh_agent-0.0.3/docmesh_agent/agent.py
+-rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.3/docmesh_agent/embeddings/__init__.py
+-rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.3/docmesh_agent/embeddings/embeddings.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.3/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.3/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      857 2024-05-10 11:02:39.301355 docmesh_agent-0.0.3/docmesh_agent/prompt.py
+-rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.3/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.3/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0      787 2024-05-11 04:38:52.647986 docmesh_agent-0.0.3/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.3/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      741 2024-05-13 03:31:34.698480 docmesh_agent-0.0.3/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.3/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0     2304 2024-05-13 04:13:58.029801 docmesh_agent-0.0.3/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.3/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     5760 2024-05-14 06:38:24.001928 docmesh_agent-0.0.3/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4384 2024-05-14 03:34:39.156802 docmesh_agent-0.0.3/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      680 2024-05-14 06:51:11.184595 docmesh_agent-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 docmesh_agent-0.0.3/PKG-INFO
```

### Comparing `docmesh_agent-0.0.2/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.3/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/prompt.py` & `docmesh_agent-0.0.3/docmesh_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.3/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.3/docmesh_agent/toolkit/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/toolkit/recommend.py` & `docmesh_agent-0.0.3/docmesh_agent/toolkit/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/__init__.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
 from langchain.callbacks.manager import CallbackManagerForToolRun
 
-from docmesh.db.neo import follow_entity, list_follows, list_popular_entities
+from docmesh_core.db.neo import follow_entity, list_follows, list_popular_entities
 from docmesh_agent.tools.base import BaseAgentTool, BaseAgentNoInputTool
 
 
 class FollowEntityToolInput(BaseModel):
     name: str = Field(description="entity name")
```

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/graph_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
 from datetime import datetime
 from langchain.callbacks.manager import CallbackManagerForToolRun
 
-from docmesh.db.neo import get_latest_citegraph
-from docmesh.utils.graph_utils import find_max_degree_nodes
+from docmesh_core.db.neo import get_latest_citegraph
+from docmesh_core.utils.graph_utils import find_max_degree_nodes
 from docmesh_agent.tools.base import BaseAgentTool
 
 
 class CiteGraphToolInput(BaseModel):
     n: str = Field(description="number of papers")
```

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/paper.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/paper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
 from langchain.callbacks.manager import CallbackManagerForToolRun
 
-from docmesh.db.neo import (
+from docmesh_core.db.neo import (
     add_paper_from_title,
     add_paper_from_arxiv,
     read_paper,
     get_paper_from_id,
     get_paper_from_title,
     list_latest_papers,
 )
-from docmesh.utils.semantic_scholar import PaperIdNotFound
+from docmesh_core.utils.semantic_scholar import PaperIdNotFound
 from docmesh_agent.tools.base import BaseAgentTool
 
 
 class AddPaperFromTitleToolInput(BaseModel):
     title: str = Field(description="paper title")
 
 
@@ -77,15 +77,21 @@
 
     def _run(
         self,
         title: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         title = self._preporcess_input(title)
-        paper_id = get_paper_from_title(title=title).paper_id
+        try:
+            paper_id = get_paper_from_title(title=title).paper_id
+        except Exception:
+            self._raise_tool_error(
+                "Input argument `title` should be paper title only, please check your input. "
+                "Pay attention that do not include any special characters like quotes."
+            )
         msg = f"Successfully find paper id {paper_id} for {title}."
         return f"\n{msg}\n"
 
 
 class MarkPaperReadToolInput(BaseModel):
     paper_id: str = Field(description="paper id")
 
@@ -121,15 +127,21 @@
 
     def _run(
         self,
         paper_id: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         paper_id = self._preporcess_input(paper_id)
-        paper = get_paper_from_id(paper_id=paper_id)
+        try:
+            paper = get_paper_from_id(paper_id=paper_id)
+        except Exception:
+            self._raise_tool_error(
+                "Input argument `paper_id` should be a paper id, please check your input. "
+                "Pay attention that paper_id is not arxiv id."
+            )
         msg = paper.summary
         return f"\n{msg}\n"
 
 
 class ListLatestPaperToolInput(BaseModel):
     n: str = Field(description="number of papers")
```

### Comparing `docmesh_agent-0.0.2/docmesh_agent/tools/recommend.py` & `docmesh_agent-0.0.3/docmesh_agent/tools/recommend.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
 from datetime import datetime
 from langchain.callbacks.manager import CallbackManagerForToolRun
 from langchain_openai import OpenAIEmbeddings
 
-from docmesh.db.neo import (
+from docmesh_core.db.neo import (
     list_unread_follows_papers,
     list_unread_influential_papers,
     list_unread_similar_papers,
     list_unread_semantic_papers,
 )
 from docmesh_agent.tools.base import BaseAgentTool
+from docmesh_agent.embeddings.embeddings import query_embeddings
 
 
 class UnreadFollowsToolInput(BaseModel):
     n: str = Field(description="number of papers")
 
 
 class UnreadFollowsTool(BaseAgentTool):
@@ -113,23 +114,15 @@
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         query = self._preporcess_input(query)
-
-        # setup embedding
-        embedding = OpenAIEmbeddings(
-            base_url=os.getenv("OPENAI_EMBEDDING_API_BASE"),
-            api_key=os.getenv("OPENAI_EMBEDDING_API_KEY"),
-            model=os.getenv("OPENAI_EMBEDDING_MODEL"),
-            dimensions=1024,
-        )
-        query_embedded = embedding.embed_query(query)
+        query_embedded = query_embeddings(query)
 
         df = list_unread_semantic_papers(
             entity_name=self.entity_name,
             semantic_embedding=query_embedded,
             n=10,
         )
         # keep score over 0.5 and drop the column
```

### Comparing `docmesh_agent-0.0.2/PKG-INFO` & `docmesh_agent-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh>=0.0.5
+Requires-Dist: docmesh_core>=0.0.2
 Requires-Dist: langchain>=0.1.15
 Requires-Dist: langchain-openai>=0.1.3
-Requires-Dist: fastapi==0.111.0
-Requires-Dist: uvicorn==0.29.0
-Requires-Dist: gunicorn==19.3.0
+Requires-Dist: langchainhub>=0.1.15
 
 # docmesh agent
```

