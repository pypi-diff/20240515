# Comparing `tmp/dify_knowledge_pipline-0.1.3.tar.gz` & `tmp/dify_knowledge_pipline-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify_knowledge_pipline-0.1.3.tar", max compression
+gzip compressed data, was "dify_knowledge_pipline-0.1.4.tar", max compression
```

## Comparing `dify_knowledge_pipline-0.1.3.tar` & `dify_knowledge_pipline-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/__init__.py
--rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/client.py
--rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/errors.py
--rw-r--r--   0        0        0    12560 2024-05-15 02:25:28.297147 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/fire_drop.py
--rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/models.py
--rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/pipline.py
--rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.3/LICENSE
--rw-r--r--   0        0        0     2717 2024-05-15 02:25:45.097301 dify_knowledge_pipline-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.3/README.md
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/__init__.py
+-rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/client.py
+-rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/errors.py
+-rw-r--r--   0        0        0    12527 2024-05-15 02:32:51.921398 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/fire_drop.py
+-rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/models.py
+-rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/pipline.py
+-rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2717 2024-05-15 02:33:16.693897 dify_knowledge_pipline-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.4/README.md
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.4/PKG-INFO
```

### Comparing `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/client.py` & `dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/client.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/errors.py` & `dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/errors.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/fire_drop.py` & `dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/fire_drop.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
             else:
                 response = self._create_document_by_text(
                     dataset_id, table_name=table_name, text=knowledge_card
                 )
             response_seq.append(response)
 
     def embed_knowledge_incremental_updates(
-            self,
-            table_to_knowledge: Dict[str, str],
-            table_to_update_time: Dict[str, int],
-            *,
-            db_name: str,
+        self,
+        table_to_knowledge: Dict[str, str],
+        table_to_update_time: Dict[str, int],
+        *,
+        db_name: str,
     ):
         if not table_to_knowledge:
             logger.error("不可以添加空的文档")
             return
 
         # [操作/新建] 知识库，获取操作句柄
         dataset_id = self._hook_knowledge_dataset(db_name=db_name)
@@ -273,16 +273,16 @@
             if document_id := self._sync_document_id(dataset_id, table_name):
                 # 对比更新时间
                 dify_doc_update_time = id2doc[document_id]["created_at"]
                 external_docs_update_time = table_to_update_time[table_name]
                 if external_docs_update_time > dify_doc_update_time + 3:
                     # 重建知识库文档，更新创建时间，添加 +3s 的节拍同步
                     self._delete_document(dataset_id, document_id)
-                    self._update_document_by_text(
-                        dataset_id, document_id, table_name=table_name, text=knowledge_card
+                    self._create_document_by_text(
+                        dataset_id, table_name=table_name, text=knowledge_card
                     )
                     logger.debug(f"更新知识库文档：{table_name}")
             else:
                 # 新建知识库文档
                 self._create_document_by_text(
                     dataset_id, table_name=table_name, text=knowledge_card
                 )
```

### Comparing `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/models.py` & `dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/models.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.3/dify_knowledge_pipline/pipline.py` & `dify_knowledge_pipline-0.1.4/dify_knowledge_pipline/pipline.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.3/LICENSE` & `dify_knowledge_pipline-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.3/pyproject.toml` & `dify_knowledge_pipline-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # https://python-poetry.org/docs/libraries/#versioning
 # https://pypi.org/project/hcaptcha-challenger/#history
 
 [tool.poetry]
+# python -m build && twine upload dist/*
 name = "dify-knowledge-pipline"
-version = "0.1.3"
+version = "0.1.4"
 description = "🥂 Gracefully embedding multimodal-knowledge to Dify"
 license = "Apache License 2.0"
 authors = ["QIN2DIM <yaoqinse@gmail.com>", "Bingjie Yan <bj.yan.pa@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/QIN2DIM/hcaptcha-challenger"
 repository = "https://github.com/QIN2DIM/hcaptcha-challenger"
 documentation = "https://github.com/QIN2DIM/hcaptcha-challenger"
@@ -65,10 +66,9 @@
 
 [tool.black]
 line-length = 100
 target-version = ["py310", "py311", "py312"]
 skip-magic-trailing-comma = true
 
 [build-system]
-# python -m build && twine upload dist/*
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dify_knowledge_pipline-0.1.3/PKG-INFO` & `dify_knowledge_pipline-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-knowledge-pipline
-Version: 0.1.3
+Version: 0.1.4
 Summary: 🥂 Gracefully embedding multimodal-knowledge to Dify
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 License: Apache-2.0
 Keywords: dify,RAG,dify-knowledge-pipline,multimodal-knowledge
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 Requires-Python: >=3.10,<4.0
```

