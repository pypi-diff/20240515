# Comparing `tmp/prompeteer-0.1.7.tar.gz` & `tmp/prompeteer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.1.7.tar", last modified: Wed May 15 07:27:56 2024, max compression
+gzip compressed data, was "prompeteer-0.1.8.tar", last modified: Wed May 15 07:44:45 2024, max compression
```

## Comparing `prompeteer-0.1.7.tar` & `prompeteer-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:27:56.762771 prompeteer-0.1.7/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:27:56.762370 prompeteer-0.1.7/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.7/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:27:56.757832 prompeteer-0.1.7/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.7/clients/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:27:56.759387 prompeteer-0.1.7/clients/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.7/clients/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.7/clients/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.7/clients/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.7/clients/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.7/clients/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:27:56.761869 prompeteer-0.1.7/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:27:56.000000 prompeteer-0.1.7/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      385 2024-05-15 07:27:56.000000 prompeteer-0.1.7/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:27:56.000000 prompeteer-0.1.7/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:27:56.000000 prompeteer-0.1.7/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       19 2024-05-15 07:27:56.000000 prompeteer-0.1.7/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)     3784 2024-05-15 06:52:18.000000 prompeteer-0.1.7/prompeteer.py
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:27:56.762839 prompeteer-0.1.7/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      825 2024-05-15 07:27:28.000000 prompeteer-0.1.7/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.811111 prompeteer-0.1.8/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:44:45.810752 prompeteer-0.1.8/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.8/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.806391 prompeteer-0.1.8/clients/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.8/clients/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.807323 prompeteer-0.1.8/clients/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.8/clients/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.8/clients/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.8/clients/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.8/clients/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.8/clients/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.810374 prompeteer-0.1.8/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:44:45.000000 prompeteer-0.1.8/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      478 2024-05-15 07:44:45.000000 prompeteer-0.1.8/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:44:45.000000 prompeteer-0.1.8/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:44:45.000000 prompeteer-0.1.8/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       32 2024-05-15 07:44:45.000000 prompeteer-0.1.8/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3784 2024-05-15 06:52:18.000000 prompeteer-0.1.8/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.809603 prompeteer-0.1.8/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.1.8/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.1.8/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2521 2024-05-13 18:08:59.000000 prompeteer-0.1.8/prompt/prompt_config.py
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:44:45.811173 prompeteer-0.1.8/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      793 2024-05-15 07:43:24.000000 prompeteer-0.1.8/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:44:45.810021 prompeteer-0.1.8/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.1.8/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1008 2024-05-15 06:52:18.000000 prompeteer-0.1.8/utils/utils.py
```

### Comparing `prompeteer-0.1.7/PKG-INFO` & `prompeteer-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.7/README.md` & `prompeteer-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.7/clients/azure_openai/azure_llm_request.py` & `prompeteer-0.1.8/clients/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.7/clients/azure_openai/azure_openai_client.py` & `prompeteer-0.1.8/clients/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.7/clients/llm_client.py` & `prompeteer-0.1.8/clients/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.7/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.1.8/prompeteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.7/prompeteer.py` & `prompeteer-0.1.8/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.7/setup.py` & `prompeteer-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.1.7',
+    version='0.1.8',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    py_modules=['prompeteer'],  # Include the top-level module
     packages=find_packages(),   # Include all packages
+    py_modules=['prompeteer'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pyyaml',
```

