# Comparing `tmp/GrammarFlow-0.0.7.tar.gz` & `tmp/GrammarFlow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrammarFlow-0.0.7.tar", last modified: Thu Mar 21 21:40:46 2024, max compression
+gzip compressed data, was "GrammarFlow-0.0.8.tar", last modified: Thu Mar 21 21:41:56 2024, max compression
```

## Comparing `GrammarFlow-0.0.7.tar` & `GrammarFlow-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/GrammarFlow.egg-info/
--rw-r--r--   0 aksha     (1000) aksha     (1000)     8343 2024-03-21 21:40:46.000000 GrammarFlow-0.0.7/GrammarFlow.egg-info/PKG-INFO
--rw-r--r--   0 aksha     (1000) aksha     (1000)      552 2024-03-21 21:40:46.000000 GrammarFlow-0.0.7/GrammarFlow.egg-info/SOURCES.txt
--rw-r--r--   0 aksha     (1000) aksha     (1000)        1 2024-03-21 21:40:46.000000 GrammarFlow-0.0.7/GrammarFlow.egg-info/dependency_links.txt
--rw-r--r--   0 aksha     (1000) aksha     (1000)       72 2024-03-21 21:40:46.000000 GrammarFlow-0.0.7/GrammarFlow.egg-info/requires.txt
--rw-r--r--   0 aksha     (1000) aksha     (1000)       12 2024-03-21 21:40:46.000000 GrammarFlow-0.0.7/GrammarFlow.egg-info/top_level.txt
--rw-r--r--   0 aksha     (1000) aksha     (1000)     1071 2024-03-16 17:48:53.000000 GrammarFlow-0.0.7/LICENSE.txt
--rw-r--r--   0 aksha     (1000) aksha     (1000)     8343 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/PKG-INFO
--rw-r--r--   0 aksha     (1000) aksha     (1000)     7658 2024-03-21 21:36:21.000000 GrammarFlow-0.0.7/README.md
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/grammarflow/
--rw-r--r--   0 aksha     (1000) aksha     (1000)      246 2024-03-17 04:49:00.000000 GrammarFlow-0.0.7/grammarflow/__init__.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     4783 2024-03-20 21:48:13.000000 GrammarFlow-0.0.7/grammarflow/constrain.py
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/grammarflow/grammars/
--rw-r--r--   0 aksha     (1000) aksha     (1000)       90 2024-03-17 18:17:43.000000 GrammarFlow-0.0.7/grammarflow/grammars/__init__.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     5861 2024-03-17 04:49:16.000000 GrammarFlow-0.0.7/grammarflow/grammars/gnbf.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     7023 2024-03-20 23:32:38.000000 GrammarFlow-0.0.7/grammarflow/grammars/json.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     7378 2024-03-20 23:33:16.000000 GrammarFlow-0.0.7/grammarflow/grammars/toml.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     9042 2024-03-20 23:32:57.000000 GrammarFlow-0.0.7/grammarflow/grammars/xml.py
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/grammarflow/prompt/
--rw-r--r--   0 aksha     (1000) aksha     (1000)       43 2024-03-17 18:17:27.000000 GrammarFlow-0.0.7/grammarflow/prompt/__init__.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     5328 2024-03-20 03:13:21.000000 GrammarFlow-0.0.7/grammarflow/prompt/builder.py
-drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/grammarflow/tools/
--rw-r--r--   0 aksha     (1000) aksha     (1000)       65 2024-03-17 18:17:22.000000 GrammarFlow-0.0.7/grammarflow/tools/__init__.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     3583 2024-03-17 04:49:16.000000 GrammarFlow-0.0.7/grammarflow/tools/pydantic.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)     2074 2024-03-20 22:39:19.000000 GrammarFlow-0.0.7/grammarflow/tools/response.py
--rw-r--r--   0 aksha     (1000) aksha     (1000)       38 2024-03-21 21:40:46.826327 GrammarFlow-0.0.7/setup.cfg
--rw-r--r--   0 aksha     (1000) aksha     (1000)      854 2024-03-21 21:40:24.000000 GrammarFlow-0.0.7/setup.py
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/GrammarFlow.egg-info/
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     8336 2024-03-21 21:41:56.000000 GrammarFlow-0.0.8/GrammarFlow.egg-info/PKG-INFO
+-rw-r--r--   0 aksha     (1000) aksha     (1000)      552 2024-03-21 21:41:56.000000 GrammarFlow-0.0.8/GrammarFlow.egg-info/SOURCES.txt
+-rw-r--r--   0 aksha     (1000) aksha     (1000)        1 2024-03-21 21:41:56.000000 GrammarFlow-0.0.8/GrammarFlow.egg-info/dependency_links.txt
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       72 2024-03-21 21:41:56.000000 GrammarFlow-0.0.8/GrammarFlow.egg-info/requires.txt
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       12 2024-03-21 21:41:56.000000 GrammarFlow-0.0.8/GrammarFlow.egg-info/top_level.txt
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     1071 2024-03-16 17:48:53.000000 GrammarFlow-0.0.8/LICENSE.txt
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     8336 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/PKG-INFO
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     7658 2024-03-21 21:41:43.000000 GrammarFlow-0.0.8/README.md
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.736318 GrammarFlow-0.0.8/grammarflow/
+-rw-r--r--   0 aksha     (1000) aksha     (1000)      246 2024-03-17 04:49:00.000000 GrammarFlow-0.0.8/grammarflow/__init__.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     4783 2024-03-20 21:48:13.000000 GrammarFlow-0.0.8/grammarflow/constrain.py
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.736318 GrammarFlow-0.0.8/grammarflow/grammars/
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       90 2024-03-17 18:17:43.000000 GrammarFlow-0.0.8/grammarflow/grammars/__init__.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     5861 2024-03-17 04:49:16.000000 GrammarFlow-0.0.8/grammarflow/grammars/gnbf.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     7023 2024-03-20 23:32:38.000000 GrammarFlow-0.0.8/grammarflow/grammars/json.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     7378 2024-03-20 23:33:16.000000 GrammarFlow-0.0.8/grammarflow/grammars/toml.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     9042 2024-03-20 23:32:57.000000 GrammarFlow-0.0.8/grammarflow/grammars/xml.py
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/grammarflow/prompt/
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       43 2024-03-17 18:17:27.000000 GrammarFlow-0.0.8/grammarflow/prompt/__init__.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     5328 2024-03-20 03:13:21.000000 GrammarFlow-0.0.8/grammarflow/prompt/builder.py
+drwxr-xr-x   0 aksha     (1000) aksha     (1000)        0 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/grammarflow/tools/
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       65 2024-03-17 18:17:22.000000 GrammarFlow-0.0.8/grammarflow/tools/__init__.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     3583 2024-03-17 04:49:16.000000 GrammarFlow-0.0.8/grammarflow/tools/pydantic.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)     2074 2024-03-20 22:39:19.000000 GrammarFlow-0.0.8/grammarflow/tools/response.py
+-rw-r--r--   0 aksha     (1000) aksha     (1000)       38 2024-03-21 21:41:56.746318 GrammarFlow-0.0.8/setup.cfg
+-rw-r--r--   0 aksha     (1000) aksha     (1000)      847 2024-03-21 21:41:43.000000 GrammarFlow-0.0.8/setup.py
```

### Comparing `GrammarFlow-0.0.7/GrammarFlow.egg-info/PKG-INFO` & `GrammarFlow-0.0.8/GrammarFlow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: GrammarFlow
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ensuring parsability of LLM responses in agent chains
 Home-page: https://github.com/e-lab/SyntaxShaper
 Author: AkshathRaghav
 Author-email: araviki@purdue.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==1.9.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: llama-cpp-python==0.2.50
 Requires-Dist: openai==1.14.1
 
@@ -194,11 +194,11 @@
 @software{GrammarFlow,
   author = {Ravikiran, Akshath Raghav and Culurciello, Eugenio},
   title = {GrammarFlow: Powering Agent Chains by Constraining LLM Outputs},
   year = {2024},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/e-lab/GrammarFlow}}, 
-  version = {0.0.7}
+  version = {0.0.8}
 }
 ```
```

### Comparing `GrammarFlow-0.0.7/GrammarFlow.egg-info/SOURCES.txt` & `GrammarFlow-0.0.8/GrammarFlow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/LICENSE.txt` & `GrammarFlow-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/PKG-INFO` & `GrammarFlow-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: GrammarFlow
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ensuring parsability of LLM responses in agent chains
 Home-page: https://github.com/e-lab/SyntaxShaper
 Author: AkshathRaghav
 Author-email: araviki@purdue.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==1.9.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: llama-cpp-python==0.2.50
 Requires-Dist: openai==1.14.1
 
@@ -194,11 +194,11 @@
 @software{GrammarFlow,
   author = {Ravikiran, Akshath Raghav and Culurciello, Eugenio},
   title = {GrammarFlow: Powering Agent Chains by Constraining LLM Outputs},
   year = {2024},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/e-lab/GrammarFlow}}, 
-  version = {0.0.7}
+  version = {0.0.8}
 }
 ```
```

### Comparing `GrammarFlow-0.0.7/README.md` & `GrammarFlow-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -174,11 +174,11 @@
 @software{GrammarFlow,
   author = {Ravikiran, Akshath Raghav and Culurciello, Eugenio},
   title = {GrammarFlow: Powering Agent Chains by Constraining LLM Outputs},
   year = {2024},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/e-lab/GrammarFlow}}, 
-  version = {0.0.7}
+  version = {0.0.8}
 }
 ```
```

### Comparing `GrammarFlow-0.0.7/grammarflow/constrain.py` & `GrammarFlow-0.0.8/grammarflow/constrain.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/grammars/gnbf.py` & `GrammarFlow-0.0.8/grammarflow/grammars/gnbf.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/grammars/json.py` & `GrammarFlow-0.0.8/grammarflow/grammars/json.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/grammars/toml.py` & `GrammarFlow-0.0.8/grammarflow/grammars/toml.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/grammars/xml.py` & `GrammarFlow-0.0.8/grammarflow/grammars/xml.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/prompt/builder.py` & `GrammarFlow-0.0.8/grammarflow/prompt/builder.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/tools/pydantic.py` & `GrammarFlow-0.0.8/grammarflow/tools/pydantic.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/grammarflow/tools/response.py` & `GrammarFlow-0.0.8/grammarflow/tools/response.py`

 * *Files identical despite different names*

### Comparing `GrammarFlow-0.0.7/setup.py` & `GrammarFlow-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="GrammarFlow",
-    version="0.0.7",
+    version="0.0.8",
     author="AkshathRaghav",
     author_email="araviki@purdue.edu",
     description="Ensuring parsability of LLM responses in agent chains",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/e-lab/SyntaxShaper",
     packages=find_packages(),
@@ -19,9 +19,9 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8, <3.10",
+    python_requires=">=3.8",
 )
```

