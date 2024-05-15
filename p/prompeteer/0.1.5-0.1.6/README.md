# Comparing `tmp/prompeteer-0.1.5.tar.gz` & `tmp/prompeteer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.1.5.tar", last modified: Wed May 15 07:15:29 2024, max compression
+gzip compressed data, was "prompeteer-0.1.6.tar", last modified: Wed May 15 07:24:55 2024, max compression
```

## Comparing `prompeteer-0.1.5.tar` & `prompeteer-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.680342 prompeteer-0.1.5/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:15:29.679936 prompeteer-0.1.5/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.5/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.673342 prompeteer-0.1.5/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.5/clients/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.674805 prompeteer-0.1.5/clients/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.5/clients/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.5/clients/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.5/clients/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.5/clients/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.5/clients/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.679483 prompeteer-0.1.5/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      371 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        8 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:15:29.680491 prompeteer-0.1.5/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      737 2024-05-15 07:15:07.000000 prompeteer-0.1.5/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:24:55.848916 prompeteer-0.1.6/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:24:55.848182 prompeteer-0.1.6/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.6/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:24:55.847545 prompeteer-0.1.6/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:24:55.000000 prompeteer-0.1.6/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      201 2024-05-15 07:24:55.000000 prompeteer-0.1.6/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:24:55.000000 prompeteer-0.1.6/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:24:55.000000 prompeteer-0.1.6/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 07:24:55.000000 prompeteer-0.1.6/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3784 2024-05-15 06:52:18.000000 prompeteer-0.1.6/prompeteer.py
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:24:55.848981 prompeteer-0.1.6/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      770 2024-05-15 07:24:34.000000 prompeteer-0.1.6/setup.py
```

### Comparing `prompeteer-0.1.5/PKG-INFO` & `prompeteer-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.5/README.md` & `prompeteer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.5/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.1.6/prompeteer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.1.5/setup.py` & `prompeteer-0.1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.1.5',
+    version='0.1.6',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    py_modules=['prompeteer'],  # Include the top-level module
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pyyaml',
```

