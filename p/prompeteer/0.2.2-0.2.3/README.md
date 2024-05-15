# Comparing `tmp/prompeteer-0.2.2.tar.gz` & `tmp/prompeteer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.2.2.tar", last modified: Wed May 15 10:01:48 2024, max compression
+gzip compressed data, was "prompeteer-0.2.3.tar", last modified: Wed May 15 10:11:50 2024, max compression
```

## Comparing `prompeteer-0.2.2.tar` & `prompeteer-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.756117 prompeteer-0.2.2/
--rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:01:48.755635 prompeteer-0.2.2/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     2514 2024-05-15 10:01:32.000000 prompeteer-0.2.2/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.746461 prompeteer-0.2.2/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:58:26.000000 prompeteer-0.2.2/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.749367 prompeteer-0.2.2/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.2.2/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.2.2/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 08:29:05.000000 prompeteer-0.2.2/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.750766 prompeteer-0.2.2/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.2.2/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.752237 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1472 2024-05-15 08:59:54.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1781 2024-05-15 09:00:45.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.753833 prompeteer-0.2.2/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1997 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1437 2024-05-15 08:31:53.000000 prompeteer-0.2.2/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.2.2/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.754569 prompeteer-0.2.2/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.2.2/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1019 2024-05-15 07:59:19.000000 prompeteer-0.2.2/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.755180 prompeteer-0.2.2/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 10:01:48.756197 prompeteer-0.2.2/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      837 2024-05-15 10:01:48.000000 prompeteer-0.2.2/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.943614 prompeteer-0.2.3/
+-rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:11:50.943312 prompeteer-0.2.3/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     2514 2024-05-15 10:01:32.000000 prompeteer-0.2.3/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.936076 prompeteer-0.2.3/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:58:26.000000 prompeteer-0.2.3/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 08:19:41.000000 prompeteer-0.2.3/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.939009 prompeteer-0.2.3/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.2.3/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.2.3/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 08:29:05.000000 prompeteer-0.2.3/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.939839 prompeteer-0.2.3/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.2.3/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.941015 prompeteer-0.2.3/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.3/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1396 2024-05-15 10:08:55.000000 prompeteer-0.2.3/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1781 2024-05-15 09:00:45.000000 prompeteer-0.2.3/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.941746 prompeteer-0.2.3/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.3/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1997 2024-05-15 08:19:41.000000 prompeteer-0.2.3/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 08:19:41.000000 prompeteer-0.2.3/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 10:06:33.000000 prompeteer-0.2.3/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.2.3/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.942471 prompeteer-0.2.3/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.2.3/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1019 2024-05-15 07:59:19.000000 prompeteer-0.2.3/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:11:50.942837 prompeteer-0.2.3/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:11:50.000000 prompeteer-0.2.3/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 10:11:50.000000 prompeteer-0.2.3/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 10:11:50.000000 prompeteer-0.2.3/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 10:11:50.000000 prompeteer-0.2.3/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 10:11:50.000000 prompeteer-0.2.3/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 10:11:50.943681 prompeteer-0.2.3/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      837 2024-05-15 10:11:50.000000 prompeteer-0.2.3/setup.py
```

### Comparing `prompeteer-0.2.2/PKG-INFO` & `prompeteer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.2.2/README.md` & `prompeteer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/prompeteer.py` & `prompeteer-0.2.3/prompeteer/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/prompt/prompt.py` & `prompeteer-0.2.3/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/prompt/prompt_config.py` & `prompeteer-0.2.3/prompeteer/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py` & `prompeteer-0.2.3/prompeteer/providers/aws_bedrock/aws_bedrock_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,17 @@
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 from prompeteer.providers.llm_client import ILLMClient
 
 
-def _init_aws_bedrock_client():
-    pass
-
-
 class AwsBedrockClient(ILLMClient):
     def __init__(self):
-        self.client = _init_aws_bedrock_client()
+        self.client = boto3.client(service_name='bedrock-runtime', region_name='us-east-1')
 
     def call(self, llm_request: AWSLLMRequest) -> str:
 
         params: Dict[str, Any] = {
             'messages': [{'role': msg.role, 'content': msg.content} for msg in llm_request.messages],
             'anthropic_version': 'bedrock-2023-05-31',
             'max_tokens': llm_request.max_tokens
@@ -34,13 +30,11 @@
         if llm_request.top_p is not None:
             params['top_p'] = llm_request.top_p
         if llm_request.top_k is not None:
             params['top_k'] = llm_request.top_k
         if llm_request.stop_sequence is not None:
             params['stop_sequence'] = llm_request.stop_sequence
 
-        bedrock_runtime = boto3.client(service_name='bedrock-runtime')
-
-        response = bedrock_runtime.invoke_model(body=json.dumps(params), modelId=llm_request.model)
+        response = self.client.invoke_model(body=json.dumps(params), modelId=llm_request.model)
         response_body = json.loads(response.get('body').read())
 
         return response_body
```

### Comparing `prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_llm_request.py` & `prompeteer-0.2.3/prompeteer/providers/aws_bedrock/aws_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_llm_request.py` & `prompeteer-0.2.3/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.2.3/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer/providers/llm_client.py` & `prompeteer-0.2.3/prompeteer/providers/llm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         logger.error(f"Unknown LLM Provider {provider}")
         raise Exception(f"Unknown LLM Provider {provider}")
 
 
 def get_llm_client(provider: LLMProvider) -> ILLMClient:
     assert provider is not None, "Provider must be provided"
     global clients
-    if provider not in clients:
+    if provider.value not in clients:
         clients[provider.value] = _init_llm_client(provider)
         logger.info(f"LLM Client for {provider} successfully initialized")
     return clients[provider.value]
```

### Comparing `prompeteer-0.2.2/prompeteer/utils/utils.py` & `prompeteer-0.2.3/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.2.3/prompeteer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.2.2/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.2.3/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.2/setup.py` & `prompeteer-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.2.2',
+    version='0.2.3',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*']),  # Include all packages
     py_modules=['prompeteer'],
```

