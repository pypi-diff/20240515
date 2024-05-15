# Comparing `tmp/eurmlsdk-0.0.84.tar.gz` & `tmp/eurmlsdk-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.84.tar", last modified: Tue May 14 10:37:15 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.85.tar", last modified: Wed May 15 12:56:43 2024, max compression
```

## Comparing `eurmlsdk-0.0.84.tar` & `eurmlsdk-0.0.85.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 10:37:15.000000 eurmlsdk-0.0.84/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.84/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.84/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 10:37:15.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      315 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-14 10:37:14.000000 eurmlsdk-0.0.84/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-14 10:37:15.000000 eurmlsdk-0.0.84/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-14 07:43:41.000000 eurmlsdk-0.0.84/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.84/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-14 10:37:15.000000 eurmlsdk-0.0.84/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-14 10:37:15.000000 eurmlsdk-0.0.84/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4171 2024-05-14 10:36:47.000000 eurmlsdk-0.0.84/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6221 2024-05-14 07:41:05.000000 eurmlsdk-0.0.84/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 10:06:18.000000 eurmlsdk-0.0.84/eurmlsdk/yolo.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 06:27:37.000000 eurmlsdk-0.0.84/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 12:55:51.000000 eurmlsdk-0.0.85/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5341 2024-05-15 12:56:10.000000 eurmlsdk-0.0.85/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.85/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.85/eurmlsdk/yolo.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 12:55:17.000000 eurmlsdk-0.0.85/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.85/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.84/setup.py` & `eurmlsdk-0.0.85/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.84',
+    version='0.0.85',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
         'paramiko',
         'tensorflow==2.13.1',
         'tqdm',
-        'ultralytics'
+        'ultralytics',
+        'torch',
+        'timm',
+        'torchvision'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
             "eurmlsdk = eurmlsdk.__main__:main"
```

### Comparing `eurmlsdk-0.0.84/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.85/eurmlsdk/eur_sdk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from ultralytics import YOLO
 from paramiko.ssh_exception import AuthenticationException
 import paramiko
 from tqdm import tqdm
 
 class ModelNotFound(Exception):
     def __init__(self, error= "Cannot Load Model"):
         self.error = error
@@ -14,14 +13,23 @@
         total_size = os.stat(localpath).st_size
         with tqdm(total=total_size, unit='B', unit_scale=True, desc=remotepath) as pbar:
             def _callback(bytes_transferred, bytes_remaining):
                 pbar.update(bytes_transferred - pbar.n)
                 if callback:
                     callback(bytes_transferred, bytes_remaining)
             return super().put(localpath, remotepath, callback=_callback, confirm=confirm)
+    
+    # def get(self, localpath, remotepath, callback=None, confirm=True):
+    #     total_size = os.stat(remotepath).st_size
+    #     with tqdm(total=total_size, unit='B', unit_scale=True, desc=localpath) as pbar:
+    #         def _callback(bytes_transferred, bytes_remaining):
+    #             pbar.update(bytes_transferred - pbar.n)
+    #             if callback:
+    #                 callback(bytes_transferred, bytes_remaining)
+    #         return super().get(remotepath, localpath, callback=_callback, confirm=confirm)
         
 class EurBaseSDK():
     def get_model(self, filepath) ->str:
         extension = filepath.split(".")
         if extension[1] != "pt" and extension[1] != "tflite":
             print("Not supported file path")
             return ""
@@ -46,24 +54,59 @@
         except TimeoutError as err:
             print("Connection Timeout Error: ", err)
             exit(1)
         except Exception as err:
             print("Error: %s" % err)
             exit(1)
 
+    def download_from_remote(self, ssh_client, local_path, remote_path):
+        print("Downloading file from {} to {}".format(remote_path, local_path))
+        sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
+        sftp_progress_bar.get(remote_path, local_path)
+        print("File download successful")
+    
+    def download_file(self, ssh_client, local_path, remote_path):
+        try:
+            command = f"ls -t {remote_path} | grep predict"
+            stdin, stdout, stderr = ssh_client.exec_command(f'{command}')
+            op = stdout.read().decode('utf-8')
+            err = stderr.read().decode('utf-8')
+            if err != "":
+                print("Error checking the prediction results: ", err)
+                return
+            if op != "":
+                directories = op.split('\n')
+                if not len(directories) or not directories[0]:
+                    print(f"Prediction results not saved in {remote_path}")
+                    return
+                
+                sftp = ssh_client.open_sftp()
+                file = sftp.listdir_attr(remote_path + "/" + directories[0] + "/")[0].filename
+                # print("File name: %s" % file)
+                local_path = local_path + file
+                remote_path = remote_path + "/" + directories[0] + "/" + file
+                self.download_from_remote(ssh_client, local_path, remote_path)
+            else:
+                print("Error checking the prediction results: ", err)
+                return
+        except Exception as err:
+            print("Error downloading file: ", err)
+            ssh_client.close()
+            exit(1)
+
     def upload_to_remote(self, ssh_client, local_path, remote_path):
         print("Uploading file {} to {}".format(local_path, remote_path))
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
         print("File upload successful")
 
     def upload_file(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
-            print("Checking for file in {}".format(home_path))
+            # print("Checking for file in {}".format(home_path))
             sftp.stat(remote_path)
             print("File already exists")
             upload = input("Do you want to upload it again (y/n)? ")
             while upload.lower() != 'y' and upload.lower() != 'n':
                 print("Your response ('{}') was not one of the expected responses: y, n".format(upload))
                 upload = input("Do you want to upload it again (y/n)? ")
             if upload == 'y':
@@ -87,54 +130,75 @@
 
     def execute_ssh_script(self, ssh_client, command):
         try:
             if command != "pwd":
                 print("Executing script")
             stdin, stdout, stderr = ssh_client.exec_command(f'{command}')
             op = stdout.read().decode('utf-8')
-            err = stdout.read().decode('utf-8')
+            err = stderr.read().decode('utf-8')
             if op:
                 return op
             if err:
                 print(err)
                 return ""
         except Exception as err:
             print("Error Executing the script: ", err)
             exit(1)
-              
-    def deploy_model(self, local_path, hostname, username, password, modelFile):
+            
+    def deploy_pytorch_model(self, scriptFile, modelFile, hostname, username, password):
+        ssh_client = self.connect_ssh_client(hostname, username, password)
+        home_path = self.execute_ssh_script(ssh_client, 'pwd')
+        if home_path == "":
+            exit(1)
+        script_path = (f'{home_path}/{scriptFile}').replace('\n', "").strip()
+        script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile}'
+        execute_script = self.execute_ssh_script(ssh_client, script_command)
+        if execute_script != "":
+            print(execute_script)
+
+
+    def deploy_model(self, scriptFile, local_path, hostname, username, password, modelFile):
         # Establish SSH connection
         ssh_client = self.connect_ssh_client(hostname, username, password)
         home_path = self.execute_ssh_script(ssh_client, 'pwd')
         if home_path == "":
             exit(1)
         remote_model_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
-        script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
+        script_path = (f'{home_path}/{scriptFile}').replace('\n', "").strip()
+        print(f"Checking for model file in {home_path}")
         self.upload_file(ssh_client, local_path, remote_model_path, home_path)
 
         print("Choose between static dataset or live feed for prediction.")
         static = input("Static dataset (y/n)? ")
         static_path = ''
         while(static.lower() != 'y' and static.lower() != 'n'):
             print("Your response ('{}') was not one of the expected responses: y, n".format(static))
             static = input("Static dataset (y/n)? ")
         if static.lower() == 'y':
             dataset_path = input("Enter img/video path: ")
             dataset_file = dataset_path.split("/")[-1]
             remote_dataset_path = (f"{home_path}/{dataset_file}").replace('\n', "").strip()
+            print(f"Checking for dataset file in {home_path}")
             self.upload_file(ssh_client, dataset_path, remote_dataset_path, home_path)
-            feedType = 'static'
+            feedType = 'static_feed'
             static_path = remote_dataset_path
         else:
             feedType = "live_feed"
             # exit(1)
 
         if feedType == "live_feed":
             script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile} {feedType}'
         else:
             script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile} {feedType} {static_path}'
+        
         execute_script = self.execute_ssh_script(ssh_client, script_command)
         if execute_script != "":
             print(execute_script)
-        # Close SSH connection
+        
+        # download prediction results to local
+        predict_path = "/runs/detect"
+        download_to = os.getcwd() + "/"
+        download_from = (f"{home_path}{predict_path}").replace('\n', "").strip()
+        # self.download_file(ssh_client, '', os.getcwd(), home_path + '/runs/detect/')
+        self.download_file(ssh_client, download_to, download_from)
         ssh_client.close()
         exit()
```

### Comparing `eurmlsdk-0.0.84/eurmlsdk/yolo.py` & `eurmlsdk-0.0.85/eurmlsdk/yolo.py`

 * *Files identical despite different names*

