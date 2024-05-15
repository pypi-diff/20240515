# Comparing `tmp/data-analytics-core-1.0.26.tar.gz` & `tmp/data_analytics_core-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-analytics-core-1.0.26.tar", last modified: Thu Mar 14 08:21:34 2024, max compression
+gzip compressed data, was "data_analytics_core-1.0.27.tar", last modified: Wed May 15 08:08:08 2024, max compression
```

## Comparing `data-analytics-core-1.0.26.tar` & `data_analytics_core-1.0.27.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/secrets_manger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/aws/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/benchmarking/display_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/benchmarking/worker_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/exceptions/da_exception_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/exceptions/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/exceptions/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/exceptions/infrastructure/aws_infrastructure_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/localstack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/localstack/boto_client_moks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/boto_client_moks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/boto_client_moks/localstack_clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.665253 data-analytics-core-1.0.26/data_analytics_core/localstack/container_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/container_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/container_manager/localstack_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/event_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/infrastructure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/data_analytics_core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/logger/da_core_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/data_analytics_core/metaclasses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/metaclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/data_analytics_core/metaclasses/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/data_analytics_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-14 08:21:34.000000 data-analytics-core-1.0.26/data_analytics_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-14 08:21:34.000000 data-analytics-core-1.0.26/data_analytics_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 08:21:34.000000 data-analytics-core-1.0.26/data_analytics_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-14 08:21:34.000000 data-analytics-core-1.0.26/data_analytics_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-14 08:21:34.000000 data-analytics-core-1.0.26/data_analytics_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-14 08:21:28.000000 data-analytics-core-1.0.26/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 08:21:34.669253 data-analytics-core-1.0.26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.794298 data_analytics_core-1.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.786298 data_analytics_core-1.0.27/data_analytics_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/aws_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/secrets_manger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/aws/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/benchmarking/display_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/benchmarking/worker_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/data_morphing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/data_morphing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/data_morphing/yaml_morphers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/exceptions/da_exception_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/exceptions/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/exceptions/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/exceptions/infrastructure/aws_infrastructure_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/localstack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/localstack/boto_client_moks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/boto_client_moks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/boto_client_moks/localstack_clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/localstack/container_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/container_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/container_manager/localstack_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/event_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/infrastructure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/logger/da_core_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core/metaclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/metaclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/data_analytics_core/metaclasses/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:08:08.790298 data_analytics_core-1.0.27/data_analytics_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 08:08:08.000000 data_analytics_core-1.0.27/data_analytics_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 08:08:08.000000 data_analytics_core-1.0.27/data_analytics_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:08:08.000000 data_analytics_core-1.0.27/data_analytics_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 08:08:08.000000 data_analytics_core-1.0.27/data_analytics_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 08:08:08.000000 data_analytics_core-1.0.27/data_analytics_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 08:08:02.000000 data_analytics_core-1.0.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:08:08.794298 data_analytics_core-1.0.27/setup.cfg
```

### Comparing `data-analytics-core-1.0.26/LICENSE` & `data_analytics_core-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `data-analytics-core-1.0.26/PKG-INFO` & `data_analytics_core-1.0.27/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-analytics-core
-Version: 1.0.26
+Version: 1.0.27
 Summary: Globally shared modules in all Data & Analytics
 Author-email: Marc Vea <marc.vea@code.seat>
 Project-URL: Homepage, https://pypi.org/project/data-analytics-core/
 Project-URL: GitHub, https://github.com/seatcode/data-analytics-core
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,9 @@
 Requires-Dist: pandas==2.0.0
 Requires-Dist: psutil==5.9.5
 Requires-Dist: Requests==2.31.0
 Requires-Dist: testcontainers==3.7.1
 Requires-Dist: docker==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: ruyaml==0.91.0
+Requires-Dist: sqlalchemy==2.0.29
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/aws/batch.py` & `data_analytics_core-1.0.27/data_analytics_core/aws/batch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """
 AWS_BatchJob Class
 Class containing all the needed AWS Service Manager actions and the client itself.
 """
-import os
-import boto3
-# custom imports
+from data_analytics_core.aws.aws_base import AmazonWebServicesInterface
 from data_analytics_core.logger.da_core_logger import da_logger
-from data_analytics_core.localstack.boto_client_moks.localstack_clients import boto3_client_localstack
 
 
-class AmazonWebServicesBatchJobs:
+class AmazonWebServicesBatchJobs(AmazonWebServicesInterface):
     def __init__(self, region_name="eu-central-1", environment_default_parameters_dict: dict = None):
-        # env aws connections generation
-        self.region_name = region_name
-        if os.getenv("LOCALSTACK_ENDPOINT_URL"):
-            self.batch_client = boto3_client_localstack(service_name="batch", region_name=self.region_name)
-        else:
-            self.batch_client = boto3.client('batch')
+        super().__call__(region_name=region_name, client="batch")
         # custom variables
         self.environment_default_parameters_dict = environment_default_parameters_dict
 
     def run_batch_with_parameters(self):
         if self.environment_default_parameters_dict:
-            response = self.batch_client.submit_job(
+            response = self.client.submit_job(
                 jobName=self.environment_default_parameters_dict.get("job_name"),
                 jobQueue=self.environment_default_parameters_dict.get("job_queue_name"),
                 jobDefinition=self.environment_default_parameters_dict.get("job_definition_name"),
                 propagateTags=True,
                 timeout={"attemptDurationSeconds": int(self.environment_default_parameters_dict.get("batch_job_timeout"))},
             )
             da_logger.info(message=f"Batch Job started succesfully with:{da_logger.new_line()}"
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/aws/glue.py` & `data_analytics_core-1.0.27/data_analytics_core/aws/glue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 """
-AWS_Glue Class
+AWS_Glue
 Class containing all the needed AWS Glue service elements, actions and the client itself.
 """
-import os
-import boto3
 from botocore.exceptions import ClientError
 # custom imports
-from data_analytics_core.localstack.boto_client_moks.localstack_clients import boto3_client_localstack
+from data_analytics_core.aws.aws_base import AmazonWebServicesInterface
 
 
-class AmazonWebServicesGlue:
+class AmazonWebServicesGlue(AmazonWebServicesInterface):
     def __init__(self, region_name="eu-central-1"):
-        # env aws connections generation
-        self.region_name = region_name
-        if os.getenv("LOCALSTACK_ENDPOINT_URL"):
-            self.glue_client = boto3_client_localstack(service_name="glue", region_name=self.region_name)
-        else:
-            self.glue_client = boto3.client('glue', region_name=self.region_name)
+        super().__init__(region_name=region_name, client="glue")
 
     def run_job(self, job_name, job_arguments):
-        self.glue_client.start_job_run(JobName=job_name, Arguments=job_arguments)
+        self.client.start_job_run(JobName=job_name, Arguments=job_arguments)
 
     def get_job_status(self, job_name) -> str:
         try:
-            job_run_id = self.glue_client.get_job_runs(JobName=job_name, MaxResults=1).get("JobRuns")[0].get("Id")
-            status_detail = self.glue_client.get_job_run(JobName=job_name, RunId=job_run_id, PredecessorsIncluded=False)
+            job_run_id = self.client.get_job_runs(JobName=job_name, MaxResults=1).get("JobRuns")[0].get("Id")
+            status_detail = self.client.get_job_run(JobName=job_name, RunId=job_run_id, PredecessorsIncluded=False)
             status = status_detail.get("JobRun").get("JobRunState")
             return status
         except ClientError as e:
             raise ClientError("boto3 client error in run_glue_job_get_status: " + e.__str__(),
                               operation_name="get_job_runs")
         except IndexError:
             return 'STOPPED'
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/aws/s3.py` & `data_analytics_core-1.0.27/data_analytics_core/aws/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,43 +8,36 @@
 import urllib.parse
 import re
 import botocore.exceptions
 import botocore.client
 import pandas as pd
 from pandas.errors import EmptyDataError
 # custom imports
+from data_analytics_core.aws.aws_base import AmazonWebServicesInterface
 from data_analytics_core.exceptions.infrastructure.aws_infrastructure_exceptions import FileDialectEncodingNotExpectedError, \
     ProviderPrefixError
 from data_analytics_core.logger.da_core_logger import da_logger
-from data_analytics_core.localstack.boto_client_moks.localstack_clients import boto3_client_localstack, boto3_resource_localstack
 
 
 # TODO: add local env discrimination logic is_aws = True if os.environ.get("AWS_DEFAULT_REGION") else False
 
 # TODO: add upload object (generic, not csv)
-class AmazonWebServicesS3:
+class AmazonWebServicesS3(AmazonWebServicesInterface):
     """
     AWS S3 service management class. Works for both, localstack and AWS environments.
     The expected partitions for events (bucket & prefixes) are the following:
     "bucket"/"data_provider"/year=yyyy/month=mm/filename.IDK
     The parameter "get_provider_prefix" can be used by any means for another kind of initial partition,
     even if the year partition is not expected afterward.
     The class can be instantiated directly over an event and working on the file/data related to this event,
     but can also work as a standalone class.
     """
     def __init__(self, eventbridge_event=None, bucket=None,
                  region_name="eu-central-1", get_provider_prefix: bool = False):
-        # env aws connections generation
-        self.region_name = region_name
-        if os.getenv("LOCALSTACK_ENDPOINT_URL"):
-            self.s3_client = boto3_client_localstack(service_name="s3", region_name=self.region_name)
-            self.s3_resource = boto3_resource_localstack(service_name="s3", region_name=self.region_name)
-        else:
-            self.s3_client = boto3.client('s3')
-            self.s3_resource = boto3.resource('s3')
+        super().__init__(region_name=region_name, client="s3", needs_resource_init=True)
         # custom variables
         self.bucket = bucket
         self.eventbridge_event = eventbridge_event
         if self.eventbridge_event:
             # from eventbridge s3 eventbridge_event
             self.key = urllib.parse.unquote_plus(self.eventbridge_event['detail']['object']['key'], encoding='utf-8')
             self.bucket = self.eventbridge_event['detail']['bucket']['name']
@@ -75,15 +68,15 @@
     def upload_dataframe(self, dataframe: pd.DataFrame, key=None, bucket=None, is_csv=True):
         if not key:
             key = self.key
         if not bucket:
             bucket = self.bucket
         if is_csv is True:
             dataframe = dataframe.to_csv(encoding="UTF-8", sep=";", decimal=".", index=False)
-            self.s3_client.upload_fileobj(io.BytesIO(bytes(dataframe, "UTF-8")), bucket, key)
+            self.client.upload_fileobj(io.BytesIO(bytes(dataframe, "UTF-8")), bucket, key)
 
     # TODO: refactor to reduce complexity but keep iteration
     def get_file_content_from_csv(self,
                                   encoding: str = None,
                                   file_body=None,
                                   separator: str = None,
                                   decimal: str = None
@@ -133,44 +126,44 @@
         # Prepare copying config
         if key and bucket:
             copy_source = {'Key': key, 'Bucket': bucket}
         else:
             copy_source = {'Key': self.key, 'Bucket': self.bucket}
         # Handling bucket and empty move file exceptions
         try:
-            self.s3_client.list_objects_v2(Bucket=self.bucket, Prefix=self.key)
+            self.client.list_objects_v2(Bucket=self.bucket, Prefix=self.key)
             # This step is used because boto3 does not raise anything if the response inside the bucket is empty
-            if self.s3_client.list_objects_v2(Bucket=self.bucket, Prefix=self.key)["KeyCount"] == 0:
+            if self.client.list_objects_v2(Bucket=self.bucket, Prefix=self.key)["KeyCount"] == 0:
                 raise da_logger.error(f"The prefix used: {self.key} was not found inside the bucket: {self.bucket}")
         except (botocore.exceptions.ClientError, botocore.client.ClientError):
             da_logger.error(f"The bucket: {self.bucket} was not found, does not exist or is misstated")
         except AttributeError:
-            self.s3_client.list_objects_v2(Bucket=bucket, Prefix=key)
+            self.client.list_objects_v2(Bucket=bucket, Prefix=key)
             # This step is used because boto3 does not raise anything if the response inside the bucket is empty
-            if self.s3_client.list_objects_v2(Bucket=bucket, Prefix=key)["KeyCount"] == 0:
+            if self.client.list_objects_v2(Bucket=bucket, Prefix=key)["KeyCount"] == 0:
                 raise da_logger.error(f"The prefix used: {key} was not found inside the bucket: {bucket}")
         # Executing possible move configs
         if new_key and new_bucket is None:
-            self.s3_client.copy_object(Bucket=copy_source.get("Bucket"), Key=new_key, CopySource=copy_source)
+            self.client.copy_object(Bucket=copy_source.get("Bucket"), Key=new_key, CopySource=copy_source)
             da_logger.info(f"The file: {key}{da_logger.new_line()}From bucket: {bucket}"
                             f"{da_logger.new_line()}Has been copied to prefix: "
                             f"{new_key}{da_logger.new_line()}And bucket: {bucket}")
         elif new_key and new_bucket:
-            self.s3_client.copy_object(Bucket=new_bucket, Key=new_key, CopySource=copy_source)
+            self.client.copy_object(Bucket=new_bucket, Key=new_key, CopySource=copy_source)
             da_logger.info(f"The file: {key}{da_logger.new_line()}From bucket: "
                             f"{bucket}{da_logger.new_line()}Has been copied to prefix: "
                             f"{new_key}{da_logger.new_line()}And bucket: {new_bucket}")
         elif new_key is None and new_bucket:
-            self.s3_client.copy_object(Bucket=new_bucket, Key=copy_source.get("Key"), CopySource=copy_source)
+            self.client.copy_object(Bucket=new_bucket, Key=copy_source.get("Key"), CopySource=copy_source)
             da_logger.info(f"The file: {self.key}{da_logger.new_line()}From bucket: "
                             f"{self.bucket}{da_logger.new_line()}Has been copied to prefix: "
                             f"{self.key}{da_logger.new_line()}And bucket: {new_bucket}")
         # Delete old file (if specified)
         if delete_origin_file:
-            self.s3_resource.Object(copy_source.get("Bucket"), copy_source.get("Key")).delete()
+            self.resource.Object(copy_source.get("Bucket"), copy_source.get("Key")).delete()
             da_logger.info("The original file has been deleted.")
 
     def extract_year_from_key(self, key=None) -> int:
         if key:
             year = re.search(r'/year=(\d{4})/', key)
         else:
             year = re.search(r'/year=(\d{4})/', self.key)
@@ -187,15 +180,15 @@
         """
         Function expected to use with another formatter on top,
         although you can be use it as is.
         :param bucket_name: S.Ex.
         :param object_key: This parameter should include the full prefix and filename.
         :return: Gets the interior data of the file, without any encoding nor parsing (plain).
         """
-        response = self.s3_client.get_object(Bucket=bucket_name, Key=object_key)
+        response = self.client.get_object(Bucket=bucket_name, Key=object_key)
         return response['Body']
 
     def get_list_of_objects(self, bucket, prefix='', suffix='') -> Optional[list]:
         """
         Function to iterate inside a specific bucket and prefix, and filter by the suffix.
         Can be used without any of the two late parameters.
         :param bucket: S. Ex.
@@ -228,15 +221,15 @@
         if isinstance(prefix, str):
             kwargs['Prefix'] = prefix
 
         while True:
 
             # The S3 API response is a large blob of metadata.
             # 'Contents' contains information about the listed objects.
-            resp = self.s3_client.list_objects_v2(**kwargs)
+            resp = self.client.list_objects_v2(**kwargs)
             if resp["KeyCount"] == 0:
                 return None
             else:
                 for obj in resp['Contents']:
                     key = obj['Key']
                     if key.startswith(prefix) and key.endswith(suffix):
                         yield key
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/aws/secrets_manger.py` & `data_analytics_core-1.0.27/data_analytics_core/aws/secrets_manger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """
-AWS_SM Class
+AWS_SM
 Class containing all the needed AWS Secrets Manager actions and the client itself.
 """
-import os
+import json
 from typing import Optional
-import boto3
 # custom imports
-from data_analytics_core.localstack.boto_client_moks.localstack_clients import boto3_client_localstack
+from data_analytics_core.aws.aws_base import AmazonWebServicesInterface
 
 
-class AmazonWebServicesSecretsManager:
+class AmazonWebServicesSecretsManager(AmazonWebServicesInterface):
     def __init__(self, region_name="eu-central-1"):
-        # env aws connections generation
-        self.region_name = region_name
-        if os.getenv("LOCALSTACK_ENDPOINT_URL"):
-            self.sm_client = boto3_client_localstack(service_name="secretsmanager", region_name=region_name)
-        else:
-            self.sm_client = boto3.client('secretsmanager', region_name=region_name)
+        super().__init__(region_name=region_name, client="secretsmanager")
 
     def extract_secret_value_as_str(self, secret_arn_or_name: str) -> Optional[str]:
-        return self.sm_client.get_secret_value(SecretId=secret_arn_or_name)["SecretString"]
+        return self.client.get_secret_value(SecretId=secret_arn_or_name)["SecretString"]
+
+    def extract_secret_value_as_dict(self, secret_arn_or_name: str) -> Optional[dict]:
+        return json.loads(self.client.get_secret_value(SecretId=secret_arn_or_name)['SecretString'])
 
     def create_secret(self, name: str, secret_value: str, description=Optional[str],
                       kms_key=Optional[str], tags=Optional[list]):
         """
         :param name:
         :param secret_value:
         :param description:
         :param kms_key: This parameter can be the ARN, ID or even the alias given to such key.
         :param tags:
         :return:
         """
-        self.sm_client.create_secret(
+        self.client.create_secret(
             Name=name,
             Description=description,
             KmsKeyId=kms_key,
             SecretString=secret_value,
             Tags=tags
         )
 
     def get_secret_arn(self, secret_name: str):
-        return self.sm_client.get_secret_value(SecretId=secret_name)["SecretString"]
+        return self.client.get_secret_value(SecretId=secret_name)["SecretString"]
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/aws/ssm.py` & `data_analytics_core-1.0.27/data_analytics_core/aws/ssm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 """
-AWS_SSM Class
+AWS_SSM
 Class containing all the needed AWS Service Manager actions and the client itself.
 """
-import os
 from typing import Optional
 import json
-import boto3
+# custom imports
+from data_analytics_core.aws.aws_base import AmazonWebServicesInterface
 
-from data_analytics_core.localstack.boto_client_moks.localstack_clients import boto3_client_localstack
 
-
-class AmazonWebServicesSSM:
+class AmazonWebServicesSSM(AmazonWebServicesInterface):
     def __init__(self, region_name="eu-central-1"):
-        # env aws connections generation
-        self.region_name = region_name
-        if os.getenv("LOCALSTACK_ENDPOINT_URL"):
-            self.ssm_client = boto3_client_localstack(service_name="ssm", region_name=region_name)
-        else:
-            self.ssm_client = boto3.client('ssm', region_name=region_name)
+        super().__init__(region_name=region_name, client="ssm")
 
     def extract_param_value_as_dict(self, param_name: str) -> Optional[dict]:
-        return eval(json.loads(json.dumps(self.ssm_client.get_parameter(Name=param_name)["Parameter"]["Value"])))
+        return eval(json.loads(json.dumps(self.client.get_parameter(Name=param_name)["Parameter"]["Value"])))
 
     def extract_param_value_as_string(self, param_name: str) -> Optional[str]:
-        return self.ssm_client.get_parameter(Name=param_name)["Parameter"]["Value"]
+        return self.client.get_parameter(Name=param_name)["Parameter"]["Value"]
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/benchmarking/display_usage.py` & `data_analytics_core-1.0.27/data_analytics_core/benchmarking/display_usage.py`

 * *Files identical despite different names*

### Comparing `data-analytics-core-1.0.26/data_analytics_core/benchmarking/worker_class.py` & `data_analytics_core-1.0.27/data_analytics_core/benchmarking/worker_class.py`

 * *Files identical despite different names*

### Comparing `data-analytics-core-1.0.26/data_analytics_core/exceptions/infrastructure/aws_infrastructure_exceptions.py` & `data_analytics_core-1.0.27/data_analytics_core/exceptions/infrastructure/aws_infrastructure_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from data_analytics_core.exceptions.da_exception_class import DataAnalyticsException
 
 #TODO: split QA and infra exceptions, and extract IGS exclusive provider exceptions
 
+
 class DataAnalyticsInfraException(DataAnalyticsException):
     def __init__(self):
         self.tech_component = "Infrastructure"
         self.code = None
         self.message = None
 
 
@@ -171,7 +172,25 @@
         self.message = message
 
 
 class RenamedColumnsAsExpectedWarning(DataAnalyticsInfraException):
     def __init__(self, message):
         self.code = "WARN.0.00.00"
         self.message = message
+
+
+class ErrorRDSClusterARNNotGiven(DataAnalyticsInfraException):
+    def __init__(self, message):
+        self.code = "ERR.0.00.00"
+        self.message = message
+
+
+class ErrorRDSClusterNotFound(DataAnalyticsInfraException):
+    def __init__(self, message):
+        self.code = "ERR.0.00.00"
+        self.message = message
+
+
+class WarningConnectionAlreadyExists(DataAnalyticsInfraException):
+    def __init__(self, message):
+        self.code = "WARN.0.00.00"
+        self.message = message
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/localstack/boto_client_moks/localstack_clients.py` & `data_analytics_core-1.0.27/data_analytics_core/localstack/boto_client_moks/localstack_clients.py`

 * *Files identical despite different names*

### Comparing `data-analytics-core-1.0.26/data_analytics_core/localstack/container_manager/localstack_container.py` & `data_analytics_core-1.0.27/data_analytics_core/localstack/container_manager/localstack_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Local Stack container manager Class
 """
 import os
 from typing import Optional
+import dotenv
 import requests
 from docker.errors import APIError
 from dotenv import dotenv_values
 # custom imports
 from testcontainers.localstack import LocalStackContainer
 from data_analytics_core.logger.da_core_logger import da_logger
 from data_analytics_core.localstack.set_up.infrastructure import LocalstackCommonInfrastructure
@@ -44,14 +45,16 @@
                 LocalStackContainer(f"localstack/localstack-pro:{self.pro_image_version}").with_env("DATA_DIR",
                                                                                             "/tmp/set_up/data").
                 with_exposed_ports(4566).with_name(ls_docker_container_name)
             )
         self.project_name = project_name
         if path_to_env_file:
             self.local_stack_container.env.update(dict(dotenv_values(path_to_env_file)))
+            # This will make sure any env you are on gets the same vars
+            dotenv.load_dotenv(path_to_env_file)
         self._start()
         self.s3_port = self.local_stack_container.get_exposed_port(4566)
         self._generate_internal_env_vars()
         self.generate_env_vars_from_dict_list(list_of_environment_variables)
         self.common_infra = LocalstackCommonInfrastructure(s3_port=self.s3_port)
         da_logger.info("Common infra emulated")
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/event_factory.py` & `data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/event_factory.py`

 * *Files identical despite different names*

### Comparing `data-analytics-core-1.0.26/data_analytics_core/localstack/set_up/infrastructure.py` & `data_analytics_core-1.0.27/data_analytics_core/localstack/set_up/infrastructure.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,21 @@
                                     role_arn: str = None, tags: list[dict] = None):
         self.aws_cf.create_resource(
             resource_name=resource_name,
             path_to_file=path_to_file,
             role_arn=role_arn,
             tags=tags
         )
-        da_logger.info(f"Creating new stack including {resource_name}.")
 
     def create_s3_buckets(self, s3_bucket_list: list[str]):
         for s3_name in s3_bucket_list:
-            self.aws_s3.s3_client.create_bucket(Bucket=s3_name)
+            self.aws_s3.s3_client.create_bucket(
+                Bucket=s3_name,
+                CreateBucketConfiguration={'LocationConstraint': self.aws_s3.region_name}
+            )
             da_logger.info(f"Created new bucket called: {s3_name}")
 
     def get_s3_file_as_output(self,
                               aws_s3: AmazonWebServicesS3,
                               bucket=None,
                               prefix: str = '',
                               suffix: str = ''):
@@ -134,14 +136,15 @@
 
     def _flattener(self, flat_list, nested_lists):
         for subelement in nested_lists:
             if isinstance(subelement, list):
                 self._flattener(flat_list, subelement)
             else:
                 flat_list.append(subelement)
+
     def _boto_clients_activation(self, generic_boto_clients_activation: bool = True):
         if generic_boto_clients_activation:
             self.aws_s3 = AmazonWebServicesS3()
             self.aws_glue = AmazonWebServicesGlue()
             self.aws_secrets_manager = AmazonWebServicesSecretsManager()
             self.aws_ssm = AmazonWebServicesSSM()
             self.aws_batch = AmazonWebServicesBatchJobs()
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core/logger/da_core_logger.py` & `data_analytics_core-1.0.27/data_analytics_core/logger/da_core_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,38 +6,44 @@
 
 
 class DataAnalyticsLogger(metaclass=SingletonMetaClass):
     """
     Logger designed to work in any environment (Local, Localstack & AWS) and logging level.
     Includes singleton Python metaclass system and 4  different levels of messaging, with different colors
     (using colorlog package) to output the messages.
+    Levels determined by logging as integers (as in their library):
+    CRITICAL = 50
+    FATAL = CRITICAL
+    ERROR = 40
+    WARNING = 30
+    WARN = WARNING
+    INFO = 20
+    DEBUG = 10
+    NOTSET = 0
     """
-    def __init__(self, project=None, tech_component=None):
+    def __init__(self, project=None, tech_component=None, level: int = colorlog.INFO):
         self.project = project
         self.tech_component = tech_component
         self.code = None
         self.logger = self._logger_config()
+        self.logger.setLevel(level)
 
     def error(self, message: str, code: str = None):
-        self.logger.setLevel(colorlog.ERROR)
         output = self.output(logger_type="Error", message=message, code=code)
         self.logger.error(output)
 
     def warning(self, message: str, code: str = None):
-        self.logger.setLevel(colorlog.WARNING)
         output = self.output(logger_type="Warning", message=message, code=code)
         self.logger.warning(output)
 
     def debug(self, message: str, code: str = None):
-        self.logger.setLevel(colorlog.DEBUG)
         output = self.output(logger_type="Debug", message=message, code=code)
         self.logger.debug(output)
 
     def info(self, message: str, code: str = None):
-        self.logger.setLevel(colorlog.INFO)
         output = self.output(logger_type="Info", message=message, code=code)
         self.logger.info(output)
 
     def output(self, logger_type: str, message: str, code: str):
         """Message with code and value."""
         output = f"{logger_type} in {self.project}:{self.tech_component};"
         if code:
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core.egg-info/PKG-INFO` & `data_analytics_core-1.0.27/data_analytics_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-analytics-core
-Version: 1.0.26
+Version: 1.0.27
 Summary: Globally shared modules in all Data & Analytics
 Author-email: Marc Vea <marc.vea@code.seat>
 Project-URL: Homepage, https://pypi.org/project/data-analytics-core/
 Project-URL: GitHub, https://github.com/seatcode/data-analytics-core
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,9 @@
 Requires-Dist: pandas==2.0.0
 Requires-Dist: psutil==5.9.5
 Requires-Dist: Requests==2.31.0
 Requires-Dist: testcontainers==3.7.1
 Requires-Dist: docker==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pyyaml==6.0.1
+Requires-Dist: ruyaml==0.91.0
+Requires-Dist: sqlalchemy==2.0.29
```

### Comparing `data-analytics-core-1.0.26/data_analytics_core.egg-info/SOURCES.txt` & `data_analytics_core-1.0.27/data_analytics_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 data_analytics_core/__init__.py
 data_analytics_core.egg-info/PKG-INFO
 data_analytics_core.egg-info/SOURCES.txt
 data_analytics_core.egg-info/dependency_links.txt
 data_analytics_core.egg-info/requires.txt
 data_analytics_core.egg-info/top_level.txt
 data_analytics_core/aws/__init__.py
+data_analytics_core/aws/aws_base.py
 data_analytics_core/aws/batch.py
 data_analytics_core/aws/cf.py
 data_analytics_core/aws/glue.py
+data_analytics_core/aws/rds.py
 data_analytics_core/aws/s3.py
 data_analytics_core/aws/secrets_manger.py
 data_analytics_core/aws/ssm.py
 data_analytics_core/benchmarking/__init__.py
 data_analytics_core/benchmarking/display_usage.py
 data_analytics_core/benchmarking/worker_class.py
+data_analytics_core/data_morphing/__init__.py
+data_analytics_core/data_morphing/yaml_morphers.py
 data_analytics_core/exceptions/__init__.py
 data_analytics_core/exceptions/da_exception_class.py
 data_analytics_core/exceptions/infrastructure/__init__.py
 data_analytics_core/exceptions/infrastructure/aws_infrastructure_exceptions.py
 data_analytics_core/localstack/__init__.py
 data_analytics_core/localstack/boto_client_moks/__init__.py
 data_analytics_core/localstack/boto_client_moks/localstack_clients.py
```

### Comparing `data-analytics-core-1.0.26/pyproject.toml` & `data_analytics_core-1.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "data-analytics-core"
-version = "1.0.26"
+version = "1.0.27"
 authors = [
   { name="Marc Vea", email="marc.vea@code.seat" },
 ]
 description = "Globally shared modules in all Data & Analytics\nTo ensure a layer-able version, install with the '--no-deps' flag and make sure the requirements are met in the rest of the layers used or in the same you are mounting this package in."
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = ["dependencies"]
```

