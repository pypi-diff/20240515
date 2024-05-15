# Comparing `tmp/maat-machine-0.1.0.tar.gz` & `tmp/maat-machine-0.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maat-machine-0.1.0.tar", max compression
+gzip compressed data, was "maat-machine-0.1.1b1.tar", max compression
```

## Comparing `maat-machine-0.1.0.tar` & `maat-machine-0.1.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2024-05-13 12:20:29.203050 maat-machine-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/__init__.py
--rw-r--r--   0        0        0      661 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/archive.py
--rw-r--r--   0        0        0     3792 2024-05-14 18:11:36.200710 maat-machine-0.1.0/maat_machine/data_images.py
--rw-r--r--   0        0        0     6844 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/directory_tree.py
--rw-r--r--   0        0        0     2265 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/filesystem.py
--rw-r--r--   0        0        0       84 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/logging.py
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/model/__init__.py
--rw-r--r--   0        0        0    11420 2024-05-14 18:18:04.316730 maat-machine-0.1.0/maat_machine/model/cv.py
--rw-r--r--   0        0        0      761 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/model/utils.py
--rw-r--r--   0        0        0      513 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/packages.py
--rw-r--r--   0        0        0      111 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/plots.py
--rw-r--r--   0        0        0     2189 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/pprint.py
--rw-r--r--   0        0        0       76 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/time.py
--rw-r--r--   0        0        0     1858 2024-05-13 12:20:29.219736 maat-machine-0.1.0/maat_machine/utils.py
--rw-r--r--   0        0        0      668 2024-05-14 18:19:32.880760 maat-machine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 maat-machine-0.1.0/setup.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 maat-machine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-13 12:20:29.203050 maat-machine-0.1.1b1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/archive.py
+-rw-r--r--   0        0        0     3792 2024-05-14 18:11:36.200710 maat-machine-0.1.1b1/maat_machine/data_images.py
+-rw-r--r--   0        0        0     6844 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/directory_tree.py
+-rw-r--r--   0        0        0     2265 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/filesystem.py
+-rw-r--r--   0        0        0       84 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/logging.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/model/__init__.py
+-rw-r--r--   0        0        0    11676 2024-05-15 16:08:33.642153 maat-machine-0.1.1b1/maat_machine/model/cv.py
+-rw-r--r--   0        0        0      761 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/model/utils.py
+-rw-r--r--   0        0        0      513 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/packages.py
+-rw-r--r--   0        0        0      111 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/plots.py
+-rw-r--r--   0        0        0     2189 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/pprint.py
+-rw-r--r--   0        0        0       76 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/time.py
+-rw-r--r--   0        0        0     1858 2024-05-13 12:20:29.219736 maat-machine-0.1.1b1/maat_machine/utils.py
+-rw-r--r--   0        0        0      670 2024-05-15 16:13:04.983426 maat-machine-0.1.1b1/pyproject.toml
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 maat-machine-0.1.1b1/setup.py
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 maat-machine-0.1.1b1/PKG-INFO
```

### Comparing `maat-machine-0.1.0/LICENSE` & `maat-machine-0.1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/archive.py` & `maat-machine-0.1.1b1/maat_machine/archive.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/data_images.py` & `maat-machine-0.1.1b1/maat_machine/data_images.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/directory_tree.py` & `maat-machine-0.1.1b1/maat_machine/directory_tree.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/filesystem.py` & `maat-machine-0.1.1b1/maat_machine/filesystem.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/model/cv.py` & `maat-machine-0.1.1b1/maat_machine/model/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import zipfile
 
 import json
 import pandas as pd
 import numpy as np
 import tensorflow as tf
 from tensorflow import keras as ktf
+import keras
 from keras import models as mktf
 from keras import layers as lktf
 from keras import optimizers as oktf
 from keras import preprocessing as ppktf
 from keras import utils as uktf
 from keras import losses as lsktf
 import tensorflow.keras.preprocessing.image as tkpi
@@ -66,15 +67,15 @@
         self.dense_activation = dense_activation
         self.dense_activation_parameter = dense_activation_parameter
         self.dense_dropout = dense_dropout
 
         self.model = None
 
     def create_cnn_model(self):
-        model = ktf.Sequential()
+        model = keras.Sequential()
         model.add(lktf.Input(shape=self.input_shape, name='input'))
 
         for i, conv_layer_config in list(enumerate(self.conv_layer_array)):
             conv_filters_i, conv_kernel_i, layers_i = conv_layer_config
             assert 'c' in layers_i
 #             if i == 0:
 #                 model.add(lktf.Conv2D(filters=conv_filters_i, kernel_size=(1, 1), padding='same'))
@@ -273,7 +274,15 @@
                 assert archive_file_name in zip_reference.namelist()
 
         with zipfile.ZipFile(path_model_archive, 'r') as zip_reference:
             zip_reference.extractall(extaction_directory_path)
 
         model = mktf.load_model(extaction_directory_path / archive_files['model'])
         model.load_weights(extaction_directory_path / archive_files['weights'])
+
+        with open(extaction_directory_path / archive_files['wrapper'], 'r') as f:
+            wrapper_dict = json.load(f)
+
+        wrapper = CNNCustomClassifier(**wrapper_dict)
+        wrapper.model = model
+        return wrapper
+
```

### Comparing `maat-machine-0.1.0/maat_machine/model/utils.py` & `maat-machine-0.1.1b1/maat_machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/packages.py` & `maat-machine-0.1.1b1/maat_machine/packages.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/pprint.py` & `maat-machine-0.1.1b1/maat_machine/pprint.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/maat_machine/utils.py` & `maat-machine-0.1.1b1/maat_machine/utils.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.0/pyproject.toml` & `maat-machine-0.1.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maat-machine"
-version = "0.1.0"
+version = "0.1.1b1"
 description = "Yet another package designed to simplify coding for data science and machine learning"
 authors = ["Dmitry Vlasov <dmitry.v.vlasov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "maat_machine"}]
 
 [tool.poetry.dependencies]
```

### Comparing `maat-machine-0.1.0/setup.py` & `maat-machine-0.1.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pillow>=10.3.0,<11.0.0',
  'scikit-learn>=1.4.2,<2.0.0',
  'tensorflow==2.16.1',
  'tqdm>=4.66.4,<5.0.0']
 
 setup_kwargs = {
     'name': 'maat-machine',
-    'version': '0.1.0',
+    'version': '0.1.1b1',
     'description': 'Yet another package designed to simplify coding for data science and machine learning',
     'long_description': '',
     'author': 'Dmitry Vlasov',
     'author_email': 'dmitry.v.vlasov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `maat-machine-0.1.0/PKG-INFO` & `maat-machine-0.1.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maat-machine
-Version: 0.1.0
+Version: 0.1.1b1
 Summary: Yet another package designed to simplify coding for data science and machine learning
 License: MIT
 Author: Dmitry Vlasov
 Author-email: dmitry.v.vlasov@gmail.com
 Requires-Python: ==3.11.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

