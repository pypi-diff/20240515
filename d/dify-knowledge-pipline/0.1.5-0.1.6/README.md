# Comparing `tmp/dify_knowledge_pipline-0.1.5.tar.gz` & `tmp/dify_knowledge_pipline-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify_knowledge_pipline-0.1.5.tar", max compression
+gzip compressed data, was "dify_knowledge_pipline-0.1.6.tar", max compression
```

## Comparing `dify_knowledge_pipline-0.1.5.tar` & `dify_knowledge_pipline-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/__init__.py
--rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/client.py
--rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/errors.py
--rw-r--r--   0        0        0    12614 2024-05-15 02:37:34.384299 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/fire_drop.py
--rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/models.py
--rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/pipline.py
--rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.5/LICENSE
--rw-r--r--   0        0        0     2717 2024-05-15 02:37:49.434196 dify_knowledge_pipline-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.5/README.md
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/__init__.py
+-rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/client.py
+-rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/errors.py
+-rw-r--r--   0        0        0    12584 2024-05-15 02:59:44.378647 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/fire_drop.py
+-rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/models.py
+-rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/pipline.py
+-rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2717 2024-05-15 03:00:14.565666 dify_knowledge_pipline-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.6/README.md
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.6/PKG-INFO
```

### Comparing `dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/client.py` & `dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/client.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/errors.py` & `dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/errors.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/fire_drop.py` & `dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/fire_drop.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,16 +193,15 @@
             if status in ["error", "completed"]:
                 break
 
     def list_documents(self, *, db_name: str, table_name: str | None = None):
         if dataset_id := self._hook_knowledge_dataset(db_name=db_name):
             return self._list_documents(dataset_id, table_name=table_name)
 
-    def delete_document(self, *, db_name: str, document_name: str, **kwargs):
-        document_name = kwargs.get("table_name", document_name)
+    def delete_document(self, *, db_name: str, document_name: str):
         if dataset_id := self._hook_knowledge_dataset(db_name=db_name):
             if document_id := self._sync_document_id(dataset_id, document_name):
                 return self._delete_document(dataset_id, document_id)
 
     def embed_knowledge(
         self, table_to_knowledge: Dict[str, str], *, db_name: str, force_override: bool = False
     ):
@@ -264,43 +263,43 @@
         # [操作/新建] 知识库，获取操作句柄
         dataset_id = self._hook_knowledge_dataset(db_name=db_name)
         docs = self._list_documents(dataset_id)
         id2doc = {doc["id"]: doc for doc in docs}
 
         # 通过文本 [更新/创建] 文档，获取操作句柄
         tasks = tqdm(table_to_knowledge.items())
-        for table_name, knowledge_card in tasks:
-            tasks.postfix = f"{db_name=} {table_name=}"
-            if document_id := self._sync_document_id(dataset_id, table_name):
+        for document_name, knowledge_card in tasks:
+            tasks.postfix = f"{db_name=} {document_name=}"
+            if document_id := self._sync_document_id(dataset_id, document_name):
                 # 对比更新时间
                 dify_doc_update_time = id2doc[document_id]["created_at"]
-                external_docs_update_time = table_to_update_time[table_name]
+                external_docs_update_time = table_to_update_time[document_name]
                 if external_docs_update_time > dify_doc_update_time + 3:
                     # 重建知识库文档，更新创建时间，添加 +3s 的节拍同步
                     self._delete_document(dataset_id, document_id)
                     self._create_document_by_text(
-                        dataset_id, table_name=table_name, text=knowledge_card
+                        dataset_id, table_name=document_name, text=knowledge_card
                     )
-                    logger.success(f"重建知识库文档: {table_name}")
+                    logger.success(f"重建知识库文档: {document_name}")
             else:
                 # 新建知识库文档
                 self._create_document_by_text(
-                    dataset_id, table_name=table_name, text=knowledge_card
+                    dataset_id, table_name=document_name, text=knowledge_card
                 )
-                logger.success(f"新建知识库文档: {table_name}")
+                logger.success(f"新建知识库文档: {document_name}")
 
         for doc in docs:
             # 移除多余的知识库文档
-            table_name = doc["name"]
-            if table_name.endswith(".txt"):
-                table_name = table_name.rstrip(".txt")
-            if table_name not in table_to_knowledge:
-                if document_id := self._sync_document_id(dataset_id, table_name):
+            document_name = doc["name"]
+            if document_name.endswith(".txt"):
+                document_name = document_name[:-4]
+            if document_name not in table_to_knowledge:
+                if document_id := self._sync_document_id(dataset_id, document_name):
                     self._delete_document(dataset_id, document_id)
-                    logger.debug(f"Deleted outdated table: {table_name}")
+                    logger.success(f"删除过期的知识库文档: {document_name}")
 
     def delete_all_document(self, *, db_name: str):
         # [操作/新建] 知识库，获取操作句柄
         dataset_id = self._hook_knowledge_dataset(db_name=db_name)
 
         docs = self._list_documents(dataset_id)
         for doc in docs:
```

### Comparing `dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/models.py` & `dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/models.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.5/dify_knowledge_pipline/pipline.py` & `dify_knowledge_pipline-0.1.6/dify_knowledge_pipline/pipline.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.5/LICENSE` & `dify_knowledge_pipline-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.5/pyproject.toml` & `dify_knowledge_pipline-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # https://python-poetry.org/docs/libraries/#versioning
 # https://pypi.org/project/hcaptcha-challenger/#history
 
 [tool.poetry]
 # python -m build && twine upload dist/*
 name = "dify-knowledge-pipline"
-version = "0.1.5"
+version = "0.1.6"
 description = "🥂 Gracefully embedding multimodal-knowledge to Dify"
 license = "Apache License 2.0"
 authors = ["QIN2DIM <yaoqinse@gmail.com>", "Bingjie Yan <bj.yan.pa@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/QIN2DIM/hcaptcha-challenger"
 repository = "https://github.com/QIN2DIM/hcaptcha-challenger"
 documentation = "https://github.com/QIN2DIM/hcaptcha-challenger"
```

### Comparing `dify_knowledge_pipline-0.1.5/PKG-INFO` & `dify_knowledge_pipline-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-knowledge-pipline
-Version: 0.1.5
+Version: 0.1.6
 Summary: 🥂 Gracefully embedding multimodal-knowledge to Dify
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 License: Apache-2.0
 Keywords: dify,RAG,dify-knowledge-pipline,multimodal-knowledge
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 Requires-Python: >=3.10,<4.0
```

