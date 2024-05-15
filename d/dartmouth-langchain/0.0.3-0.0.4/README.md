# Comparing `tmp/dartmouth_langchain-0.0.3.tar.gz` & `tmp/dartmouth_langchain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dartmouth_langchain-0.0.3.tar", last modified: Wed May 15 14:17:16 2024, max compression
+gzip compressed data, was "dartmouth_langchain-0.0.4.tar", last modified: Wed May 15 14:24:44 2024, max compression
```

## Comparing `dartmouth_langchain-0.0.3.tar` & `dartmouth_langchain-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.786057 dartmouth_langchain-0.0.3/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.3/LICENSE
--rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:17:16.785827 dartmouth_langchain-0.0.3/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)     1070 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/README.md
--rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-05-15 14:14:51.000000 dartmouth_langchain-0.0.3/pyproject.toml
--rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-05-15 14:17:16.786104 dartmouth_langchain-0.0.3/setup.cfg
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.781896 dartmouth_langchain-0.0.3/src/
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.783762 dartmouth_langchain-0.0.3/src/dartmouth_langchain/
--rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/__init__.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      805 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/base.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      836 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/cross_encoders.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      163 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/definitions.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     1776 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/embeddings.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     2728 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/llms.py
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.784734 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/
--rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/__init__.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     3305 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/document_compressors.py
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.785522 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)      606 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/requires.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/top_level.txt
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.784894 dartmouth_langchain-0.0.3/tests/
--rw-r--r--   0 f006pfk    (502) staff       (20)     2486 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/tests/tests.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.561924 dartmouth_langchain-0.0.4/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.4/LICENSE
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:24:44.561655 dartmouth_langchain-0.0.4/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1070 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/README.md
+-rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-05-15 14:24:17.000000 dartmouth_langchain-0.0.4/pyproject.toml
+-rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-05-15 14:24:44.561972 dartmouth_langchain-0.0.4/setup.cfg
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.558377 dartmouth_langchain-0.0.4/src/
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.559703 dartmouth_langchain-0.0.4/src/dartmouth_langchain/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      805 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/base.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      836 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/cross_encoders.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      163 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/definitions.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1776 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/embeddings.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2817 2024-05-15 14:23:04.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/llms.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.560619 dartmouth_langchain-0.0.4/src/dartmouth_langchain/retrievers/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/retrievers/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     3305 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain/retrievers/document_compressors.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.561344 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:24:44.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)      606 2024-05-15 14:24:44.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-05-15 14:24:44.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-05-15 14:24:44.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/requires.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-05-15 14:24:44.000000 dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/top_level.txt
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:24:44.560773 dartmouth_langchain-0.0.4/tests/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2504 2024-05-15 14:23:31.000000 dartmouth_langchain-0.0.4/tests/tests.py
```

### Comparing `dartmouth_langchain-0.0.3/LICENSE` & `dartmouth_langchain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/PKG-INFO` & `dartmouth_langchain-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dartmouth_langchain-0.0.3/README.md` & `dartmouth_langchain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/pyproject.toml` & `dartmouth_langchain-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dartmouth_langchain"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Simon Stone", email="simon.stone@dartmouth.edu" },
 ]
 description = "LangChain components for Dartmouth-hosted models."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain/base.py` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain/base.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain/cross_encoders.py` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain/cross_encoders.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain/embeddings.py` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain/llms.py` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain/llms.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,34 +18,38 @@
     dartmouth_api_key: str = None
     """A Dartmouth API key (obtainable from https://developer.dartmouth.edu)"""
     jwt_url: str = None
     """URL of the Dartmouth API endpoint returning a JSON Web Token (JWT)"""
 
     def __init__(
         self,
+        *args,
         dartmouth_api_key: str = None,
         model_name="llama-2-13b-chat-hf",
         authenticator: Callable = None,
         jwt_url: str = None,
         inference_server_url: str = None,
+        **kwargs,
     ):
         """
         Initializes the object
 
         Args:
             dartmouth_api_key (str, optional): A valid Dartmouth API key (see https://developer.dartmouth.edu/keys).
                 If not specified, it is attempted to be inferred from an environment variable DARTMOUTH_API_KEY.
             model_name (str, optional): Name of the model to use. Defaults to "llama-2-13b-chat-hf".
             authenticator (Callable, optional): A Callable that returns a valid JWT to use for authentication.
                 If specified, `dartmouth_api_key` is ignored.
             inference_server_url (str, optional): URL pointing to an inference endpoint. Defaults to "https://ai-api.dartmouth.edu/tgi/".
         """
-        if inference_server_url is None:
-            inference_server_url = f"{LLM_BASE_URL}{model_name}/"
-        super().__init__(inference_server_url=inference_server_url)
+        if inference_server_url:
+            kwargs["inference_server_url"] = inference_server_url
+        else:
+            kwargs["inference_server_url"] = f"{LLM_BASE_URL}{model_name}/"
+        super().__init__(*args, **kwargs)
         self.authenticator = authenticator
         self.dartmouth_api_key = dartmouth_api_key
         self.jwt_url = jwt_url
         self.authenticate(jwt_url=self.jwt_url)
 
     def invoke(self, *args, **kwargs) -> str:
         """Invokes the model to get a response to a query."""
```

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/document_compressors.py` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain/retrievers/document_compressors.py`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/PKG-INFO` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/SOURCES.txt` & `dartmouth_langchain-0.0.4/src/dartmouth_langchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.3/tests/tests.py` & `dartmouth_langchain-0.0.4/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def test_dartmouth_chat():
     llm = DartmouthChatModel()
     response = llm.invoke("<s>[INST]Please respond with the single word OK[/INST]")
     assert response.strip() == "OK"
 
-    llm = DartmouthChatModel(model_name="llama-3-8b-instruct")
+    llm = DartmouthChatModel(model_name="llama-3-8b-instruct", temperature=0.01)
     response = llm.invoke(
         "<|begin_of_text|><|start_header_id|>user<|end_header_id|>\n\nPlease respond with the single word OK<|eot_id|><|start_header_id|>assistant<|end_header_id|>"
     )
     assert response.strip() == "OK"
 
     llm = DartmouthChatModel(model_name="codellama-13b-instruct-hf")
     response = llm.invoke("<s>[INST]Please respond with the single word OK[/INST]")
```

