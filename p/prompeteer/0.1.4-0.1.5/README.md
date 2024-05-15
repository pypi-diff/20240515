# Comparing `tmp/prompeteer-0.1.4.tar.gz` & `tmp/prompeteer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.1.4.tar", last modified: Wed May 15 07:10:52 2024, max compression
+gzip compressed data, was "prompeteer-0.1.5.tar", last modified: Wed May 15 07:15:29 2024, max compression
```

## Comparing `prompeteer-0.1.4.tar` & `prompeteer-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.608963 prompeteer-0.1.4/
--rw-r--r--   0 yoaz       (502) staff       (20)      383 2024-05-15 07:10:52.608571 prompeteer-0.1.4/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.4/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.603381 prompeteer-0.1.4/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.4/clients/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.604938 prompeteer-0.1.4/clients/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.4/clients/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.4/clients/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.4/clients/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.4/clients/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.4/clients/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.608075 prompeteer-0.1.4/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)      383 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      371 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        8 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:10:52.609028 prompeteer-0.1.4/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      520 2024-05-15 06:57:13.000000 prompeteer-0.1.4/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.680342 prompeteer-0.1.5/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:15:29.679936 prompeteer-0.1.5/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.5/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.673342 prompeteer-0.1.5/clients/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.5/clients/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.674805 prompeteer-0.1.5/clients/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.5/clients/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.5/clients/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.5/clients/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.5/clients/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.5/clients/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:15:29.679483 prompeteer-0.1.5/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     1996 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      371 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        8 2024-05-15 07:15:29.000000 prompeteer-0.1.5/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:15:29.680491 prompeteer-0.1.5/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      737 2024-05-15 07:15:07.000000 prompeteer-0.1.5/setup.py
```

### Comparing `prompeteer-0.1.4/README.md` & `prompeteer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.4/clients/azure_openai/azure_llm_request.py` & `prompeteer-0.1.5/clients/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.4/clients/azure_openai/azure_openai_client.py` & `prompeteer-0.1.5/clients/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.1.4/clients/llm_client.py` & `prompeteer-0.1.5/clients/llm_client.py`

 * *Files identical despite different names*

