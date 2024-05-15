# Comparing `tmp/dify_knowledge_pipline-0.1.2.tar.gz` & `tmp/dify_knowledge_pipline-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify_knowledge_pipline-0.1.2.tar", max compression
+gzip compressed data, was "dify_knowledge_pipline-0.1.3.tar", max compression
```

## Comparing `dify_knowledge_pipline-0.1.2.tar` & `dify_knowledge_pipline-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/__init__.py
--rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/client.py
--rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/errors.py
--rw-r--r--   0        0        0    10280 2024-05-15 01:55:50.101958 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/fire_drop.py
--rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/models.py
--rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/pipline.py
--rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.2/LICENSE
--rw-r--r--   0        0        0     2717 2024-05-15 01:55:50.093956 dify_knowledge_pipline-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.2/README.md
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/__init__.py
+-rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/client.py
+-rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/errors.py
+-rw-r--r--   0        0        0    12560 2024-05-15 02:25:28.297147 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/fire_drop.py
+-rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/models.py
+-rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/pipline.py
+-rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2717 2024-05-15 02:25:45.097301 dify_knowledge_pipline-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.3/README.md
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.3/PKG-INFO
```

### Comparing `dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/client.py` & `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/client.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/errors.py` & `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/errors.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/fire_drop.py` & `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/fire_drop.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 class UploadDocumentResponse(BaseModel):
     document: Dict[str, Any] = Field(default_factory=dict)
     batch: str = Field(...)
 
 
 class DifyFireDrop:
     def __init__(
-            self,
-            separator: str | None = None,
-            dify_base_url: str = "http://192.168.1.180/v1",
-            api_key: str | None = None,
+        self,
+        separator: str | None = None,
+        dify_base_url: str = "http://192.168.1.180/v1",
+        api_key: str | None = None,
     ):
         self.my_separator = separator or "\n\n------------\n\n"
 
         if not (_dify_dataset_api_key := os.getenv("DIFY_DATABASE_API_KEY", api_key)):
             parser = urlparse(dify_base_url)
             lu = f"{parser.scheme}://{parser.netloc}/datasets?category=api"
             logger.error(f"DIFY_DATABASE_API_KEY 缺失，去授权 API 密钥 {lu}")
@@ -62,15 +62,15 @@
 
     def _delete_document(self, dataset_id: str, document_id: str):
         url = f"/datasets/{dataset_id}/documents/{document_id}"
         res = self._client.delete(url)
         res.raise_for_status()
 
     def _update_document_by_text(
-            self, dataset_id: str, document_id: str, *, table_name: str, text: str
+        self, dataset_id: str, document_id: str, *, table_name: str, text: str
     ) -> UploadDocumentResponse | None:
         url = f"/datasets/{dataset_id}/documents/{document_id}/update_by_text"
         payload = self._document_preprocess_payload(name=table_name, text=text)
         res = self._client.post(url, json=payload, timeout=30)
         try:
             res.raise_for_status()
         except httpx.HTTPStatusError:
@@ -81,15 +81,15 @@
 
         udr = UploadDocumentResponse(**res.json())
         # document_name = f"{table_name}.txt"
         # logger.debug(f"通过文本更新文档 - {document_name=}")
         return udr
 
     def _create_document_by_text(
-            self, dataset_id: str, *, table_name: str, text: str
+        self, dataset_id: str, *, table_name: str, text: str
     ) -> UploadDocumentResponse:
         """
         通过文本创建知识库文档
 
         自动创建一个 [self.table_name].txt 的知识库文档文件
         Args:
             dataset_id:
@@ -132,15 +132,15 @@
         for document in documents:
             if document["name"] == document_name:
                 document_id = document["id"]
                 # logger.debug(f"获取知识库文档Id - {document_name=} {document_id=}")
                 return document_id
 
     def _list_documents(
-            self, dataset_id: str, table_name: str | None = None
+        self, dataset_id: str, table_name: str | None = None
     ) -> List[Dict[str, Any]]:
         """
 
         :param dataset_id:
         :param table_name:
         :return:
         {
@@ -193,21 +193,22 @@
             if status in ["error", "completed"]:
                 break
 
     def list_documents(self, *, db_name: str, table_name: str | None = None):
         if dataset_id := self._hook_knowledge_dataset(db_name=db_name):
             return self._list_documents(dataset_id, table_name=table_name)
 
-    def delete_document(self, *, db_name: str, table_name: str):
+    def delete_document(self, *, db_name: str, document_name: str, **kwargs):
+        document_name = kwargs.get("table_name", document_name)
         if dataset_id := self._hook_knowledge_dataset(db_name=db_name):
-            if document_id := self._sync_document_id(dataset_id, table_name):
+            if document_id := self._sync_document_id(dataset_id, document_name):
                 return self._delete_document(dataset_id, document_id)
 
     def embed_knowledge(
-            self, table_to_knowledge: Dict[str, str], *, db_name: str, force_override: bool = False
+        self, table_to_knowledge: Dict[str, str], *, db_name: str, force_override: bool = False
     ):
         """
         通过文本更新文档。
 
         - 若知识库不存在则新建知识库
         - 若文档不存在则新建文档
         - 若存在文档则更新文档
@@ -245,14 +246,61 @@
                     )
             else:
                 response = self._create_document_by_text(
                     dataset_id, table_name=table_name, text=knowledge_card
                 )
             response_seq.append(response)
 
+    def embed_knowledge_incremental_updates(
+            self,
+            table_to_knowledge: Dict[str, str],
+            table_to_update_time: Dict[str, int],
+            *,
+            db_name: str,
+    ):
+        if not table_to_knowledge:
+            logger.error("不可以添加空的文档")
+            return
+
+        # [操作/新建] 知识库，获取操作句柄
+        dataset_id = self._hook_knowledge_dataset(db_name=db_name)
+        docs = self._list_documents(dataset_id)
+        id2doc = {doc["id"]: doc for doc in docs}
+
+        # 通过文本 [更新/创建] 文档，获取操作句柄
+        tasks = tqdm(table_to_knowledge.items())
+        for table_name, knowledge_card in tasks:
+            tasks.postfix = f"{db_name=} {table_name=}"
+            if document_id := self._sync_document_id(dataset_id, table_name):
+                # 对比更新时间
+                dify_doc_update_time = id2doc[document_id]["created_at"]
+                external_docs_update_time = table_to_update_time[table_name]
+                if external_docs_update_time > dify_doc_update_time + 3:
+                    # 重建知识库文档，更新创建时间，添加 +3s 的节拍同步
+                    self._delete_document(dataset_id, document_id)
+                    self._update_document_by_text(
+                        dataset_id, document_id, table_name=table_name, text=knowledge_card
+                    )
+                    logger.debug(f"更新知识库文档：{table_name}")
+            else:
+                # 新建知识库文档
+                self._create_document_by_text(
+                    dataset_id, table_name=table_name, text=knowledge_card
+                )
+
+        for doc in docs:
+            # 移除多余的知识库文档
+            table_name = doc["name"]
+            if table_name.endswith(".txt"):
+                table_name = table_name.rstrip(".txt")
+            if table_name not in table_to_knowledge:
+                if document_id := self._sync_document_id(dataset_id, table_name):
+                    self._delete_document(dataset_id, document_id)
+                    logger.debug(f"Deleted outdated table: {table_name}")
+
     def delete_all_document(self, *, db_name: str):
         # [操作/新建] 知识库，获取操作句柄
         dataset_id = self._hook_knowledge_dataset(db_name=db_name)
 
         docs = self._list_documents(dataset_id)
         for doc in docs:
             try:
```

### Comparing `dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/models.py` & `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/models.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.2/dify_knowledge_pipline/pipline.py` & `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/pipline.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.2/LICENSE` & `dify_knowledge_pipline-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.2/pyproject.toml` & `dify_knowledge_pipline-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://python-poetry.org/docs/libraries/#versioning
 # https://pypi.org/project/hcaptcha-challenger/#history
 
 [tool.poetry]
 name = "dify-knowledge-pipline"
-version = "0.1.2"
+version = "0.1.3"
 description = "🥂 Gracefully embedding multimodal-knowledge to Dify"
 license = "Apache License 2.0"
 authors = ["QIN2DIM <yaoqinse@gmail.com>", "Bingjie Yan <bj.yan.pa@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/QIN2DIM/hcaptcha-challenger"
 repository = "https://github.com/QIN2DIM/hcaptcha-challenger"
 documentation = "https://github.com/QIN2DIM/hcaptcha-challenger"
```

### Comparing `dify_knowledge_pipline-0.1.2/PKG-INFO` & `dify_knowledge_pipline-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-knowledge-pipline
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🥂 Gracefully embedding multimodal-knowledge to Dify
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 License: Apache-2.0
 Keywords: dify,RAG,dify-knowledge-pipline,multimodal-knowledge
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 Requires-Python: >=3.10,<4.0
```

