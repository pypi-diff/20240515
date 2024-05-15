# Comparing `tmp/arcee_py-1.0.6.tar.gz` & `tmp/arcee_py-1.0.7.tar.gz`

## Comparing `arcee_py-1.0.6.tar` & `arcee_py-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/__init__.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/api.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/doc.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 arcee_py-1.0.6/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.6/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.6/.gitignore
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 arcee_py-1.0.6/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 arcee_py-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/__init__.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/api.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 arcee_py-1.0.7/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.7/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.7/.gitignore
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 arcee_py-1.0.7/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 arcee_py-1.0.7/PKG-INFO
```

### Comparing `arcee_py-1.0.6/tasks.py` & `arcee_py-1.0.7/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/.github/iced/test.yml` & `arcee_py-1.0.7/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/.github/workflows/publish.yml` & `arcee_py-1.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/arcee/__init__.py` & `arcee_py-1.0.7/arcee/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 import os
 
 from arcee import config
-from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus, upload_alignment
+from arcee.api import upload_docs, upload_corpus_folder, upload_qa_pairs, start_alignment, start_pretraining, start_retriever_training, get_retriever_status, start_deployment, stop_deployment, generate, retrieve, delete_corpus, upload_alignment, start_merging
 from arcee.dalm import DALM, DALMFilter
 
 if not config.ARCEE_API_KEY:
     # We check this because it's impossible the user imported arcee, _then_ set the env, then imported again
     config.ARCEE_API_KEY = os.getenv("ARCEE_API_KEY", "")
     while not config.ARCEE_API_KEY:
         config.ARCEE_API_KEY = input("ARCEE_API_KEY not found in environment. Please input api key: ")
     os.environ["ARCEE_API_KEY"] = config.ARCEE_API_KEY
 
-__all__ = ["upload_docs", "DALM", "DALMFilter", "upload_corpus_folder", "upload_qa_pairs", "start_alignment", "start_pretraining", "start_retriever_training", "get_retriever_status", "start_deployment", "stop_deployment", "generate", "retrieve", "delete_corpus", "upload_alignment"]
+__all__ = ["upload_docs", "DALM", "DALMFilter", "upload_corpus_folder", "upload_qa_pairs", "start_alignment", "start_pretraining", "start_retriever_training", "get_retriever_status", "start_deployment", "stop_deployment", "generate", "retrieve", "delete_corpus", "upload_alignment", "start_merging"]
```

### Comparing `arcee_py-1.0.6/arcee/api.py` & `arcee_py-1.0.7/arcee/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,14 +80,33 @@
         base_model (str): The name of the base model to use
     """
 
     data = {"pretraining_name": pretraining_name, "corpus_name": corpus, "base_model": base_model}
 
     return make_request("post", Route.pretraining+"/startTraining", data)
 
+def start_merging(merging_name: str, arcee_models: Optional[List[str]] = None, hf_models: Optional[List[str]] = None, qa_set_ids: Optional[List[str]] = None, general_evals: Optional[List[str]] = None, base_model: Optional[str] = None, merge_method: Optional[str] = None, time_budget: int = 1) -> None:
+    """
+    Start merging models
+
+    Args:
+        merging_name (str): The name of the merging job
+        arcee_models (list): A list of ARCEE models to merge
+        hf_models (list): A list of Hugging Face models to merge
+        qa_set_ids (list): A list of QA sets to merge
+        general_evals (list): A list of general evaluations to merge
+        base_model (str): The name of the base model to use
+        merge_method (str): The merging method to use
+        time_budget (int): The time budget for the merging job (hourss)
+    """
+
+    data = {"name": merging_name, "arcee_models": arcee_models, "hf_models": hf_models, "qa_set_ids": qa_set_ids, "general_evals": general_evals, "base_model": base_model, "merge_method": merge_method, "time_budget": time_budget}
+
+    return make_request("post", Route.merging+"/startMerging", data)
+
 def delete_corpus(corpus: str) -> None:
     """
     Delete a corpus
 
     Args:
         corpus (str): The name of the corpus to delete
     """
@@ -123,18 +142,19 @@
         f'Retriever model training started - view model status at {status_url} or with arcee.get_retriever_status("{name}")'
     )
 
 def get_retriever_status(id_or_name: str) -> Dict[str, str]:
     """Gets the status of a retriever training job"""
     return check_model_status(id_or_name)
 
-def start_deployment(deployment_name: str, alignment: Optional[str] = None, retriever: Optional[str] = None):
-    data = {"deployment_name": deployment_name, "alignment_name": alignment, "retriever_name": retriever}
+def start_deployment(deployment_name: str, alignment: Optional[str] = None, retriever: Optional[str] = None, target_instance: Optional[str] = None, openai_compatability: Optional[bool] = False):
+    data = {"deployment_name": deployment_name, "alignment_name": alignment, "retriever_name": retriever, "target_instance": target_instance, "openai_compatability": openai_compatability}
     return make_request("post", Route.deployment+"/startDeployment", data)
 
+
 def stop_deployment(deployment_name: str):
     data = {"deployment_name": deployment_name}
     return make_request("post", Route.deployment+"/stopDeployment", data)
 
 def generate(deployment_name: str, query: str):
     data = {"deployment_name": deployment_name, "query": query}
     return make_request("post", Route.deployment+"/generate", data)
```

### Comparing `arcee_py-1.0.6/arcee/api_handler.py` & `arcee_py-1.0.7/arcee/api_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     headers = headers or {}
     internal_headers = {"X-Token": f"{config.ARCEE_API_KEY}", "Content-Type": "application/json"}
     headers.update(**internal_headers)
     url = f"{config.ARCEE_API_URL}/{config.ARCEE_API_VERSION}/{route}"
 
     req_type = getattr(requests, request)
     response = req_type(url, json=body, params=params, headers=headers)
-    if response.status_code not in (200, 201):
+    if response.status_code not in (200, 201, 202):
         raise Exception(f"Failed to make request. Response: {response.text}")
     return response.json()
```

### Comparing `arcee_py-1.0.6/arcee/cli.py` & `arcee_py-1.0.7/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/arcee/cli_handler.py` & `arcee_py-1.0.7/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/arcee/config.py` & `arcee_py-1.0.7/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/arcee/dalm.py` & `arcee_py-1.0.7/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/tests/test_api_handler.py` & `arcee_py-1.0.7/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/.gitignore` & `arcee_py-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/README.md` & `arcee_py-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# DALM by Arcee
+# Arcee Client Docs
 
 The Arcee client for executing domain-adpated language model routines
 
-![Arcee DALMs](https://uploads-ssl.webflow.com/64c95915793c8a64a186e43e/64de2c7fb2c99494dec2e0a4_realistic-lifelike-dalmatian-dog-puppy-pastel-bright-vintage-outfits-commercial%201-min.jpg)
-
-
 ## Installation
 
 ```
 pip install arcee-py
 ```
 
 ## Authenticating
```

### Comparing `arcee_py-1.0.6/pyproject.toml` & `arcee_py-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.6/PKG-INFO` & `arcee_py-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.6
+Version: 1.0.7
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
@@ -21,21 +21,18 @@
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-env; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-requests; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# DALM by Arcee
+# Arcee Client Docs
 
 The Arcee client for executing domain-adpated language model routines
 
-![Arcee DALMs](https://uploads-ssl.webflow.com/64c95915793c8a64a186e43e/64de2c7fb2c99494dec2e0a4_realistic-lifelike-dalmatian-dog-puppy-pastel-bright-vintage-outfits-commercial%201-min.jpg)
-
-
 ## Installation
 
 ```
 pip install arcee-py
 ```
 
 ## Authenticating
```

