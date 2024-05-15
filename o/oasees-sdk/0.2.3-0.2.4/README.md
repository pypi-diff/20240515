# Comparing `tmp/oasees_sdk-0.2.3.tar.gz` & `tmp/oasees_sdk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.2.3.tar", max compression
+gzip compressed data, was "oasees_sdk-0.2.4.tar", max compression
```

## Comparing `oasees_sdk-0.2.3.tar` & `oasees_sdk-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.3/README.md
--rw-r--r--   0        0        0      619 2024-05-15 14:59:26.600138 oasees_sdk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    21765 2024-05-15 14:53:58.345336 oasees_sdk-0.2.3/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0     9898 2024-05-15 14:57:29.720577 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.4/README.md
+-rw-r--r--   0        0        0      619 2024-05-15 15:13:43.540718 oasees_sdk-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    21799 2024-05-15 15:13:30.532771 oasees_sdk-0.2.4/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0     9898 2024-05-15 14:57:29.720577 oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.4/PKG-INFO
```

### Comparing `oasees_sdk-0.2.3/pyproject.toml` & `oasees_sdk-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.2.3"
+version = "0.2.4"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.2.3/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.2.4/src/oasees_sdk/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
       containers:
       - name: ipfs-kubo
         image: ipfs/kubo:latest
         ports:
         - containerPort: 4001
         - containerPort: 8080
         - containerPort: 5001
-      nodeName: k8s-quick-master
+      nodeSelector:
+        node-role.kubernetes.io/master: "true"
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: ipfs-kubo-service
 spec:
   selector:
```

### Comparing `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/sdk.py` & `oasees_sdk-0.2.4/src/oasees_sdk/oasees_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.3/PKG-INFO` & `oasees_sdk-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.2.3
+Version: 0.2.4
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

