# Comparing `tmp/genflowly_lambda_utils-0.0.8.tar.gz` & `tmp/genflowly_lambda_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly_lambda_utils-0.0.8.tar", last modified: Sun Apr 14 22:13:46 2024, max compression
+gzip compressed data, was "genflowly_lambda_utils-0.0.9.tar", last modified: Sun Apr 21 20:35:29 2024, max compression
```

## Comparing `genflowly_lambda_utils-0.0.8.tar` & `genflowly_lambda_utils-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:13:46.835618 genflowly_lambda_utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 22:13:46.835618 genflowly_lambda_utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:13:46.835618 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 22:13:46.000000 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 22:13:46.000000 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:13:46.000000 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 22:13:46.000000 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:13:46.000000 genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:13:46.835618 genflowly_lambda_utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:13:46.835618 genflowly_lambda_utils-0.0.8/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/hashing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 22:13:16.000000 genflowly_lambda_utils-0.0.8/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:35:29.700437 genflowly_lambda_utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-21 20:35:29.700437 genflowly_lambda_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:35:29.700437 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-21 20:35:29.000000 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 20:35:29.000000 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:35:29.000000 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 20:35:29.000000 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 20:35:29.000000 genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:35:29.700437 genflowly_lambda_utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:35:29.700437 genflowly_lambda_utils-0.0.9/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/hashing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-21 20:35:03.000000 genflowly_lambda_utils-0.0.9/utils/jwt_utils.py
```

### Comparing `genflowly_lambda_utils-0.0.8/PKG-INFO` & `genflowly_lambda_utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.8/README.md` & `genflowly_lambda_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.8/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly_lambda_utils-0.0.9/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.8/setup.py` & `genflowly_lambda_utils-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly_lambda_utils-0.0.8/utils/aws_dynamodb_utils.py` & `genflowly_lambda_utils-0.0.9/utils/aws_dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.8/utils/aws_sns_utils.py` & `genflowly_lambda_utils-0.0.9/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.8/utils/aws_step_functions_utils.py` & `genflowly_lambda_utils-0.0.9/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.8/utils/jwt_utils.py` & `genflowly_lambda_utils-0.0.9/utils/jwt_utils.py`

 * *Files identical despite different names*

