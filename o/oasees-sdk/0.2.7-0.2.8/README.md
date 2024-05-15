# Comparing `tmp/oasees_sdk-0.2.7.tar.gz` & `tmp/oasees_sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.2.7.tar", max compression
+gzip compressed data, was "oasees_sdk-0.2.8.tar", max compression
```

## Comparing `oasees_sdk-0.2.7.tar` & `oasees_sdk-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.7/README.md
--rw-r--r--   0        0        0      619 2024-05-15 15:47:56.728076 oasees_sdk-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    21799 2024-05-15 15:13:30.532771 oasees_sdk-0.2.7/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0    10094 2024-05-15 15:47:06.936285 oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.8/README.md
+-rw-r--r--   0        0        0      619 2024-05-15 15:55:10.682256 oasees_sdk-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    21799 2024-05-15 15:13:30.532771 oasees_sdk-0.2.8/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0    10073 2024-05-15 15:54:37.450395 oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.8/PKG-INFO
```

### Comparing `oasees_sdk-0.2.7/pyproject.toml` & `oasees_sdk-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.2.7"
+version = "0.2.8"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.2.7/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.2.8/src/oasees_sdk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.7/src/oasees_sdk/oasees_sdk/sdk.py` & `oasees_sdk-0.2.8/src/oasees_sdk/oasees_sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,16 @@
     __get_config()
 
     with open('config', 'r') as f:
         kube_config = yaml.safe_load(f)
 
     master_ip = kube_config['clusters'][0]['cluster']['server']
     master_ip = master_ip.split(':')
-    print(master_ip[1][2:])
 
-    ipfs_api_url = "http://{}:31005".format(master_ip)
+    ipfs_api_url = "http://{}:31005".format(master_ip[1][2:])
     directory_path = image_folder_path
     ipfs_cid = assets_to_ipfs(ipfs_api_url, directory_path)
     print(ipfs_cid)
     app_name = directory_path.split('/')[-1].lower()
     print(app_name)
     config.load_kube_config("./config")
     # config.load_kube_config()
```

### Comparing `oasees_sdk-0.2.7/PKG-INFO` & `oasees_sdk-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.2.7
+Version: 0.2.8
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

