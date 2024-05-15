# Comparing `tmp/prompeteer-0.2.9.tar.gz` & `tmp/prompeteer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.2.9.tar", last modified: Wed May 15 13:59:15 2024, max compression
+gzip compressed data, was "prompeteer-0.3.0.tar", last modified: Wed May 15 15:21:45 2024, max compression
```

## Comparing `prompeteer-0.2.9.tar` & `prompeteer-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.978981 prompeteer-0.2.9/
--rw-r--r--   0 yoaz       (502) staff       (20)     3859 2024-05-15 13:59:15.977891 prompeteer-0.2.9/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     3682 2024-05-15 13:57:29.000000 prompeteer-0.2.9/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.961616 prompeteer-0.2.9/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.967177 prompeteer-0.2.9/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.969759 prompeteer-0.2.9/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.972138 prompeteer-0.2.9/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1396 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1517 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.973877 prompeteer-0.2.9/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1734 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.975654 prompeteer-0.2.9/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3041 2024-05-15 12:42:33.000000 prompeteer-0.2.9/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 13:59:15.977088 prompeteer-0.2.9/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     3859 2024-05-15 13:59:15.000000 prompeteer-0.2.9/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 13:59:15.000000 prompeteer-0.2.9/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 13:59:15.000000 prompeteer-0.2.9/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       43 2024-05-15 13:59:15.000000 prompeteer-0.2.9/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 13:59:15.000000 prompeteer-0.2.9/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 13:59:15.979276 prompeteer-0.2.9/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      844 2024-05-15 13:59:15.000000 prompeteer-0.2.9/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.005557 prompeteer-0.3.0/
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-15 15:21:45.005261 prompeteer-0.3.0/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     3682 2024-05-15 13:57:29.000000 prompeteer-0.3.0/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:44.998097 prompeteer-0.3.0/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 14:32:25.000000 prompeteer-0.3.0/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.000724 prompeteer-0.3.0/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.001716 prompeteer-0.3.0/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.002858 prompeteer-0.3.0/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1955 2024-05-15 15:18:52.000000 prompeteer-0.3.0/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1517 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.003742 prompeteer-0.3.0/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1734 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.004245 prompeteer-0.3.0/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3041 2024-05-15 12:42:33.000000 prompeteer-0.3.0/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:21:45.004845 prompeteer-0.3.0/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-15 15:21:44.000000 prompeteer-0.3.0/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      797 2024-05-15 15:21:44.000000 prompeteer-0.3.0/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 15:21:44.000000 prompeteer-0.3.0/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-15 15:21:44.000000 prompeteer-0.3.0/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 15:21:44.000000 prompeteer-0.3.0/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 15:21:45.005618 prompeteer-0.3.0/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      864 2024-05-15 15:21:44.000000 prompeteer-0.3.0/setup.py
```

### Comparing `prompeteer-0.2.9/PKG-INFO` & `prompeteer-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.9
+Version: 0.3.0
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
 Requires-Dist: boto3
+Requires-Dist: tenacity
 
 # Prompeteer
 
 ## **[pypi.org/prompeteer](https://pypi.org/project/prompeteer/)**
 
 ### Prompt evaluation and development environment
```

### Comparing `prompeteer-0.2.9/README.md` & `prompeteer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/prompeteer.py` & `prompeteer-0.3.0/prompeteer/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/prompt/prompt.py` & `prompeteer-0.3.0/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/prompt/prompt_config.py` & `prompeteer-0.3.0/prompeteer/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/providers/aws_bedrock/aws_llm_request.py` & `prompeteer-0.3.0/prompeteer/providers/aws_bedrock/aws_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/providers/azure_openai/azure_llm_request.py` & `prompeteer-0.3.0/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.3.0/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/providers/llm_client.py` & `prompeteer-0.3.0/prompeteer/providers/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer/utils/utils.py` & `prompeteer-0.3.0/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.3.0/prompeteer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.2.9
+Version: 0.3.0
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
 Requires-Dist: boto3
+Requires-Dist: tenacity
 
 # Prompeteer
 
 ## **[pypi.org/prompeteer](https://pypi.org/project/prompeteer/)**
 
 ### Prompt evaluation and development environment
```

### Comparing `prompeteer-0.2.9/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.3.0/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.2.9/setup.py` & `prompeteer-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("public_README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.2.9',
+    version='0.3.0',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*']),  # Include all packages
     py_modules=['prompeteer'],
@@ -19,10 +19,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pyyaml',
         'openai == 1.28.1',
         'azure-identity',
-        'boto3'
+        'boto3',
+        'tenacity'
     ],
 )
```

