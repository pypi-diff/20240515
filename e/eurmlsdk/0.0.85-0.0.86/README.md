# Comparing `tmp/eurmlsdk-0.0.85.tar.gz` & `tmp/eurmlsdk-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.85.tar", last modified: Wed May 15 12:56:43 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.86.tar", last modified: Wed May 15 13:04:23 2024, max compression
```

## Comparing `eurmlsdk-0.0.85.tar` & `eurmlsdk-0.0.86.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 12:55:51.000000 eurmlsdk-0.0.85/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.85/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 12:56:43.000000 eurmlsdk-0.0.85/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5341 2024-05-15 12:56:10.000000 eurmlsdk-0.0.85/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.85/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.85/eurmlsdk/yolo.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 12:55:17.000000 eurmlsdk-0.0.85/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.85/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 13:04:04.000000 eurmlsdk-0.0.86/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5642 2024-05-15 13:04:09.000000 eurmlsdk-0.0.86/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.86/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.86/eurmlsdk/yolo.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 12:55:17.000000 eurmlsdk-0.0.86/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.86/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.85/setup.py` & `eurmlsdk-0.0.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.85',
+    version='0.0.86',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.85/eurmlsdk/__main__.py` & `eurmlsdk-0.0.86/eurmlsdk/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 logging.getLogger('tensorflow').setLevel(logging.ERROR)  # Suppress TensorFlow warning logs
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model type> <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
-    print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
-    print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
+    print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result using yolo model")
+    print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset using yolo model")
+    print("  pt-predict <model path>                              : Predicts the labels and saves the predicted result using Pytorch model")
+    print("  pt-validate <model path>                             : Validates the model and returns the metrics using default dataset using Pytorch model")
     print(" ")
     print("Options:")
     print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
     print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
     print(" <username>     : Remote Server username")
 
 def main():
-    commands_list = ['deploy','help','--h','predict','validate', 'py-predict', 'pt-validate']
+    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.85")
+            print("Version: 0.0.86")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
@@ -73,25 +75,25 @@
             predictData = argv[3]
             yoloSDK = ModelYolo()
             yoloSDK.predict_model(modelPath, predictData)
 
         elif command == "pt-predict":
             if argLen <3 :
                 print("Missing required arguments")
-                print("<model_path> <dataset_path>")
+                print("<model_path>")
                 exit(1)
             else:
                 model_path = argv[2]
                 pyTorchSDK = ModelPytorch()
                 pyTorchSDK.predict_model(model_path)
 
         elif command == "pt-validate":
             if argLen <3 :
                 print("Missing required arguments")
-                print("<model_path> <dataset_path>")
+                print("<model_path>")
                 exit(1)
             else:
                 model_path = argv[2]
                 pyTorchSDK = ModelPytorch()
                 pyTorchSDK.validate_model(model_path)
 
         elif command == "deploy":
```

### Comparing `eurmlsdk-0.0.85/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.86/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.85/eurmlsdk/yolo.py` & `eurmlsdk-0.0.86/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.85/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.86/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

