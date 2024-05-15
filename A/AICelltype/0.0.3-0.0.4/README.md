# Comparing `tmp/aicelltype-0.0.3.tar.gz` & `tmp/aicelltype-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicelltype-0.0.3.tar", last modified: Tue May  7 01:42:51 2024, max compression
+gzip compressed data, was "aicelltype-0.0.4.tar", last modified: Tue May 14 03:37:56 2024, max compression
```

## Comparing `aicelltype-0.0.3.tar` & `aicelltype-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 01:42:51.307331 aicelltype-0.0.3/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3600 2024-05-07 01:42:51.305329 aicelltype-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3120 2024-05-06 09:21:04.000000 aicelltype-0.0.3/README.md
--rw-rw-rw-   0        0        0      575 2024-05-07 01:42:38.000000 aicelltype-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 01:42:51.307331 aicelltype-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 01:42:51.274763 aicelltype-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 01:42:51.279773 aicelltype-0.0.3/src/AICelltype/
--rw-rw-rw-   0        0        0     7699 2024-05-07 01:41:12.000000 aicelltype-0.0.3/src/AICelltype/__init__.py
--rw-rw-rw-   0        0        0       21 2024-05-05 04:52:48.000000 aicelltype-0.0.3/src/AICelltype/aicelltype.py
-drwxrwxrwx   0        0        0        0 2024-05-07 01:42:51.305329 aicelltype-0.0.3/src/AICelltype.egg-info/
--rw-rw-rw-   0        0        0     3600 2024-05-07 01:42:51.000000 aicelltype-0.0.3/src/AICelltype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-07 01:42:51.000000 aicelltype-0.0.3/src/AICelltype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 01:42:51.000000 aicelltype-0.0.3/src/AICelltype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-07 01:42:51.000000 aicelltype-0.0.3/src/AICelltype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 01:42:51.000000 aicelltype-0.0.3/src/AICelltype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:37:56.796050 aicelltype-0.0.4/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3607 2024-05-14 03:37:56.795050 aicelltype-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3127 2024-05-12 12:16:34.000000 aicelltype-0.0.4/README.md
+-rw-rw-rw-   0        0        0      575 2024-05-14 03:37:41.000000 aicelltype-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:37:56.796050 aicelltype-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 03:37:56.759050 aicelltype-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 03:37:56.761054 aicelltype-0.0.4/src/AICelltype/
+-rw-rw-rw-   0        0        0     7737 2024-05-14 02:12:32.000000 aicelltype-0.0.4/src/AICelltype/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:37:56.794051 aicelltype-0.0.4/src/AICelltype.egg-info/
+-rw-rw-rw-   0        0        0     3607 2024-05-14 03:37:56.000000 aicelltype-0.0.4/src/AICelltype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-14 03:37:56.000000 aicelltype-0.0.4/src/AICelltype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:37:56.000000 aicelltype-0.0.4/src/AICelltype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-14 03:37:56.000000 aicelltype-0.0.4/src/AICelltype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-14 03:37:56.000000 aicelltype-0.0.4/src/AICelltype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.4/src/__init__.py
```

### Comparing `aicelltype-0.0.3/PKG-INFO` & `aicelltype-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.3
+Version: 0.0.4
 Summary: AICelltype: Annotate cell type through gpt-4 without openai key.
 Author-email: renzhg <rzgedu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In theory, tissue_name can be any type of biological tissue.  
 gene_list  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Identify one cell type for each row in gene_list.  
 model  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;One model should be chosen from `['gpt4', 'qwen-max', 'ERNIE-4.0']`.  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**gpt4**: annotate cell type through gpt4 (default);  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**qwen-max**: annotate cell type through ali qwen model, QWEN_KEY needed, refer to [link](https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key) for a key;  
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY needed, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
 # Usage
 ```
 tissue_name = 'human prostate'
 gene_lt = [
     ['KLK3', 'KRT8', 'KLK2', 'MSMB', 'ACPP', 'KLK1', 'KLK4'],
     ['MMRN1', 'FLT4', 'RELN', 'CCL21', 'PROX1', 'LYVE1'],
     ['CD69', 'IL7R', 'CD3D', 'CD3E', 'CD3G', 'ACTA2', 'MYO1B', 'ACTA2', 'ANPEP', 'PDGFRB', 'CSPG4'],
```

### Comparing `aicelltype-0.0.3/README.md` & `aicelltype-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In theory, tissue_name can be any type of biological tissue.  
 gene_list  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Identify one cell type for each row in gene_list.  
 model  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;One model should be chosen from `['gpt4', 'qwen-max', 'ERNIE-4.0']`.  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**gpt4**: annotate cell type through gpt4 (default);  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**qwen-max**: annotate cell type through ali qwen model, QWEN_KEY needed, refer to [link](https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key) for a key;  
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY needed, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
 # Usage
 ```
 tissue_name = 'human prostate'
 gene_lt = [
     ['KLK3', 'KRT8', 'KLK2', 'MSMB', 'ACPP', 'KLK1', 'KLK4'],
     ['MMRN1', 'FLT4', 'RELN', 'CCL21', 'PROX1', 'LYVE1'],
     ['CD69', 'IL7R', 'CD3D', 'CD3E', 'CD3G', 'ACTA2', 'MYO1B', 'ACTA2', 'ANPEP', 'PDGFRB', 'CSPG4'],
```

### Comparing `aicelltype-0.0.3/pyproject.toml` & `aicelltype-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "AICelltype"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name = "renzhg", email = "rzgedu@163.com" },
 ]
 dependencies = ['dashscope==1.17.1', 'requests==2.31.0']
 description = "AICelltype: Annotate cell type through gpt-4 without openai key."
 readme = "README.md"
 requires-python = ">=3.10.0"
```

### Comparing `aicelltype-0.0.3/src/AICelltype/__init__.py` & `aicelltype-0.0.4/src/AICelltype/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,18 @@
     url = 'https://gq86p6-3000.csb.app/api/create'
     response = requests.post(url, data={})
     return response.json()
 
 
 def qwen(tissue_name, gene_list):
     gene_str = '\n'.join([','.join(i) for i in gene_list])
-    input_msg = f'Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
+    input_msg = f'Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else without number before the output. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
     # print(input_msg)
     messages = [{'role': 'user', 'content': input_msg}]
-    response = Generation.call("qwen-max",
+    response = Generation.call("qwen-max-0403",
                                messages=messages,
                                result_format='message',
                               )
     if response.status_code == HTTPStatus.OK:
         # print(response)
         cellstr= response['output']['choices'][0]['message']['content']
         cell_lt = cellstr.split('\n')
```

### Comparing `aicelltype-0.0.3/src/AICelltype.egg-info/PKG-INFO` & `aicelltype-0.0.4/src/AICelltype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.3
+Version: 0.0.4
 Summary: AICelltype: Annotate cell type through gpt-4 without openai key.
 Author-email: renzhg <rzgedu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In theory, tissue_name can be any type of biological tissue.  
 gene_list  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Identify one cell type for each row in gene_list.  
 model  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;One model should be chosen from `['gpt4', 'qwen-max', 'ERNIE-4.0']`.  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**gpt4**: annotate cell type through gpt4 (default);  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**qwen-max**: annotate cell type through ali qwen model, QWEN_KEY needed, refer to [link](https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key) for a key;  
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**ERNIE-4.0**: annotate cell type through  baidu qianfan model, API_KEY and SECRET_KEY needed, refer to [link](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) for them.
 # Usage
 ```
 tissue_name = 'human prostate'
 gene_lt = [
     ['KLK3', 'KRT8', 'KLK2', 'MSMB', 'ACPP', 'KLK1', 'KLK4'],
     ['MMRN1', 'FLT4', 'RELN', 'CCL21', 'PROX1', 'LYVE1'],
     ['CD69', 'IL7R', 'CD3D', 'CD3E', 'CD3G', 'ACTA2', 'MYO1B', 'ACTA2', 'ANPEP', 'PDGFRB', 'CSPG4'],
```

