# Comparing `tmp/docmesh_core-0.0.1.tar.gz` & `tmp/docmesh_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.1.tar` & `docmesh_core-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-10 11:02:39.301355 docmesh_core-0.0.1/README.md
--rw-r--r--   0        0        0       22 2024-05-13 03:58:25.558297 docmesh_core-0.0.1/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1092 2024-05-12 15:13:18.166469 docmesh_core-0.0.1/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-10 11:07:24.642695 docmesh_core-0.0.1/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    10070 2024-05-13 02:09:44.402228 docmesh_core-0.0.1/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      379 2024-05-11 04:30:05.745437 docmesh_core-0.0.1/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-10 11:02:39.301355 docmesh_core-0.0.1/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3496 2024-05-11 04:34:00.106569 docmesh_core-0.0.1/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 03:58:49.882596 docmesh_core-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-14 06:50:36.660302 docmesh_core-0.0.2/docmesh_core/__init__.py
+-rw-r--r--   0        0        0     1234 2024-05-14 02:57:17.145280 docmesh_core-0.0.2/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.2/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0    10850 2024-05-14 02:57:07.949200 docmesh_core-0.0.2/docmesh_core/db/neo.py
+-rw-r--r--   0        0        0      417 2024-05-13 10:34:53.297212 docmesh_core-0.0.2/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.2/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.2/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.2/PKG-INFO
```

### Comparing `docmesh_core-0.0.1/docmesh_core/db/__init__.py` & `docmesh_core-0.0.2/docmesh_core/db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 from .neo import (
     Entity,
     Paper,
+    DuplicateEntity,
     get_entity,
     add_entity,
     follow_entity,
     list_follows,
     list_popular_entities,
     get_paper_from_id,
     get_paper_from_title,
     add_paper_from_title,
     add_paper_from_arxiv,
+    update_papers,
     read_paper,
     list_latest_papers,
     list_unread_similar_papers,
     list_unread_semantic_papers,
     list_unread_follows_papers,
     list_unread_influential_papers,
+    list_unembedded_papers,
     get_latest_citegraph,
 )
 from .auth import (
     add_auth_for_entity,
     get_auth_from_entity,
     get_entity_from_auth,
 )
 
 __all__ = [
     "Entity",
     "Paper",
+    "DuplicateEntity",
     "get_entity",
     "add_entity",
     "follow_entity",
     "list_follows",
     "list_popular_entities",
     "get_paper_from_id",
     "get_paper_from_title",
     "add_paper_from_title",
     "add_paper_from_arxiv",
+    "update_papers",
     "read_paper",
     "list_latest_papers",
     "list_unread_similar_papers",
     "list_unread_semantic_papers",
     "list_unread_follows_papers",
     "list_unread_influential_papers",
+    "list_unembedded_papers",
     "get_latest_citegraph",
     "add_auth_for_entity",
     "get_auth_from_entity",
     "get_entity_from_auth",
 ]
```

### Comparing `docmesh_core-0.0.1/docmesh_core/db/auth.py` & `docmesh_core-0.0.2/docmesh_core/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.1/docmesh_core/db/neo.py` & `docmesh_core-0.0.2/docmesh_core/db/neo.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     get_paper_id_from_arxiv,
     get_references,
     get_paper_details,
     PaperIdNotFound,
 )
 
 
+class DuplicateEntity(Exception): ...
+
+
 class FollowRel(StructuredRel):
     since = DateTimeProperty(default_now=True, index=True)
 
 
 class ReadRel(StructuredRel):
     read_time = DateTimeProperty(default_now=True, index=True)
 
@@ -87,14 +90,17 @@
 def get_entity(entity_name: str) -> Entity:
     entity = Entity.nodes.get(name=entity_name)
     return entity
 
 
 @db.transaction
 def add_entity(entity_name: str) -> Entity:
+    if Entity.nodes.get_or_none(name=entity_name) is not None:
+        raise DuplicateEntity(f"{entity_name} already exists, please change the name.")
+
     entity: Entity = Entity.create_or_update({"name": entity_name})
     return entity
 
 
 @db.transaction
 def follow_entity(follower_name: str, follow_name: str) -> None:
     follower_entity = get_entity(follower_name)
@@ -193,14 +199,20 @@
         raise PaperIdNotFound(f"Cannot find semantic scholar paper id from arxiv {arxiv_id}.")
 
     paper = _add_paper(paper_id)
     return paper
 
 
 @db.transaction
+def update_papers(papers: DataFrame) -> list[Paper]:
+    papers: list[Paper] = Paper.create_or_update(*papers.to_dict(orient="records"))
+    return papers
+
+
+@db.transaction
 def read_paper(entity_name: str, paper_id: str) -> None:
     entity = get_entity(entity_name)
     paper = get_paper_from_id(paper_id=paper_id)
     # XXX: neomodel says that they can ensure relationship uniqueness
     # however, it doesn't
     if not entity.reads.is_connected(paper):
         entity.reads.connect(paper)
@@ -334,14 +346,30 @@
         )
     )
 
     return df
 
 
 @db.transaction
+def list_unembedded_papers() -> DataFrame:
+    # XXX: use cypher query language, since OGM is not well supported
+    query = """
+        MATCH (p:Paper)
+        WHERE p.embedding_te3l IS NULL
+        RETURN p.paper_id AS paper_id, p.title AS title, p.abstract AS abstract, p.summary AS summary
+        LIMIT 500;
+    """
+    df = to_dataframe(
+        db.cypher_query(query),
+    )
+
+    return df
+
+
+@db.transaction
 def get_latest_citegraph(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e1:Entity) -[r:read]-> (p1:Paper) -[:cite]-> (p2:Paper) <-[:read]- (e2:Entity)
         WHERE e1.name = $name AND e2.name = $entity_name
         RETURN p1.paper_id AS p1_paper_id, p2.paper_id AS p2_paper_id
         ORDER BY r.read_time DESC
```

### Comparing `docmesh_core-0.0.1/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.2/docmesh_core/utils/semantic_scholar.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,28 @@
     rsp = requests.get(url, headers=headers)
     rsp.raise_for_status()
 
     paper_id = rsp.json().get("paperId", None)
     return paper_id
 
 
+def get_paper_id(paper: str) -> Optional[str]:
+    try:
+        title_paper_id = get_paper_id_from_title(paper)
+    except Exception:
+        title_paper_id = None
+
+    try:
+        arxiv_paper_id = get_paper_id_from_arxiv(paper)
+    except Exception:
+        arxiv_paper_id = None
+
+    return title_paper_id if title_paper_id is not None else arxiv_paper_id
+
+
 @retry(tries=3)
 def get_references(paper_id: str) -> list[str]:
     fields = ["references"]
     details = _get_details([paper_id], fields)
 
     references = details[0]["references"]
     paper_ids = [ref["paperId"] for ref in references if ref["paperId"] is not None]
```

### Comparing `docmesh_core-0.0.1/pyproject.toml` & `docmesh_core-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.1/PKG-INFO` & `docmesh_core-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

