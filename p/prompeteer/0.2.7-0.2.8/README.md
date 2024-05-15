# Comparing `tmp/prompeteer-0.2.7.tar.gz` & `tmp/prompeteer-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.2.7.tar", last modified: Wed May 15 13:54:34 2024, max compression
+gzip compressed data, was "prompeteer-0.2.8.tar", last modified: Wed May 15 13:55:59 2024, max compression
```

## Comparing `prompeteer-0.2.7.tar` & `prompeteer-0.2.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.975456 prompeteer-0.2.7/
--rw-r--r--   0 yoaz       (502) staff       (20)     4127 2024-05-15 13:54:34.975040 prompeteer-0.2.7/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     3682 2024-05-15 13:54:01.000000 prompeteer-0.2.7/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.961914 prompeteer-0.2.7/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.967217 prompeteer-0.2.7/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.968523 prompeteer-0.2.7/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.969858 prompeteer-0.2.7/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1396 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1517 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.972892 prompeteer-0.2.7/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1734 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.973615 prompeteer-0.2.7/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3041 2024-05-15 12:42:33.000000 prompeteer-0.2.7/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:54:34.974452 prompeteer-0.2.7/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     4127 2024-05-15 13:54:34.000000 prompeteer-0.2.7/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 13:54:34.000000 prompeteer-0.2.7/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 13:54:34.000000 prompeteer-0.2.7/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 13:54:34.000000 prompeteer-0.2.7/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 13:54:34.000000 prompeteer-0.2.7/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 13:54:34.975520 prompeteer-0.2.7/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      837 2024-05-15 13:54:34.000000 prompeteer-0.2.7/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.524191 prompeteer-0.2.8/
+-rw-r--r--   0 yoaz       (502) staff       (20)     4040 2024-05-15 13:55:59.523676 prompeteer-0.2.8/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     3595 2024-05-15 13:55:47.000000 prompeteer-0.2.8/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.502980 prompeteer-0.2.8/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.507786 prompeteer-0.2.8/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.509811 prompeteer-0.2.8/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.512274 prompeteer-0.2.8/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1396 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1517 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.514626 prompeteer-0.2.8/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1734 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.519320 prompeteer-0.2.8/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3041 2024-05-15 12:42:33.000000 prompeteer-0.2.8/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:55:59.520841 prompeteer-0.2.8/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     4040 2024-05-15 13:55:59.000000 prompeteer-0.2.8/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 13:55:59.000000 prompeteer-0.2.8/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 13:55:59.000000 prompeteer-0.2.8/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 13:55:59.000000 prompeteer-0.2.8/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 13:55:59.000000 prompeteer-0.2.8/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 13:55:59.524254 prompeteer-0.2.8/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      837 2024-05-15 13:55:59.000000 prompeteer-0.2.8/setup.py
```

### Comparing `prompeteer-0.2.7/PKG-INFO` & `prompeteer-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -37,17 +37,14 @@
 ## usage
 
 ### Azure OpenAI - GPT
 
 1. Install Azure CLI and run `az login`
 2. choose an AzureOpenAI Resource to work with and specify it in the ```AZURE_OPENAI_RESOURCE_NAME``` environment
    variable.
-   for Example:
-
-```export AZURE_OPENAI_RESOURCE_NAME=gong-dev-research-ea-uk-south```
 
 3. Create your prompt configuration YAML file:
 
 ```yaml 
 # azure_openai_prompt.yaml
 version: 1.0
 name: my_prompt
```

### Comparing `prompeteer-0.2.7/README.md` & `prompeteer-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 ## usage
 
 ### Azure OpenAI - GPT
 
 1. Install Azure CLI and run `az login`
 2. choose an AzureOpenAI Resource to work with and specify it in the ```AZURE_OPENAI_RESOURCE_NAME``` environment
    variable.
-   for Example:
-
-```export AZURE_OPENAI_RESOURCE_NAME=gong-dev-research-ea-uk-south```
 
 3. Create your prompt configuration YAML file:
 
 ```yaml 
 # azure_openai_prompt.yaml
 version: 1.0
 name: my_prompt
```

### Comparing `prompeteer-0.2.7/prompeteer/prompeteer.py` & `prompeteer-0.2.8/prompeteer/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/prompt/prompt.py` & `prompeteer-0.2.8/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/prompt/prompt_config.py` & `prompeteer-0.2.8/prompeteer/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/providers/aws_bedrock/aws_bedrock_client.py` & `prompeteer-0.2.8/prompeteer/providers/aws_bedrock/aws_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/providers/aws_bedrock/aws_llm_request.py` & `prompeteer-0.2.8/prompeteer/providers/aws_bedrock/aws_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/providers/azure_openai/azure_llm_request.py` & `prompeteer-0.2.8/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.2.8/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/providers/llm_client.py` & `prompeteer-0.2.8/prompeteer/providers/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer/utils/utils.py` & `prompeteer-0.2.8/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.2.8/prompeteer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.7
+Version: 0.2.8
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -37,17 +37,14 @@
 ## usage
 
 ### Azure OpenAI - GPT
 
 1. Install Azure CLI and run `az login`
 2. choose an AzureOpenAI Resource to work with and specify it in the ```AZURE_OPENAI_RESOURCE_NAME``` environment
    variable.
-   for Example:
-
-```export AZURE_OPENAI_RESOURCE_NAME=gong-dev-research-ea-uk-south```
 
 3. Create your prompt configuration YAML file:
 
 ```yaml 
 # azure_openai_prompt.yaml
 version: 1.0
 name: my_prompt
```

### Comparing `prompeteer-0.2.7/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.2.8/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.7/setup.py` & `prompeteer-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.2.7',
+    version='0.2.8',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*']),  # Include all packages
     py_modules=['prompeteer'],
```

