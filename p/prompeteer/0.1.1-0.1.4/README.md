# Comparing `tmp/prompeteer-0.1.1.tar.gz` & `tmp/prompeteer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.1.1.tar", last modified: Wed May  8 14:15:03 2024, max compression
+gzip compressed data, was "prompeteer-0.1.4.tar", last modified: Wed May 15 07:10:52 2024, max compression
```

## Comparing `prompeteer-0.1.1.tar` & `prompeteer-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.710083 prompeteer-0.1.1/
--rw-r--r--   0 yoaz       (502) staff       (20)      447 2024-05-08 14:15:03.709756 prompeteer-0.1.1/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)       88 2024-05-06 14:09:08.000000 prompeteer-0.1.1/README.md
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.705860 prompeteer-0.1.1/clients/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-06 15:57:43.000000 prompeteer-0.1.1/clients/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)      792 2024-05-08 06:53:15.000000 prompeteer-0.1.1/clients/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      962 2024-05-08 06:53:15.000000 prompeteer-0.1.1/clients/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      192 2024-05-08 06:53:15.000000 prompeteer-0.1.1/clients/llm_client.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.707822 prompeteer-0.1.1/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)      447 2024-05-08 14:15:03.000000 prompeteer-0.1.1/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      416 2024-05-08 14:15:03.000000 prompeteer-0.1.1/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-08 14:15:03.000000 prompeteer-0.1.1/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       56 2024-05-08 14:15:03.000000 prompeteer-0.1.1/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       21 2024-05-08 14:15:03.000000 prompeteer-0.1.1/prompeteer.egg-info/top_level.txt
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.708537 prompeteer-0.1.1/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-07 11:36:48.000000 prompeteer-0.1.1/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3643 2024-05-08 14:05:53.000000 prompeteer-0.1.1/prompt/prompt_loader.py
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-08 14:15:03.710155 prompeteer-0.1.1/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      572 2024-05-08 14:14:48.000000 prompeteer-0.1.1/setup.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.708868 prompeteer-0.1.1/tests/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-06 16:03:08.000000 prompeteer-0.1.1/tests/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-08 14:15:03.709343 prompeteer-0.1.1/tests/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-07 11:36:42.000000 prompeteer-0.1.1/tests/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3244 2024-05-08 14:05:27.000000 prompeteer-0.1.1/tests/prompeteer/test_prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.608963 prompeteer-0.1.4/
+-rw-r--r--   0 yoaz       (502) staff       (20)      383 2024-05-15 07:10:52.608571 prompeteer-0.1.4/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)     1571 2024-05-15 07:07:55.000000 prompeteer-0.1.4/README.md
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.603381 prompeteer-0.1.4/clients/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-13 18:06:15.000000 prompeteer-0.1.4/clients/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.604938 prompeteer-0.1.4/clients/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-12 13:15:26.000000 prompeteer-0.1.4/clients/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1973 2024-05-13 18:19:50.000000 prompeteer-0.1.4/clients/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3051 2024-05-13 18:21:21.000000 prompeteer-0.1.4/clients/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1270 2024-05-15 06:58:31.000000 prompeteer-0.1.4/clients/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-13 11:23:51.000000 prompeteer-0.1.4/clients/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 07:10:52.608075 prompeteer-0.1.4/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)      383 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      371 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       37 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        8 2024-05-15 07:10:52.000000 prompeteer-0.1.4/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 07:10:52.609028 prompeteer-0.1.4/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      520 2024-05-15 06:57:13.000000 prompeteer-0.1.4/setup.py
```

