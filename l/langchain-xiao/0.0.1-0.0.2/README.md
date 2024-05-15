# Comparing `tmp/langchain_xiao-0.0.1.tar.gz` & `tmp/langchain_xiao-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_xiao-0.0.1.tar", last modified: Fri Apr 26 08:59:48 2024, max compression
+gzip compressed data, was "langchain_xiao-0.0.2.tar", last modified: Wed May 15 09:06:48 2024, max compression
```

## Comparing `langchain_xiao-0.0.1.tar` & `langchain_xiao-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.748391 langchain_xiao-0.0.1/
--rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.1/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      898 2024-04-26 08:59:48.747373 langchain_xiao-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-04-26 08:56:28.000000 langchain_xiao-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.727023 langchain_xiao-0.0.1/langchain_xiao/
--rw-rw-rw-   0        0        0       23 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.735069 langchain_xiao-0.0.1/langchain_xiao/chat_models/
--rw-rw-rw-   0        0        0       74 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/chat_models/__init__.py
--rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/chat_models/baichuan.py
--rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/chat_models/llamacpp.py
--rw-rw-rw-   0        0        0     1219 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/langchain_xiao/chat_models/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.736142 langchain_xiao-0.0.1/langchain_xiao/embeddings/
--rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/embeddings/__init__.py
--rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/embeddings/fastllm.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.739137 langchain_xiao-0.0.1/langchain_xiao/llms/
--rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/llms/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/llms/gpt4all.py
--rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/langchain_xiao/llms/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.740136 langchain_xiao-0.0.1/langchain_xiao/retrievers/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.741798 langchain_xiao-0.0.1/langchain_xiao/retrievers/document_compressors/
--rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/retrievers/document_compressors/__init__.py
--rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.1/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.746374 langchain_xiao-0.0.1/langchain_xiao.egg-info/
--rw-rw-rw-   0        0        0      898 2024-04-26 08:59:48.000000 langchain_xiao-0.0.1/langchain_xiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-04-26 08:59:48.000000 langchain_xiao-0.0.1/langchain_xiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:59:48.000000 langchain_xiao-0.0.1/langchain_xiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-26 08:59:48.000000 langchain_xiao-0.0.1/langchain_xiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 08:59:48.000000 langchain_xiao-0.0.1/langchain_xiao.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 08:59:48.748904 langchain_xiao-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 08:59:48.745378 langchain_xiao-0.0.1/tests/
--rw-rw-rw-   0        0        0     1040 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/tests/chat_models_utils.py
--rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/tests/fastllm_embeddings.py
--rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/tests/fastllm_rerank.py
--rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.1/tests/llms_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.515916 langchain_xiao-0.0.2/
+-rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      949 2024-05-15 09:06:48.514916 langchain_xiao-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.456089 langchain_xiao-0.0.2/langchain_xiao/
+-rw-rw-rw-   0        0        0       23 2024-05-15 09:04:17.000000 langchain_xiao-0.0.2/langchain_xiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.484123 langchain_xiao-0.0.2/langchain_xiao/chat_models/
+-rw-rw-rw-   0        0        0      102 2024-05-15 09:01:59.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/__init__.py
+-rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/baichuan.py
+-rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/llamacpp.py
+-rw-rw-rw-   0        0        0     1235 2024-05-15 09:01:26.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.491734 langchain_xiao-0.0.2/langchain_xiao/embeddings/
+-rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/embeddings/fastllm.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.499733 langchain_xiao-0.0.2/langchain_xiao/llms/
+-rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/llms/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/llms/gpt4all.py
+-rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/langchain_xiao/llms/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.500733 langchain_xiao-0.0.2/langchain_xiao/retrievers/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.508917 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/
+-rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/__init__.py
+-rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.513917 langchain_xiao-0.0.2/langchain_xiao.egg-info/
+-rw-rw-rw-   0        0        0      949 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:06:48.515916 langchain_xiao-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.512916 langchain_xiao-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1095 2024-05-15 09:05:12.000000 langchain_xiao-0.0.2/tests/chat_models_utils.py
+-rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/fastllm_embeddings.py
+-rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/fastllm_rerank.py
+-rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/llms_utils.py
```

### Comparing `langchain_xiao-0.0.1/.gitignore` & `langchain_xiao-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/LICENSE` & `langchain_xiao-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/PKG-INFO` & `langchain_xiao-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.1
+Version: 0.0.2
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +18,12 @@
 License-File: LICENSE
 Requires-Dist: langchain-core>=0.1.45
 Requires-Dist: langchain-community>=0.0.34
 Requires-Dist: pydantic<=1.10.15
 
 # langchain-xiao
 langchain扩展包
+
+## 安装
+```
+pip install langchain-xiao
+```
```

### Comparing `langchain_xiao-0.0.1/langchain_xiao/chat_models/baichuan.py` & `langchain_xiao-0.0.2/langchain_xiao/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao/chat_models/llamacpp.py` & `langchain_xiao-0.0.2/langchain_xiao/chat_models/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao/chat_models/utils.py` & `langchain_xiao-0.0.2/langchain_xiao/chat_models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from langchain_core.language_models import BaseChatModel
 
 
 XIAO_CHAT_MODELS = [
     "ChatLlamaCpp",
     "MyChatBaichuan",
+    "ChatCyou"
 ]
 
 
 def get_chat_model(instance_type: str, **model_kwargs: Any) -> BaseChatModel:
     if instance_type == "ChatOpenAI":
         try:
             from langchain_openai import ChatOpenAI
```

### Comparing `langchain_xiao-0.0.1/langchain_xiao/embeddings/fastllm.py` & `langchain_xiao-0.0.2/langchain_xiao/embeddings/fastllm.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao/llms/gpt4all.py` & `langchain_xiao-0.0.2/langchain_xiao/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao/llms/utils.py` & `langchain_xiao-0.0.2/langchain_xiao/llms/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py` & `langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/langchain_xiao.egg-info/PKG-INFO` & `langchain_xiao-0.0.2/langchain_xiao.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.1
+Version: 0.0.2
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +18,12 @@
 License-File: LICENSE
 Requires-Dist: langchain-core>=0.1.45
 Requires-Dist: langchain-community>=0.0.34
 Requires-Dist: pydantic<=1.10.15
 
 # langchain-xiao
 langchain扩展包
+
+## 安装
+```
+pip install langchain-xiao
+```
```

### Comparing `langchain_xiao-0.0.1/langchain_xiao.egg-info/SOURCES.txt` & `langchain_xiao-0.0.2/langchain_xiao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/pyproject.toml` & `langchain_xiao-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.1/tests/chat_models_utils.py` & `langchain_xiao-0.0.2/tests/chat_models_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 async def main():
     # instance_type = "ChatLlamaCpp"
     # model_kwargs = {
     #     "model_path": r"E:\WorkSpace\LLMWorkSpace\Models\LLM\qwen\Qwen1.5-0.5B-Chat-GGUF\qwen1_5-0_5b-chat-q5_k_m.gguf",
     #     "verbose": True,
     # }
-    instance_type = "ChatOpenAI"
+    instance_type = "ChatCyou"
     model_kwargs = {
-        "model_name": "moonshot-v1-8k",
-        "openai_api_key": "sk-xxx",
-        "openai_api_base": "https://api.moonshot.cn/v1",
+        "client_id": "a01a4923df7a43b39a4923df7a33b34c",
+        "private_key": "3cJB7EJH",
+        "api_base": "http://43.143.110.198:20001",
     }
 
     chat_model = get_chat_model(instance_type, **model_kwargs)
-    messages = [
-        SystemMessage(content="你是一个聪明的助手，请根据用户的提示来完成任务"),
-        HumanMessage(content="介绍一下你自己"),
-    ]
-    print(await chat_model.ainvoke(messages))
-    # async for chunk in chat_model.astream(messages):
-    #     print(chunk)
+    # chat_model.invoke("你是谁")
+    # messages = [
+    #     SystemMessage(content="你是一个聪明的助手，请根据用户的提示来完成任务"),
+    #     HumanMessage(content="介绍一下你自己"),
+    # ]
+    # print(await chat_model.ainvoke(messages))
+    async for chunk in chat_model.astream("你是谁"):
+        print(chunk)
 
 
 if __name__ == "__main__":
     import asyncio
     asyncio.run(main())
```

### Comparing `langchain_xiao-0.0.1/tests/fastllm_rerank.py` & `langchain_xiao-0.0.2/tests/fastllm_rerank.py`

 * *Files identical despite different names*

