# Comparing `tmp/prompeteer-0.1.9.tar.gz` & `tmp/prompeteer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.1.9.tar", last modified: Wed May 15 07:51:47 2024, max compression
+gzip compressed data, was "prompeteer-0.2.0.tar", last modified: Wed May 15 07:54:59 2024, max compression
```

## Comparing `prompeteer-0.1.9.tar` & `prompeteer-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.404349 prompeteer-0.1.9/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:51:47.404041 prompeteer-0.1.9/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.9/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.397065 prompeteer-0.1.9/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.9/clients/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.398316 prompeteer-0.1.9/clients/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.9/clients/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.9/clients/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.9/clients/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.9/clients/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.9/clients/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.403607 prompeteer-0.1.9/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:51:47.000000 prompeteer-0.1.9/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      543 2024-05-15 07:51:47.000000 prompeteer-0.1.9/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:51:47.000000 prompeteer-0.1.9/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:51:47.000000 prompeteer-0.1.9/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:51:47.000000 prompeteer-0.1.9/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)     3784 2024-05-15 06:52:18.000000 prompeteer-0.1.9/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.401566 prompeteer-0.1.9/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.1.9/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.1.9/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2521 2024-05-13 18:08:59.000000 prompeteer-0.1.9/prompt/prompt_config.py
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:51:47.404525 prompeteer-0.1.9/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      810 2024-05-15 07:51:47.000000 prompeteer-0.1.9/setup.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.394801 prompeteer-0.1.9/tests/
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.402436 prompeteer-0.1.9/tests/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:31.000000 prompeteer-0.1.9/tests/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3078 2024-05-15 07:46:07.000000 prompeteer-0.1.9/tests/prompeteer/test_prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:51:47.403106 prompeteer-0.1.9/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.1.9/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1008 2024-05-15 06:52:18.000000 prompeteer-0.1.9/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.200379 prompeteer-0.2.0/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:54:59.200022 prompeteer-0.2.0/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.2.0/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.193595 prompeteer-0.2.0/clients/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.2.0/clients/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.194869 prompeteer-0.2.0/clients/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.2.0/clients/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.2.0/clients/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.2.0/clients/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.2.0/clients/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.2.0/clients/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.199559 prompeteer-0.2.0/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:54:59.000000 prompeteer-0.2.0/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      478 2024-05-15 07:54:59.000000 prompeteer-0.2.0/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:54:59.000000 prompeteer-0.2.0/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:54:59.000000 prompeteer-0.2.0/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       32 2024-05-15 07:54:59.000000 prompeteer-0.2.0/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3784 2024-05-15 06:52:18.000000 prompeteer-0.2.0/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.197843 prompeteer-0.2.0/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:02.000000 prompeteer-0.2.0/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-13 18:06:32.000000 prompeteer-0.2.0/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2521 2024-05-13 18:08:59.000000 prompeteer-0.2.0/prompt/prompt_config.py
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:54:59.200442 prompeteer-0.2.0/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      810 2024-05-15 07:54:58.000000 prompeteer-0.2.0/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:54:59.198554 prompeteer-0.2.0/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 07:42:14.000000 prompeteer-0.2.0/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1008 2024-05-15 06:52:18.000000 prompeteer-0.2.0/utils/utils.py
```

### Comparing `prompeteer-0.1.9/PKG-INFO` & `prompeteer-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.9/README.md` & `prompeteer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/clients/azure_openai/azure_llm_request.py` & `prompeteer-0.2.0/clients/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/clients/azure_openai/azure_openai_client.py` & `prompeteer-0.2.0/clients/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/clients/llm_client.py` & `prompeteer-0.2.0/clients/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.2.0/prompeteer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.9/prompeteer.py` & `prompeteer-0.2.0/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/prompt/prompt.py` & `prompeteer-0.2.0/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/prompt/prompt_config.py` & `prompeteer-0.2.0/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.9/setup.py` & `prompeteer-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.1.9',
+    version='0.2.0',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),   # Include all packages
     py_modules=['prompeteer'],
```

### Comparing `prompeteer-0.1.9/utils/utils.py` & `prompeteer-0.2.0/utils/utils.py`

 * *Files identical despite different names*

