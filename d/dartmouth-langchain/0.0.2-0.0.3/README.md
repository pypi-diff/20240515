# Comparing `tmp/dartmouth_langchain-0.0.2.tar.gz` & `tmp/dartmouth_langchain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dartmouth_langchain-0.0.2.tar", last modified: Wed Mar 13 02:44:10 2024, max compression
+gzip compressed data, was "dartmouth_langchain-0.0.3.tar", last modified: Wed May 15 14:17:16 2024, max compression
```

## Comparing `dartmouth_langchain-0.0.2.tar` & `dartmouth_langchain-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-03-13 02:44:10.659260 dartmouth_langchain-0.0.2/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.2/LICENSE
--rw-r--r--   0 f006pfk    (502) staff       (20)     1815 2024-03-13 02:44:10.659018 dartmouth_langchain-0.0.2/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)     1069 2024-03-12 21:23:53.000000 dartmouth_langchain-0.0.2/README.md
--rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-03-13 02:44:00.000000 dartmouth_langchain-0.0.2/pyproject.toml
--rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-03-13 02:44:10.659301 dartmouth_langchain-0.0.2/setup.cfg
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-03-13 02:44:10.656261 dartmouth_langchain-0.0.2/src/
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-03-13 02:44:10.657392 dartmouth_langchain-0.0.2/src/dartmouth_langchain/
--rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain/__init__.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      496 2024-03-13 02:41:01.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain/base.py
--rw-r--r--   0 f006pfk    (502) staff       (20)      109 2024-03-12 21:03:36.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain/definitions.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     1680 2024-03-12 21:15:05.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain/embeddings.py
--rw-r--r--   0 f006pfk    (502) staff       (20)     2231 2024-03-12 21:14:05.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain/llms.py
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-03-13 02:44:10.658739 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1815 2024-03-13 02:44:10.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/PKG-INFO
--rw-r--r--   0 f006pfk    (502) staff       (20)      458 2024-03-13 02:44:10.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-03-13 02:44:10.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-03-13 02:44:10.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/requires.txt
--rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-03-13 02:44:10.000000 dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/top_level.txt
-drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-03-13 02:44:10.658249 dartmouth_langchain-0.0.2/tests/
--rw-r--r--   0 f006pfk    (502) staff       (20)     1125 2024-03-12 20:57:08.000000 dartmouth_langchain-0.0.2/tests/tests.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.786057 dartmouth_langchain-0.0.3/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1068 2024-03-12 21:00:11.000000 dartmouth_langchain-0.0.3/LICENSE
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:17:16.785827 dartmouth_langchain-0.0.3/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1070 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/README.md
+-rw-r--r--   0 f006pfk    (502) staff       (20)      713 2024-05-15 14:14:51.000000 dartmouth_langchain-0.0.3/pyproject.toml
+-rw-r--r--   0 f006pfk    (502) staff       (20)       38 2024-05-15 14:17:16.786104 dartmouth_langchain-0.0.3/setup.cfg
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.781896 dartmouth_langchain-0.0.3/src/
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.783762 dartmouth_langchain-0.0.3/src/dartmouth_langchain/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-03-12 20:49:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      805 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/base.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      836 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/cross_encoders.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)      163 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/definitions.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1776 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/embeddings.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2728 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/llms.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.784734 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/
+-rw-r--r--   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/__init__.py
+-rw-r--r--   0 f006pfk    (502) staff       (20)     3305 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain/retrievers/document_compressors.py
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.785522 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     1816 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 f006pfk    (502) staff       (20)      606 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)        1 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       61 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/requires.txt
+-rw-r--r--   0 f006pfk    (502) staff       (20)       20 2024-05-15 14:17:16.000000 dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/top_level.txt
+drwxr-xr-x   0 f006pfk    (502) staff       (20)        0 2024-05-15 14:17:16.784894 dartmouth_langchain-0.0.3/tests/
+-rw-r--r--   0 f006pfk    (502) staff       (20)     2486 2024-05-15 14:13:51.000000 dartmouth_langchain-0.0.3/tests/tests.py
```

### Comparing `dartmouth_langchain-0.0.2/LICENSE` & `dartmouth_langchain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dartmouth_langchain-0.0.2/PKG-INFO` & `dartmouth_langchain-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,10 +52,10 @@
 
 ```{python}
 from dartmouth_langchain import DartmouthEmbeddingsModel
 
 
 embeddings = DartmouthEmbeddingsModel()
 
-embeddings.embed_query("Hello? Is there anybody in there?)
+embeddings.embed_query("Hello? Is there anybody in there?")
 ```
```

### Comparing `dartmouth_langchain-0.0.2/README.md` & `dartmouth_langchain-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,10 +34,10 @@
 
 ```{python}
 from dartmouth_langchain import DartmouthEmbeddingsModel
 
 
 embeddings = DartmouthEmbeddingsModel()
 
-embeddings.embed_query("Hello? Is there anybody in there?)
+embeddings.embed_query("Hello? Is there anybody in there?")
 ```
```

### Comparing `dartmouth_langchain-0.0.2/src/dartmouth_langchain/embeddings.py` & `dartmouth_langchain-0.0.3/src/dartmouth_langchain/embeddings.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,38 +9,35 @@
 class DartmouthEmbeddings(HuggingFaceHubEmbeddings, AuthenticatedMixin):
     """
     Extends the LangChain class HuggingFaceHubEmbeddings for more convenient
     interaction with Dartmouth's instance of Text Embeddings Inference
     """
 
     authenticator: Callable = None
+    """A Callable returning a JSON Web Token (JWT) for authentication"""
     dartmouth_api_key: str = None
+    """A Dartmouth API key (obtainable from https://developer.dartmouth.edu)"""
     jwt_url: str = None
+    """URL of the Dartmouth API endpoint returning a JSON Web Token (JWT)"""
 
     def __init__(
         self,
-        *args,
         dartmouth_api_key: str = None,
-        model=None,
         model_name="bge-large-en-v1-5",
         authenticator: Callable = None,
         jwt_url: str = None,
-        **kwargs,
     ):
-        f"""
+        """
         Initializes the object
 
         Args:
             dartmouth_api_key (str, optional): A valid Dartmouth API key (see https://developer.dartmouth.edu/keys).
                 If not specified, it is attempted to be inferred from an environment variable DARTMOUTH_API_KEY.
             model_name (str, optional): Name of the model to use. Defaults to "bge-large-en-v1-5".
             authenticator (Callable, optional): A Callable that returns a valid JWT to use for authentication.
                 If specified, `dartmouth_api_key` is ignored.
         """
-        if model:
-            kwargs["model"] = model
-        else:
-            kwargs["model"] = f"{EMBEDDINGS_BASE_URL}{model_name}/"
-        super().__init__(*args, **kwargs)
+        endpoint = f"{EMBEDDINGS_BASE_URL}{model_name}/"
+        super().__init__(model=endpoint)
         self.authenticator = authenticator
         self.dartmouth_api_key = dartmouth_api_key
         self.authenticate(jwt_url=jwt_url)
```

### Comparing `dartmouth_langchain-0.0.2/src/dartmouth_langchain/llms.py` & `dartmouth_langchain-0.0.3/src/dartmouth_langchain/llms.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,47 +10,55 @@
 class DartmouthChatModel(HuggingFaceTextGenInference, AuthenticatedMixin):
     """
     Extends the LangChain class HuggingFaceTextGenInference for more convenient
     interaction with Dartmouth's instance of Text Generation Inference
     """
 
     authenticator: Callable = None
+    """A Callable returning a JSON Web Token (JWT) for authentication"""
     dartmouth_api_key: str = None
+    """A Dartmouth API key (obtainable from https://developer.dartmouth.edu)"""
     jwt_url: str = None
+    """URL of the Dartmouth API endpoint returning a JSON Web Token (JWT)"""
 
     def __init__(
         self,
-        *args,
         dartmouth_api_key: str = None,
         model_name="llama-2-13b-chat-hf",
         authenticator: Callable = None,
         jwt_url: str = None,
         inference_server_url: str = None,
-        **kwargs,
     ):
-        f"""
+        """
         Initializes the object
 
         Args:
             dartmouth_api_key (str, optional): A valid Dartmouth API key (see https://developer.dartmouth.edu/keys).
-                If not specified, it is attempted to be inferred from an environment variable {ENV_NAMES["dartmouth_api_key"]}.
+                If not specified, it is attempted to be inferred from an environment variable DARTMOUTH_API_KEY.
             model_name (str, optional): Name of the model to use. Defaults to "llama-2-13b-chat-hf".
             authenticator (Callable, optional): A Callable that returns a valid JWT to use for authentication.
                 If specified, `dartmouth_api_key` is ignored.
-            inference_server_url (str, optional): URL pointing to an inference endpoint. Defaults to '{LLM_BASE_URL}{model_name}/'.
+            inference_server_url (str, optional): URL pointing to an inference endpoint. Defaults to "https://ai-api.dartmouth.edu/tgi/".
         """
-        if inference_server_url:
-            kwargs["inference_server_url"] = inference_server_url
-        else:
-            kwargs["inference_server_url"] = f"{LLM_BASE_URL}{model_name}/"
-        super().__init__(*args, **kwargs)
+        if inference_server_url is None:
+            inference_server_url = f"{LLM_BASE_URL}{model_name}/"
+        super().__init__(inference_server_url=inference_server_url)
         self.authenticator = authenticator
         self.dartmouth_api_key = dartmouth_api_key
-        self.authenticate(jwt_url=jwt_url)
+        self.jwt_url = jwt_url
+        self.authenticate(jwt_url=self.jwt_url)
 
     def invoke(self, *args, **kwargs) -> str:
         """Invokes the model to get a response to a query."""
         try:
             return super().invoke(*args, **kwargs)
         except KeyError:
-            self.authenticate()
+            self.authenticate(jwt_url=self.jwt_url)
             return super().invoke(*args, **kwargs)
+
+    async def ainvoke(self, *args, **kwargs) -> str:
+        """Invokes the model to get a response to a query."""
+        try:
+            return super().ainvoke(*args, **kwargs)
+        except KeyError:
+            self.authenticate(jwt_url=self.jwt_url)
+            return super().ainvoke(*args, **kwargs)
```

### Comparing `dartmouth_langchain-0.0.2/src/dartmouth_langchain.egg-info/PKG-INFO` & `dartmouth_langchain-0.0.3/src/dartmouth_langchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartmouth_langchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: LangChain components for Dartmouth-hosted models.
 Author-email: Simon Stone <simon.stone@dartmouth.edu>
 Project-URL: Homepage, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain
 Project-URL: Issues, https://git.dartmouth.edu/lib-digital-strategies/RDS/projects/dartmouth-langchain/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,10 +52,10 @@
 
 ```{python}
 from dartmouth_langchain import DartmouthEmbeddingsModel
 
 
 embeddings = DartmouthEmbeddingsModel()
 
-embeddings.embed_query("Hello? Is there anybody in there?)
+embeddings.embed_query("Hello? Is there anybody in there?")
 ```
```

