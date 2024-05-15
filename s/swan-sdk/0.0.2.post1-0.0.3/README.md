# Comparing `tmp/swan_sdk-0.0.2.post1.tar.gz` & `tmp/swan_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swan_sdk-0.0.2.post1.tar", last modified: Sun May  5 21:27:20 2024, max compression
+gzip compressed data, was "swan_sdk-0.0.3.tar", last modified: Wed May 15 14:54:41 2024, max compression
```

## Comparing `swan_sdk-0.0.2.post1.tar` & `swan_sdk-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.281707 swan_sdk-0.0.2.post1/
--rw-r--r--   0 zihangchen   (501) staff       (20)     1072 2024-04-27 21:10:50.000000 swan_sdk-0.0.2.post1/LICENSE
--rw-r--r--   0 zihangchen   (501) staff       (20)       32 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/MANIFEST.in
--rw-r--r--   0 zihangchen   (501) staff       (20)    10936 2024-05-05 21:27:20.281433 swan_sdk-0.0.2.post1/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)    10391 2024-05-05 21:22:01.000000 swan_sdk-0.0.2.post1/README.md
--rw-r--r--   0 zihangchen   (501) staff       (20)       38 2024-05-05 21:27:20.281756 swan_sdk-0.0.2.post1/setup.cfg
--rw-------   0 zihangchen   (501) staff       (20)     1085 2024-05-05 21:23:00.000000 swan_sdk-0.0.2.post1/setup.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.275225 swan_sdk-0.0.2.post1/swan/
--rw-r--r--   0 zihangchen   (501) staff       (20)      151 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/__init__.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.275874 swan_sdk-0.0.2.post1/swan/api/
--rw-r--r--   0 zihangchen   (501) staff       (20)       25 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/api/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)    12230 2024-05-05 13:56:09.000000 swan_sdk-0.0.2.post1/swan/api/swan_api.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     4279 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/api_client.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.277801 swan_sdk-0.0.2.post1/swan/common/
--rw-r--r--   0 zihangchen   (501) staff       (20)       27 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      922 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/constant.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      327 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/exception.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      447 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/common/file.py
--rw-r--r--   0 zihangchen   (501) staff       (20)       26 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/common/params.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     3256 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/utils.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.278228 swan_sdk-0.0.2.post1/swan/contract/
--rw-r--r--   0 zihangchen   (501) staff       (20)       29 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/__init__.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.279631 swan_sdk-0.0.2.post1/swan/contract/abi/
--rw-r--r--   0 zihangchen   (501) staff       (20)     9074 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/ClientPayment.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     9742 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/PaymentContract.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     8855 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/SwanToken.json
--rw-r--r--   0 zihangchen   (501) staff       (20)       33 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     8789 2024-05-05 21:22:01.000000 swan_sdk-0.0.2.post1/swan/contract/swan_contract.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.280131 swan_sdk-0.0.2.post1/swan/object/
--rw-r--r--   0 zihangchen   (501) staff       (20)      111 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/object/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      844 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/object/cp_config.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     1198 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/object/task.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.281098 swan_sdk-0.0.2.post1/swan_sdk.egg-info/
--rw-r--r--   0 zihangchen   (501) staff       (20)    10936 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)      676 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        1 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)       69 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/requires.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        5 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.868883 swan_sdk-0.0.3/
+-rw-r--r--   0 aaronli    (501) staff       (20)     1072 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/LICENSE
+-rw-r--r--   0 aaronli    (501) staff       (20)       32 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/MANIFEST.in
+-rw-r--r--   0 aaronli    (501) staff       (20)    10883 2024-05-15 14:54:41.868622 swan_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 aaronli    (501) staff       (20)    10345 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/README.md
+-rw-r--r--   0 aaronli    (501) staff       (20)       38 2024-05-15 14:54:41.869048 swan_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 aaronli    (501) staff       (20)     1190 2024-05-15 14:38:16.000000 swan_sdk-0.0.3/setup.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.855263 swan_sdk-0.0.3/swan/
+-rw-r--r--   0 aaronli    (501) staff       (20)      151 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/__init__.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.856191 swan_sdk-0.0.3/swan/api/
+-rw-r--r--   0 aaronli    (501) staff       (20)       25 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/api/__init__.py
+-rw-r--r--   0 aaronli    (501) staff       (20)    12230 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/api/swan_api.py
+-rw-r--r--   0 aaronli    (501) staff       (20)     4279 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/api_client.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.858061 swan_sdk-0.0.3/swan/common/
+-rw-r--r--   0 aaronli    (501) staff       (20)       27 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/__init__.py
+-rw-r--r--   0 aaronli    (501) staff       (20)      922 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/constant.py
+-rw-r--r--   0 aaronli    (501) staff       (20)      327 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/exception.py
+-rw-r--r--   0 aaronli    (501) staff       (20)      447 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/file.py
+-rw-r--r--   0 aaronli    (501) staff       (20)       26 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/params.py
+-rw-r--r--   0 aaronli    (501) staff       (20)     3256 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/common/utils.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.858828 swan_sdk-0.0.3/swan/contract/
+-rw-r--r--   0 aaronli    (501) staff       (20)       29 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/contract/__init__.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.862303 swan_sdk-0.0.3/swan/contract/abi/
+-rw-r--r--   0 aaronli    (501) staff       (20)     9074 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/contract/abi/ClientPayment.json
+-rw-r--r--   0 aaronli    (501) staff       (20)     9742 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/contract/abi/PaymentContract.json
+-rw-r--r--   0 aaronli    (501) staff       (20)     8855 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/contract/abi/SwanToken.json
+-rw-r--r--   0 aaronli    (501) staff       (20)       33 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/contract/abi/__init__.py
+-rw-r--r--   0 aaronli    (501) staff       (20)     8797 2024-05-15 13:50:37.000000 swan_sdk-0.0.3/swan/contract/swan_contract.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.864240 swan_sdk-0.0.3/swan/object/
+-rw-r--r--   0 aaronli    (501) staff       (20)      111 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/object/__init__.py
+-rw-r--r--   0 aaronli    (501) staff       (20)      844 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/object/cp_config.py
+-rw-r--r--   0 aaronli    (501) staff       (20)     1198 2024-05-15 13:43:29.000000 swan_sdk-0.0.3/swan/object/task.py
+drwxr-xr-x   0 aaronli    (501) staff       (20)        0 2024-05-15 14:54:41.868115 swan_sdk-0.0.3/swan_sdk.egg-info/
+-rw-r--r--   0 aaronli    (501) staff       (20)    10883 2024-05-15 14:54:41.000000 swan_sdk-0.0.3/swan_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 aaronli    (501) staff       (20)      676 2024-05-15 14:54:41.000000 swan_sdk-0.0.3/swan_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronli    (501) staff       (20)        1 2024-05-15 14:54:41.000000 swan_sdk-0.0.3/swan_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronli    (501) staff       (20)       69 2024-05-15 14:54:41.000000 swan_sdk-0.0.3/swan_sdk.egg-info/requires.txt
+-rw-r--r--   0 aaronli    (501) staff       (20)        5 2024-05-15 14:54:41.000000 swan_sdk-0.0.3/swan_sdk.egg-info/top_level.txt
```

### Comparing `swan_sdk-0.0.2.post1/LICENSE` & `swan_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/PKG-INFO` & `swan_sdk-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: swan-sdk
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: A python developer tool kit for Swan Orchestrator services.
-Home-page: https://github.com/swanchain/orchestrator-sdk
+Home-page: https://github.com/swanchain/python-swan-sdk
 Author: SwanCloud
 Author-email: swan.development@nbai.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,23 +67,22 @@
 pip install swan-sdk==0.0.2
 ```
 
 **Clone from GitHub:**
 
 ```bash
 git clone https://github.com/swanchain/orchestrator-sdk.git
-git checkout release/v0.0.2-1
 ```
 
 ## Use Python dotenv
 
 It is recommended to store your important personal information in configuration or as environmental variables. Python dotenv allows loading environment variables from `.env` files for easier access and better security.
 
 python-dotenv package: https://pypi.org/project/python-dotenv/ \
-Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2-1/docs/configuration.md
+Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/main/docs/configuration.md
 
 ## Quick Start Guide for Swan SDK
 
 Jump into using the SDK with this quick example:
 
 ### 1. Get Orchestrator API Key
 
@@ -144,20 +143,20 @@
 - `HardwareConfig().region` is a list of all regions this hardware is available in.
 - Retrieve individual hardware attributes:
 ```python
 print(chosen_hardware.id) # hardware id
 print(chosen_hardware.name) # hardware name
 print(chosen_hardware.description) # hardware description
 print(chosen_hardware.type) # hardware type
-print(chosen_hardware.region) # all avaliable hardware region
+print(chosen_hardware.region) # all available hardware region
 print(chosen_hardware.price) # current hardware price
-print(chosen_hardware.status) # overall hardware avaliablility
+print(chosen_hardware.status) # overall hardware availability
 ```
 
-More detials go oject documentation: https://github.com/swanchain/python-swan-sdk/blob/release/v0.0.2.post1/docs/object.md
+For more details go to project documentation: https://github.com/swanchain/python-swan-sdk/blob/main/docs/object.md
 
 Useful example: Retrieve the hardware with hardware ID 0:
 ```python
 hardwares = swan_api.get_hardware_config()
 chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0][0]
 print(chosen_hardware.to_dict())
 ```
@@ -202,15 +201,15 @@
 duration_hour = 1 # or duration you want the deployment to run
 amount = contract.estimate_payment(chosen_hardware.id, duration_hour)
 print(amount) # amount is in wei, 18 decimals
 ```
 
 ### 7. Create Task
 
-Before paying for the task. First, create a task on Orchestrator using desired task attributes.
+Before paying for the task, first, create a task on Orchestrator using desired task attributes.
 
 ```python
 import json
 
 duration_hour = 1
 # Notice that from here, you need to convert the duration to seconds
 duration = 3600*duration_hour
@@ -254,15 +253,15 @@
 
 **The `task['uuid']` will be used in the following operations.**
 
 
 
 ### 8. Submit Payment
 
-- **If you got error about insufficient balance, please make sure you have enough balance in your wallet.**
+- **If you got any error about insufficient balance, please make sure you have enough balance in your wallet.**
 - *If you have Error like "to_wei() does not exist", please make sure you have web3.py 6.15 or later.*
 
 Use `SwanContract().submit_payment()` to pay for the task. The TX hash is the receipt for the payment.
 
 ```python
 tx_hash = contract.submit_payment(task_uuid, chosen_hardware.id, duration) # duration in seconds
 ```
```

### Comparing `swan_sdk-0.0.2.post1/README.md` & `swan_sdk-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,22 @@
 pip install swan-sdk==0.0.2
 ```
 
 **Clone from GitHub:**
 
 ```bash
 git clone https://github.com/swanchain/orchestrator-sdk.git
-git checkout release/v0.0.2-1
 ```
 
 ## Use Python dotenv
 
 It is recommended to store your important personal information in configuration or as environmental variables. Python dotenv allows loading environment variables from `.env` files for easier access and better security.
 
 python-dotenv package: https://pypi.org/project/python-dotenv/ \
-Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2-1/docs/configuration.md
+Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/main/docs/configuration.md
 
 ## Quick Start Guide for Swan SDK
 
 Jump into using the SDK with this quick example:
 
 ### 1. Get Orchestrator API Key
 
@@ -127,20 +126,20 @@
 - `HardwareConfig().region` is a list of all regions this hardware is available in.
 - Retrieve individual hardware attributes:
 ```python
 print(chosen_hardware.id) # hardware id
 print(chosen_hardware.name) # hardware name
 print(chosen_hardware.description) # hardware description
 print(chosen_hardware.type) # hardware type
-print(chosen_hardware.region) # all avaliable hardware region
+print(chosen_hardware.region) # all available hardware region
 print(chosen_hardware.price) # current hardware price
-print(chosen_hardware.status) # overall hardware avaliablility
+print(chosen_hardware.status) # overall hardware availability
 ```
 
-More detials go oject documentation: https://github.com/swanchain/python-swan-sdk/blob/release/v0.0.2.post1/docs/object.md
+For more details go to project documentation: https://github.com/swanchain/python-swan-sdk/blob/main/docs/object.md
 
 Useful example: Retrieve the hardware with hardware ID 0:
 ```python
 hardwares = swan_api.get_hardware_config()
 chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0][0]
 print(chosen_hardware.to_dict())
 ```
@@ -185,15 +184,15 @@
 duration_hour = 1 # or duration you want the deployment to run
 amount = contract.estimate_payment(chosen_hardware.id, duration_hour)
 print(amount) # amount is in wei, 18 decimals
 ```
 
 ### 7. Create Task
 
-Before paying for the task. First, create a task on Orchestrator using desired task attributes.
+Before paying for the task, first, create a task on Orchestrator using desired task attributes.
 
 ```python
 import json
 
 duration_hour = 1
 # Notice that from here, you need to convert the duration to seconds
 duration = 3600*duration_hour
@@ -237,15 +236,15 @@
 
 **The `task['uuid']` will be used in the following operations.**
 
 
 
 ### 8. Submit Payment
 
-- **If you got error about insufficient balance, please make sure you have enough balance in your wallet.**
+- **If you got any error about insufficient balance, please make sure you have enough balance in your wallet.**
 - *If you have Error like "to_wei() does not exist", please make sure you have web3.py 6.15 or later.*
 
 Use `SwanContract().submit_payment()` to pay for the task. The TX hash is the receipt for the payment.
 
 ```python
 tx_hash = contract.submit_payment(task_uuid, chosen_hardware.id, duration) # duration in seconds
 ```
```

### Comparing `swan_sdk-0.0.2.post1/setup.py` & `swan_sdk-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """ SwanSDK setup code """
-
+ 
 from setuptools import setup, find_packages
-
-
+ 
+ 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-
+ 
 setup(
-    name="swan-sdk",
-    version="0.0.2.post1",
-    packages=['swan', 'swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
-    # package_data={'swan.contract.abi': ['swan/contract/abi/PaymentContract.json', 'swan/contract/abi/SwanToken.json']},
-    include_package_data=True,
-    description="A python developer tool kit for Swan Orchestrator services.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/swanchain/orchestrator-sdk",
-    author="SwanCloud",
-    author_email="swan.development@nbai.io",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-    ],
-    install_requires=[
-        "requests==2.28.1",
-        "requests-toolbelt==0.10.1",
-        "web3==6.15.1",
-        "tqdm==4.64.1"
+        name="swan-sdk",
+        version="0.0.3",
+        packages=['swan', 'swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
+        # package_data={'swan.contract.abi': ['swan/contract/abi/PaymentContract.json', 'swan/contract/abi/SwanToken.json']},
+        include_package_data=True,
+        description="A python developer tool kit for Swan Orchestrator services.",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        url="https://github.com/swanchain/python-swan-sdk",
+        author="SwanCloud",
+        author_email="swan.development@nbai.io",
+        license="MIT",
+        classifiers=[
+            "License :: OSI Approved :: MIT License",
+            "Programming Language :: Python :: 3",
         ],
-    entry_points={
-        # placeholder
-    },
-)
+        install_requires=[
+            "requests==2.28.1",
+            "requests-toolbelt==0.10.1",
+            "web3==6.15.1",
+            "tqdm==4.64.1"
+            ],
+        entry_points={
+            # placeholder
+        },
+        )
```

### Comparing `swan_sdk-0.0.2.post1/swan/api/swan_api.py` & `swan_sdk-0.0.3/swan/api/swan_api.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/api_client.py` & `swan_sdk-0.0.3/swan/api_client.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/common/constant.py` & `swan_sdk-0.0.3/swan/common/constant.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/common/utils.py` & `swan_sdk-0.0.3/swan/common/utils.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/contract/abi/ClientPayment.json` & `swan_sdk-0.0.3/swan/contract/abi/ClientPayment.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/contract/abi/PaymentContract.json` & `swan_sdk-0.0.3/swan/contract/abi/PaymentContract.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/contract/abi/SwanToken.json` & `swan_sdk-0.0.3/swan/contract/abi/SwanToken.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/contract/swan_contract.py` & `swan_sdk-0.0.3/swan/contract/swan_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             hardware_id=hardware_id, 
             duration=duration/3600  # duration in estimate_
         ))
         self._approve_payment(amount)
 
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.client_contract.functions.submitPayment(
             task_uuid, 
             hardware_id, 
             duration
@@ -110,27 +110,27 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.toHex(tx_hash)
+        return self.w3.to_hex(tx_hash)
     
 
     def _approve_payment(self, amount):
         """
         called in submit_payment
 
         Args:
             amount: amount in wei
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.token_contract.functions.approve(
             self.client_contract.address,
             amount
         ).build_transaction({
@@ -138,24 +138,24 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.toHex(tx_hash)
+        return self.w3.to_hex(tx_hash)
     
 
     def lock_revenue(self, task_id: str, hardware_id: int, duration: int):
         """
         deprecated
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.payment_contract.functions.lockRevenue(
             task_id, 
             hardware_id, 
             duration
@@ -164,23 +164,23 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.toHex(tx_hash)
+        return self.w3.to_hex(tx_hash)
     
     def _approve_swan_token(self, amount):
         """
         deprecated
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.token_contract.functions.approve(
             self.payment_contract.address, 
             amount
         ).build_transaction({
@@ -188,15 +188,15 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.toHex(tx_hash)
+        return self.w3.to_hex(tx_hash)
     
     def _get_swan_balance(self, address=None):
         """Retrieve swan token balance of any wallet from Swan token contract.
 
         Args:
             address: wallet address to check balance. If None, retrieve own token balance.
```

### Comparing `swan_sdk-0.0.2.post1/swan/object/cp_config.py` & `swan_sdk-0.0.3/swan/object/cp_config.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan/object/task.py` & `swan_sdk-0.0.3/swan/object/task.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2.post1/swan_sdk.egg-info/PKG-INFO` & `swan_sdk-0.0.3/swan_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: swan-sdk
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: A python developer tool kit for Swan Orchestrator services.
-Home-page: https://github.com/swanchain/orchestrator-sdk
+Home-page: https://github.com/swanchain/python-swan-sdk
 Author: SwanCloud
 Author-email: swan.development@nbai.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,23 +67,22 @@
 pip install swan-sdk==0.0.2
 ```
 
 **Clone from GitHub:**
 
 ```bash
 git clone https://github.com/swanchain/orchestrator-sdk.git
-git checkout release/v0.0.2-1
 ```
 
 ## Use Python dotenv
 
 It is recommended to store your important personal information in configuration or as environmental variables. Python dotenv allows loading environment variables from `.env` files for easier access and better security.
 
 python-dotenv package: https://pypi.org/project/python-dotenv/ \
-Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2-1/docs/configuration.md
+Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/main/docs/configuration.md
 
 ## Quick Start Guide for Swan SDK
 
 Jump into using the SDK with this quick example:
 
 ### 1. Get Orchestrator API Key
 
@@ -144,20 +143,20 @@
 - `HardwareConfig().region` is a list of all regions this hardware is available in.
 - Retrieve individual hardware attributes:
 ```python
 print(chosen_hardware.id) # hardware id
 print(chosen_hardware.name) # hardware name
 print(chosen_hardware.description) # hardware description
 print(chosen_hardware.type) # hardware type
-print(chosen_hardware.region) # all avaliable hardware region
+print(chosen_hardware.region) # all available hardware region
 print(chosen_hardware.price) # current hardware price
-print(chosen_hardware.status) # overall hardware avaliablility
+print(chosen_hardware.status) # overall hardware availability
 ```
 
-More detials go oject documentation: https://github.com/swanchain/python-swan-sdk/blob/release/v0.0.2.post1/docs/object.md
+For more details go to project documentation: https://github.com/swanchain/python-swan-sdk/blob/main/docs/object.md
 
 Useful example: Retrieve the hardware with hardware ID 0:
 ```python
 hardwares = swan_api.get_hardware_config()
 chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0][0]
 print(chosen_hardware.to_dict())
 ```
@@ -202,15 +201,15 @@
 duration_hour = 1 # or duration you want the deployment to run
 amount = contract.estimate_payment(chosen_hardware.id, duration_hour)
 print(amount) # amount is in wei, 18 decimals
 ```
 
 ### 7. Create Task
 
-Before paying for the task. First, create a task on Orchestrator using desired task attributes.
+Before paying for the task, first, create a task on Orchestrator using desired task attributes.
 
 ```python
 import json
 
 duration_hour = 1
 # Notice that from here, you need to convert the duration to seconds
 duration = 3600*duration_hour
@@ -254,15 +253,15 @@
 
 **The `task['uuid']` will be used in the following operations.**
 
 
 
 ### 8. Submit Payment
 
-- **If you got error about insufficient balance, please make sure you have enough balance in your wallet.**
+- **If you got any error about insufficient balance, please make sure you have enough balance in your wallet.**
 - *If you have Error like "to_wei() does not exist", please make sure you have web3.py 6.15 or later.*
 
 Use `SwanContract().submit_payment()` to pay for the task. The TX hash is the receipt for the payment.
 
 ```python
 tx_hash = contract.submit_payment(task_uuid, chosen_hardware.id, duration) # duration in seconds
 ```
```

### Comparing `swan_sdk-0.0.2.post1/swan_sdk.egg-info/SOURCES.txt` & `swan_sdk-0.0.3/swan_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

