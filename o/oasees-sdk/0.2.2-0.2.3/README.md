# Comparing `tmp/oasees_sdk-0.2.2.tar.gz` & `tmp/oasees_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.2.2.tar", max compression
+gzip compressed data, was "oasees_sdk-0.2.3.tar", max compression
```

## Comparing `oasees_sdk-0.2.2.tar` & `oasees_sdk-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.2/README.md
--rw-r--r--   0        0        0      619 2024-05-13 14:35:05.186648 oasees_sdk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    20316 2024-05-13 14:33:09.171369 oasees_sdk-0.2.2/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0     9898 2024-05-13 14:33:13.795340 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.3/README.md
+-rw-r--r--   0        0        0      619 2024-05-15 14:59:26.600138 oasees_sdk-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    21765 2024-05-15 14:53:58.345336 oasees_sdk-0.2.3/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0     9898 2024-05-15 14:57:29.720577 oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.3/PKG-INFO
```

### Comparing `oasees_sdk-0.2.2/pyproject.toml` & `oasees_sdk-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.2.2"
+version = "0.2.3"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.2.2/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.2.3/src/oasees_sdk/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,68 @@
 import requests
 import web3
 import socket
 import os
 from dotenv import load_dotenv
 import yaml
 
+ipfs_manifest_str = """apiVersion: apps/v1
+kind: Deployment
+metadata:
+  name: ipfs-kubo-deployment
+spec:
+  replicas: 1
+  selector:
+    matchLabels:
+      app: ipfs-kubo
+  template:
+    metadata:
+      labels:
+        app: ipfs-kubo
+    spec:
+      containers:
+      - name: ipfs-kubo
+        image: ipfs/kubo:latest
+        ports:
+        - containerPort: 4001
+        - containerPort: 8080
+        - containerPort: 5001
+      nodeName: k8s-quick-master
+---
+apiVersion: v1
+kind: Service
+metadata:
+  name: ipfs-kubo-service
+spec:
+  selector:
+    app: ipfs-kubo
+  type: NodePort
+  ports:
+    - name: main-tcp
+      port: 4001
+      targetPort: 4001
+      protocol: TCP
+      nodePort: 31001
+    - name: main-udp
+      port: 4001
+      targetPort: 4001
+      protocol: UDP
+      nodePort: 31002
+    - name: gateway
+      port: 8080
+      targetPort: 8080
+      protocol: TCP
+      nodePort: 31003
+    - name: api
+      port: 5002
+      targetPort: 5001
+      protocol: TCP
+      nodePort: 31005
+"""
+
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def cli(ctx):
     if not ctx.invoked_subcommand:
         bash_script = r'''
         Y='\x1b[38;2;252;220;132m'
@@ -93,15 +147,19 @@
         mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
         click.echo(result)
         curl.wait()
-        # Print the output of the 'ls' command
+
+        echo = subprocess.Popen(['echo', ipfs_manifest_str], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        result = subprocess.check_output(['kubectl','apply','-f','-'], stdin=echo.stdout)
+        click.echo(result)
+        echo.wait()
 
         with open('/home/'+getpass.getuser()+'/.kube/config', 'r') as f:
             cluster_config = yaml.safe_load(f)
 
         result = subprocess.run(['kubectl','get','nodes','-o','custom-columns=IP:.status.addresses[].address','--no-headers'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         ip = result.stdout.strip().split('\n')
 
@@ -436,8 +494,12 @@
     mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
     result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
     click.echo(result)
     curl.wait()
 
+    echo = subprocess.Popen(['echo', ipfs_manifest_str], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+    result = subprocess.check_output(['kubectl','apply','-f','-'], stdin=echo.stdout)
+    click.echo(result)
+    echo.wait()
 config_exists()
```

### Comparing `oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/sdk.py` & `oasees_sdk-0.2.3/src/oasees_sdk/oasees_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.2.2/PKG-INFO` & `oasees_sdk-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

