# Comparing `tmp/prompeteer-0.2.1.tar.gz` & `tmp/prompeteer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.2.1.tar", last modified: Wed May 15 08:11:29 2024, max compression
+gzip compressed data, was "prompeteer-0.2.2.tar", last modified: Wed May 15 10:01:48 2024, max compression
```

## Comparing `prompeteer-0.2.1.tar` & `prompeteer-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.743955 prompeteer-0.2.1/
--rw-r--r--   0 yoaz       (502) staff       (20)     2012 2024-05-15 08:11:29.743573 prompeteer-0.2.1/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     1587 2024-05-15 08:00:18.000000 prompeteer-0.2.1/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.732914 prompeteer-0.2.1/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:58:26.000000 prompeteer-0.2.1/prompeteer/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.739799 prompeteer-0.2.1/prompeteer/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.2.1/prompeteer/clients/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.740783 prompeteer-0.2.1/prompeteer/clients/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.1/prompeteer/clients/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1995 2024-05-15 07:59:19.000000 prompeteer-0.2.1/prompeteer/clients/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3073 2024-05-15 07:59:19.000000 prompeteer-0.2.1/prompeteer/clients/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1303 2024-05-15 07:59:19.000000 prompeteer-0.2.1/prompeteer/clients/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.2.1/prompeteer/clients/llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3828 2024-05-15 08:08:48.000000 prompeteer-0.2.1/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.741733 prompeteer-0.2.1/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.2.1/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.2.1/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2565 2024-05-15 07:59:19.000000 prompeteer-0.2.1/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.742360 prompeteer-0.2.1/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.2.1/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1019 2024-05-15 07:59:19.000000 prompeteer-0.2.1/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 08:11:29.743080 prompeteer-0.2.1/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     2012 2024-05-15 08:11:29.000000 prompeteer-0.2.1/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      633 2024-05-15 08:11:29.000000 prompeteer-0.2.1/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 08:11:29.000000 prompeteer-0.2.1/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 08:11:29.000000 prompeteer-0.2.1/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 08:11:29.000000 prompeteer-0.2.1/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 08:11:29.744009 prompeteer-0.2.1/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      821 2024-05-15 08:11:29.000000 prompeteer-0.2.1/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.756117 prompeteer-0.2.2/
+-rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:01:48.755635 prompeteer-0.2.2/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     2514 2024-05-15 10:01:32.000000 prompeteer-0.2.2/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.746461 prompeteer-0.2.2/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:58:26.000000 prompeteer-0.2.2/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.749367 prompeteer-0.2.2/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.2.2/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.2.2/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 08:29:05.000000 prompeteer-0.2.2/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.750766 prompeteer-0.2.2/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.2.2/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.752237 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1472 2024-05-15 08:59:54.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1781 2024-05-15 09:00:45.000000 prompeteer-0.2.2/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.753833 prompeteer-0.2.2/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1997 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 08:19:41.000000 prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1437 2024-05-15 08:31:53.000000 prompeteer-0.2.2/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.2.2/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.754569 prompeteer-0.2.2/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.2.2/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1019 2024-05-15 07:59:19.000000 prompeteer-0.2.2/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 10:01:48.755180 prompeteer-0.2.2/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     2960 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 10:01:48.000000 prompeteer-0.2.2/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 10:01:48.756197 prompeteer-0.2.2/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      837 2024-05-15 10:01:48.000000 prompeteer-0.2.2/setup.py
```

### Comparing `prompeteer-0.2.1/PKG-INFO` & `prompeteer-0.2.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: openai==1.28.1
 Requires-Dist: azure-identity
+Requires-Dist: boto3
 
 # Prompeteer
+
 ### Prompt evaluation and development environment
 
-- Use prompt Yaml config to describe your prompt templates  
-- use csv input file to inject different variables to prompt templates
-- run and evaluate *multiple* instances of a prompt (with different variables)
-- supports AzureOpenAi, AWS Bedrock
+- Define a prompt template and run it with different variables from an input.csv file
+- supports AzureOpenAi (GPT), AWS Bedrock (Anthropic Claude)
+- write output to an output.csv file (or just the console)
 
 ## installation
+
 ```shell
 pip install prompeteer
 ```
 
 ## usage
-```python
-from prompeteer import prompeteer
-prompeteer.run_prompt(prompt_config_file_path='azure_openai_test_prompt.yaml',
-                              output_csv='./output.csv',
-                              include_prompt=True,
-                              input_csv='./input.csv',
-                              row_numbers_to_process=[0, 1],
-                              destination='file')
-```
 
-here is an example of how the prompt YAML config might look like:
-```yaml
+### Azure OpenAI - GPT
+
+```yaml 
+# azure_openai_prompt.yaml
 version: 1.0
 name: my_prompt
 provider: azure
 schemaVersion: 1.0
 variables:
   - name: topic
     required: true
@@ -63,14 +58,60 @@
     - role: system
       content: "You are a helpful assistant."
     - role: user
       content: "give a short summary about {topic} in the year {year} ahd here is a summary example"
 
 ```
 
+### AWS Bedrock - Claude
+
+```yaml
+# aws_bedrock_prompt.yaml
+version: 1.0
+name: formal
+provider: aws
+schemaVersion: 1.0
+variables:
+  - name: topic
+    required: true
+  - name: year
+    required: true
+  - name: summary
+    required: true
+request:
+  model: 'anthropic.claude-3-haiku-20240307-v1:0'
+  temperature: 0.8
+  topP: 1.0
+  topK: 2
+  maxTokens: 250
+  messages:
+    - role: user
+      content: "summarize about {topic} in the year {year} use this example summary: {summary}. do it in a very formal way"
+    - role: assistant
+      content: "You are a helpful assistant."
+```
+
+```python
+from prompeteer import prompeteer
+
+prompeteer.run_prompt(prompt_config_file_path='azure_openai_prompt.yaml',
+                      output_csv='./output.csv',
+                      include_prompt=True,  # show request + response in the output
+                      input_csv='./input.csv',
+                      destination='file'  # write output to CSV file
+                      )
+
+prompeteer.run_prompt(prompt_config_file_path='aws_bedrock_prompt.yaml',
+                      include_prompt=False,  # show only request in the output
+                      input_csv='./input.csv',
+                      row_numbers_to_process=[0, 1],  # use and run only rows 0 and 1 from the input.csv 
+                      destination='console'  # write output to the console
+                      )
+```
+
 ```csv``` ("|" seperated)
 
 "topic"|"year"|"summary"
 
 "basketball"|2002|"A famous quote: ""Just do it"".
 
 "soccer"|1999|"Championship game was exciting"
```

### Comparing `prompeteer-0.2.1/README.md` & `prompeteer-0.2.2/prompeteer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+Metadata-Version: 2.1
+Name: prompeteer
+Version: 0.2.2
+Summary: Prompt Development and Evaluation tool
+Author: Yoaz Menda
+Author-email: yoazmenda@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: pyyaml
+Requires-Dist: openai==1.28.1
+Requires-Dist: azure-identity
+Requires-Dist: boto3
+
 # Prompeteer
+
 ### Prompt evaluation and development environment
 
-- Use prompt Yaml config to describe your prompt templates  
-- use csv input file to inject different variables to prompt templates
-- run and evaluate *multiple* instances of a prompt (with different variables)
-- supports AzureOpenAi, AWS Bedrock
+- Define a prompt template and run it with different variables from an input.csv file
+- supports AzureOpenAi (GPT), AWS Bedrock (Anthropic Claude)
+- write output to an output.csv file (or just the console)
 
 ## installation
+
 ```shell
 pip install prompeteer
 ```
 
 ## usage
-```python
-from prompeteer import prompeteer
-prompeteer.run_prompt(prompt_config_file_path='azure_openai_test_prompt.yaml',
-                              output_csv='./output.csv',
-                              include_prompt=True,
-                              input_csv='./input.csv',
-                              row_numbers_to_process=[0, 1],
-                              destination='file')
-```
 
-here is an example of how the prompt YAML config might look like:
-```yaml
+### Azure OpenAI - GPT
+
+```yaml 
+# azure_openai_prompt.yaml
 version: 1.0
 name: my_prompt
 provider: azure
 schemaVersion: 1.0
 variables:
   - name: topic
     required: true
@@ -49,16 +58,62 @@
     - role: system
       content: "You are a helpful assistant."
     - role: user
       content: "give a short summary about {topic} in the year {year} ahd here is a summary example"
 
 ```
 
+### AWS Bedrock - Claude
+
+```yaml
+# aws_bedrock_prompt.yaml
+version: 1.0
+name: formal
+provider: aws
+schemaVersion: 1.0
+variables:
+  - name: topic
+    required: true
+  - name: year
+    required: true
+  - name: summary
+    required: true
+request:
+  model: 'anthropic.claude-3-haiku-20240307-v1:0'
+  temperature: 0.8
+  topP: 1.0
+  topK: 2
+  maxTokens: 250
+  messages:
+    - role: user
+      content: "summarize about {topic} in the year {year} use this example summary: {summary}. do it in a very formal way"
+    - role: assistant
+      content: "You are a helpful assistant."
+```
+
+```python
+from prompeteer import prompeteer
+
+prompeteer.run_prompt(prompt_config_file_path='azure_openai_prompt.yaml',
+                      output_csv='./output.csv',
+                      include_prompt=True,  # show request + response in the output
+                      input_csv='./input.csv',
+                      destination='file'  # write output to CSV file
+                      )
+
+prompeteer.run_prompt(prompt_config_file_path='aws_bedrock_prompt.yaml',
+                      include_prompt=False,  # show only request in the output
+                      input_csv='./input.csv',
+                      row_numbers_to_process=[0, 1],  # use and run only rows 0 and 1 from the input.csv 
+                      destination='console'  # write output to the console
+                      )
+```
+
 ```csv``` ("|" seperated)
 
 "topic"|"year"|"summary"
 
 "basketball"|2002|"A famous quote: ""Just do it"".
 
 "soccer"|1999|"Championship game was exciting"
 
-```
+```
```

### Comparing `prompeteer-0.2.1/prompeteer/clients/azure_openai/azure_llm_request.py` & `prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List, Optional, Union, Dict
 
-from prompeteer.clients.llm_request import ILLMRequest
+from prompeteer.providers.llm_request import ILLMRequest
 from prompeteer.prompt.prompt import Message, Variable, DeclaredVariable
 
 
 class AzureLLMRequest(ILLMRequest):
 
     def __init__(self,
                  variables_to_inject: List[Variable],
```

### Comparing `prompeteer-0.2.1/prompeteer/clients/azure_openai/azure_openai_client.py` & `prompeteer-0.2.2/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 from typing import Dict, Any
 
 from azure.identity import DefaultAzureCredential, get_bearer_token_provider
 from openai import AzureOpenAI
 from openai.types.chat import ChatCompletion
 
-from prompeteer.clients.azure_openai.azure_llm_request import AzureLLMRequest
-from prompeteer.clients.llm_client import ILLMClient
+from prompeteer.providers.azure_openai.azure_llm_request import AzureLLMRequest
+from prompeteer.providers.llm_client import ILLMClient
 
 token_provider = get_bearer_token_provider(
     DefaultAzureCredential(), "https://cognitiveservices.azure.com/.default"
 )
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
```

### Comparing `prompeteer-0.2.1/prompeteer/clients/llm_client.py` & `prompeteer-0.2.2/prompeteer/providers/llm_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from abc import abstractmethod, ABC
 from typing import Dict
 
-from prompeteer.clients.llm_request import ILLMRequest
 from prompeteer.prompt.prompt import LLMProvider
+from prompeteer.providers.llm_request import ILLMRequest
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class ILLMClient(ABC):
     @abstractmethod
@@ -17,18 +17,20 @@
 
 clients: Dict[str, ILLMClient] = {}
 
 
 def _init_llm_client(provider: LLMProvider) -> ILLMClient:
     if provider == LLMProvider.azure:
         logger.info("Initializing Azure OpenAI LLM Client")
-        from prompeteer.clients.azure_openai.azure_openai_client import AzureOpenAiClient
+        from prompeteer.providers.azure_openai.azure_openai_client import AzureOpenAiClient
         return AzureOpenAiClient()
     elif provider == LLMProvider.aws:
-        raise NotImplementedError("implement aws!")
+        logger.info("Initializing AWS Bedrock LLM Client")
+        from prompeteer.providers.aws_bedrock.aws_bedrock_client import AwsBedrockClient
+        return AwsBedrockClient()
     else:
         logger.error(f"Unknown LLM Provider {provider}")
         raise Exception(f"Unknown LLM Provider {provider}")
 
 
 def get_llm_client(provider: LLMProvider) -> ILLMClient:
     assert provider is not None, "Provider must be provided"
```

### Comparing `prompeteer-0.2.1/prompeteer/prompeteer.py` & `prompeteer-0.2.2/prompeteer/prompeteer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Author: Yoaz Menda
 import csv
 import logging
 import os
 from datetime import datetime
 from typing import List, Literal, Tuple
 
-from prompeteer.clients.llm_request import ILLMRequest
-from prompeteer.clients.llm_client import ILLMClient, get_llm_client
+from prompeteer.providers.llm_request import ILLMRequest
+from prompeteer.providers.llm_client import ILLMClient, get_llm_client
 from prompeteer.prompt.prompt import Variable
 from prompeteer.prompt.prompt_config import load_prompt_config, PromptConfig
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 clients = {}
```

### Comparing `prompeteer-0.2.1/prompeteer/prompt/prompt.py` & `prompeteer-0.2.2/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.1/prompeteer/prompt/prompt_config.py` & `prompeteer-0.2.2/prompeteer/prompt/prompt_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import List, Dict, Any
 
 import yaml
 
-from prompeteer.clients.azure_openai.azure_llm_request import AzureLLMRequest
-from prompeteer.clients.llm_request import ILLMRequest
+from prompeteer.providers.aws_bedrock.aws_llm_request import AWSLLMRequest
+from prompeteer.providers.azure_openai.azure_llm_request import AzureLLMRequest
+from prompeteer.providers.llm_request import ILLMRequest
 from prompeteer.prompt.prompt import LLMProvider, DeclaredVariable, Variable
 from prompeteer.utils.utils import normalize_keys, create_declared_variable_list
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
@@ -22,16 +23,15 @@
         self.llm_request_config: Dict[str, Any] = llm_request_config
         self.declared_variables: List[DeclaredVariable] = create_declared_variable_list(variables)
 
     def to_llm_request(self, variables_to_inject: List[Variable]) -> ILLMRequest:
         if self.llm_provider == LLMProvider.azure:
             return AzureLLMRequest(variables_to_inject, self.declared_variables, **self.llm_request_config)
         elif self.llm_provider == LLMProvider.aws:
-            # return AwsLLMRequest(variables, **self.llm_request)
-            raise NotImplementedError("implement aws!")
+            return AWSLLMRequest(variables_to_inject, self.declared_variables, **self.llm_request_config)
         else:
             logger.error("Unsupported LLM")
             raise ValueError("Unsupported LLM")
 
 
 def load_prompt_config(prompt_config_file_path) -> PromptConfig:
     with open(prompt_config_file_path, 'r') as file:
```

### Comparing `prompeteer-0.2.1/prompeteer/utils/utils.py` & `prompeteer-0.2.2/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.1/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.2.2/prompeteer.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 prompeteer/__init__.py
 prompeteer/prompeteer.py
 prompeteer.egg-info/PKG-INFO
 prompeteer.egg-info/SOURCES.txt
 prompeteer.egg-info/dependency_links.txt
 prompeteer.egg-info/requires.txt
 prompeteer.egg-info/top_level.txt
-prompeteer/clients/__init__.py
-prompeteer/clients/llm_client.py
-prompeteer/clients/llm_request.py
-prompeteer/clients/azure_openai/__init__.py
-prompeteer/clients/azure_openai/azure_llm_request.py
-prompeteer/clients/azure_openai/azure_openai_client.py
 prompeteer/prompt/__init__.py
 prompeteer/prompt/prompt.py
 prompeteer/prompt/prompt_config.py
+prompeteer/providers/__init__.py
+prompeteer/providers/llm_client.py
+prompeteer/providers/llm_request.py
+prompeteer/providers/aws_bedrock/__init__.py
+prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+prompeteer/providers/aws_bedrock/aws_llm_request.py
+prompeteer/providers/azure_openai/__init__.py
+prompeteer/providers/azure_openai/azure_llm_request.py
+prompeteer/providers/azure_openai/azure_openai_client.py
 prompeteer/utils/__init__.py
 prompeteer/utils/utils.py
```

