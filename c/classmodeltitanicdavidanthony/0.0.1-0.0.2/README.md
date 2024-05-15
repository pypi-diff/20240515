# Comparing `tmp/classmodeltitanicdavidanthony-0.0.1.tar.gz` & `tmp/classmodeltitanicdavidanthony-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classmodeltitanicdavidanthony-0.0.1.tar", last modified: Thu May  9 12:40:45 2024, max compression
+gzip compressed data, was "classmodeltitanicdavidanthony-0.0.2.tar", last modified: Wed May 15 20:31:27 2024, max compression
```

## Comparing `classmodeltitanicdavidanthony-0.0.1.tar` & `classmodeltitanicdavidanthony-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.042358 classmodeltitanicdavidanthony-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-05-07 18:08:48.000000 classmodeltitanicdavidanthony-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      515 2024-05-08 12:29:08.000000 classmodeltitanicdavidanthony-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1231 2024-05-09 12:40:45.040299 classmodeltitanicdavidanthony-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:44.996309 classmodeltitanicdavidanthony-0.0.1/classification_model/
--rw-rw-rw-   0        0        0        7 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/VERSION
--rw-rw-rw-   0        0        0      879 2024-05-08 12:37:15.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:44.999310 classmodeltitanicdavidanthony-0.0.1/classification_model/config/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/config/__init__.py
--rw-rw-rw-   0        0        0     2316 2024-05-08 16:10:04.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/config/core.py
--rw-rw-rw-   0        0        0      859 2024-05-08 16:10:48.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/config.yml
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.005306 classmodeltitanicdavidanthony-0.0.1/classification_model/datasets/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/datasets/__init__.py
--rw-rw-rw-   0        0        0    21794 2024-05-07 18:49:48.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/datasets/test_titanic.csv
--rw-rw-rw-   0        0        0    87780 2024-05-07 18:49:48.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/datasets/train_titanic.csv
--rw-rw-rw-   0        0        0     1934 2024-05-08 16:12:03.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/pipeline.py
--rw-rw-rw-   0        0        0     1258 2024-05-08 16:59:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.016074 classmodeltitanicdavidanthony-0.0.1/classification_model/processing/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/processing/__init__.py
--rw-rw-rw-   0        0        0     3432 2024-05-08 16:51:02.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/processing/data_manager.py
--rw-rw-rw-   0        0        0     1748 2024-05-08 15:04:55.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/processing/features.py
--rw-rw-rw-   0        0        0     1400 2024-05-08 17:09:11.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/processing/validation.py
--rw-rw-rw-   0        0        0      943 2024-05-08 15:05:22.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.019788 classmodeltitanicdavidanthony-0.0.1/classification_model/trained_models/
--rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/trained_models/__init__.py
--rw-rw-rw-   0        0        0     3454 2024-05-08 17:16:52.000000 classmodeltitanicdavidanthony-0.0.1/classification_model/trained_models/classification_model_output_v0.0.1.pkl
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.038299 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/
--rw-rw-rw-   0        0        0     1231 2024-05-09 12:40:44.000000 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1136 2024-05-09 12:40:44.000000 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:40:44.000000 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2024-05-09 12:40:44.000000 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-09 12:40:44.000000 classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1962 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.032299 classmodeltitanicdavidanthony-0.0.1/requirements/
--rw-rw-rw-   0        0        0      604 2024-05-08 17:10:25.000000 classmodeltitanicdavidanthony-0.0.1/requirements/requirements.txt
--rw-rw-rw-   0        0        0       69 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.1/requirements/test_requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:40:45.043299 classmodeltitanicdavidanthony-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2309 2024-05-09 12:40:27.000000 classmodeltitanicdavidanthony-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:40:45.036299 classmodeltitanicdavidanthony-0.0.1/tests/
--rw-rw-rw-   0        0        0      590 2024-05-08 15:23:09.000000 classmodeltitanicdavidanthony-0.0.1/tests/test_features.py
--rw-rw-rw-   0        0        0      945 2024-05-08 17:16:20.000000 classmodeltitanicdavidanthony-0.0.1/tests/test_prediction.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.616750 classmodeltitanicdavidanthony-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-07 18:08:48.000000 classmodeltitanicdavidanthony-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-05-08 12:29:08.000000 classmodeltitanicdavidanthony-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1258 2024-05-15 20:31:27.615760 classmodeltitanicdavidanthony-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.575254 classmodeltitanicdavidanthony-0.0.2/classification_model/
+-rw-rw-rw-   0        0        0        7 2024-05-14 05:00:55.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/VERSION
+-rw-rw-rw-   0        0        0      879 2024-05-08 12:37:15.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.579292 classmodeltitanicdavidanthony-0.0.2/classification_model/config/
+-rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/config/__init__.py
+-rw-rw-rw-   0        0        0     2320 2024-05-14 06:28:05.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/config/core.py
+-rw-rw-rw-   0        0        0      951 2024-05-14 06:27:09.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.581851 classmodeltitanicdavidanthony-0.0.2/classification_model/datasets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1934 2024-05-14 05:12:21.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/pipeline.py
+-rw-rw-rw-   0        0        0     1258 2024-05-15 12:58:39.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.590374 classmodeltitanicdavidanthony-0.0.2/classification_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/processing/__init__.py
+-rw-rw-rw-   0        0        0     4001 2024-05-15 20:29:23.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0     1748 2024-05-08 15:04:55.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/processing/features.py
+-rw-rw-rw-   0        0        0     1401 2024-05-14 05:06:43.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1669 2024-05-15 20:28:03.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.593374 classmodeltitanicdavidanthony-0.0.2/classification_model/trained_models/
+-rw-rw-rw-   0        0        0        0 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/trained_models/__init__.py
+-rw-rw-rw-   0        0        0     3486 2024-05-15 20:29:34.000000 classmodeltitanicdavidanthony-0.0.2/classification_model/trained_models/classification_model_output_v0.0.2.pkl
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.613522 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/
+-rw-rw-rw-   0        0        0     1258 2024-05-15 20:31:27.000000 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-05-15 20:31:27.000000 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 20:31:27.000000 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2024-05-15 20:31:27.000000 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-15 20:31:27.000000 classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1962 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.606726 classmodeltitanicdavidanthony-0.0.2/requirements/
+-rw-rw-rw-   0        0        0      616 2024-05-14 05:58:29.000000 classmodeltitanicdavidanthony-0.0.2/requirements/requirements.txt
+-rw-rw-rw-   0        0        0       69 2024-04-03 17:10:35.000000 classmodeltitanicdavidanthony-0.0.2/requirements/test_requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 20:31:27.617751 classmodeltitanicdavidanthony-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2309 2024-05-09 12:40:27.000000 classmodeltitanicdavidanthony-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 20:31:27.609788 classmodeltitanicdavidanthony-0.0.2/tests/
+-rw-rw-rw-   0        0        0      587 2024-05-14 05:43:16.000000 classmodeltitanicdavidanthony-0.0.2/tests/test_features.py
+-rw-rw-rw-   0        0        0      927 2024-05-14 05:26:30.000000 classmodeltitanicdavidanthony-0.0.2/tests/test_prediction.py
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/LICENSE` & `classmodeltitanicdavidanthony-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/MANIFEST.in` & `classmodeltitanicdavidanthony-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/PKG-INFO` & `classmodeltitanicdavidanthony-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classmodeltitanicdavidanthony
-Version: 0.0.1
+Version: 0.0.2
 Summary: Classification model package from Train In Data.
 Home-page: https://github.com/davidanthony-ai/Deployment-titanic-package-MLOPS
 Author: DavidAnthony
 Author-email: daouedraogo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,9 +22,10 @@
 Requires-Dist: pandas==2.0.2
 Requires-Dist: pydantic<2.0.0,>=1.8.1
 Requires-Dist: scikit-learn<2.0.0,>=1.1.3
 Requires-Dist: strictyaml<2.0.0,>=1.3.2
 Requires-Dist: ruamel.yaml<1.0.0,>=0.16.12
 Requires-Dist: feature-engine==1.0.2
 Requires-Dist: joblib<2.0.0,>=1.0.1
+Requires-Dist: matplotlib
 
 Classification model package from Train In Data.
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/__init__.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/config/core.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/config/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 class AppConfig(BaseModel):
     """
     Application-level config.
     """
 
     package_name: str
-    training_data_file: str
-    test_data_file: str
     pipeline_save_file: str
+    titanic_data: str
+    feature_importance_save : str
 
 
 class ModelConfig(BaseModel):
     """
     All configuration relevant to model
     training and feature engineering.
     """
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/config.yml` & `classmodeltitanicdavidanthony-0.0.2/classification_model/config.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Package Overview
 package_name: classification_model
 
 # Data Files
-training_data_file: train_titanic.csv
-test_data_file: test_titanic.csv
+#training_data_file: train_titanic.csv
+#test_data_file: test_titanic.csv
+titanic_data: titanic_data.csv
 
 # Pipeline config
 pipeline_name: classification_model
 pipeline_save_file: classification_model_output_v
+feature_importance_save: feature_importance_model_output
 
 # Variables
 NUMERICAL_VARIABLES:
   - age
   - fare
   - pclass
   - sibsp
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/pipeline.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/predict.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/predict.py`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/processing/data_manager.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/processing/data_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import joblib
 import pandas as pd
 from sklearn.pipeline import Pipeline
 import numpy as np
 from classification_model import __version__ as _version
 from classification_model.config.core import DATASET_DIR, TRAINED_MODEL_DIR, config
 import re
-
+import json
 
 logger = logging.getLogger(__name__)
 
 
 # retain only the first cabin if more than
 # 1 are available per passenger
 # float type for np.nan
@@ -79,14 +79,29 @@
     # Prepare versioned save file name
     save_file_name = f"{config.app_config.pipeline_save_file}{_version}.pkl"
     save_path = TRAINED_MODEL_DIR / save_file_name
 
     remove_old_pipelines(files_to_keep=[save_file_name])
     joblib.dump(pipeline_to_persist, save_path)
 
+def save_feature_importance(*, features_imp: dict) -> None:
+    """Features importance saving.
+    Saves the versioned  
+    """
+    # Prepare versioned save file name
+    save_file_name = f"{config.app_config.feature_importance_save}{_version}.json"
+    save_path = TRAINED_MODEL_DIR / save_file_name
+    #print(save_path)
+
+    # Write data to the JSON file
+    with open(save_path, "w") as json_file:
+        #print(json_file)
+        #print(features_imp)
+        json.dump(features_imp, json_file)
+    #joblib.dump(features_imp, save_path)
 
 def load_pipeline(*, file_name: str) -> Pipeline:
     """Load a persisted pipeline."""
 
     file_path = TRAINED_MODEL_DIR / file_name
     trained_model = joblib.load(filename=file_path)
     return trained_model
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/processing/features.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/processing/validation.py` & `classmodeltitanicdavidanthony-0.0.2/classification_model/processing/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, ValidationError
 
 from classification_model.config.core import config
-from classification_model.processing.data_manager import pre_processing
+#from classification_model.processing.data_manager import pre_processing
 
 
 
 
 def validate_inputs(*, input_data: pd.DataFrame) -> Tuple[pd.DataFrame, Optional[dict]]:
     """Check model inputs for unprocessable values."""
     #pre_processed = pre_processing(dataframe=input_data)
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classification_model/trained_models/classification_model_output_v0.0.1.pkl` & `classmodeltitanicdavidanthony-0.0.2/classification_model/trained_models/classification_model_output_v0.0.2.pkl`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95fe 0500 0000 0000 008c 1073 6b6c  .............skl
+00000000: 8004 95f8 0500 0000 0000 008c 1073 6b6c  .............skl
 00000010: 6561 726e 2e70 6970 656c 696e 6594 8c08  earn.pipeline...
 00000020: 5069 7065 6c69 6e65 9493 9429 8194 7d94  Pipeline...)..}.
 00000030: 288c 0573 7465 7073 945d 9428 8c16 6361  (..steps.].(..ca
 00000040: 7465 676f 7269 6361 6c5f 696d 7075 7461  tegorical_imputa
 00000050: 7469 6f6e 948c 2566 6561 7475 7265 5f65  tion..%feature_e
 00000060: 6e67 696e 652e 696d 7075 7461 7469 6f6e  ngine.imputation
 00000070: 2e63 6174 6567 6f72 6963 616c 948c 1243  .categorical...C
@@ -14,203 +14,205 @@
 000000d0: 0976 6172 6961 626c 6573 945d 9428 8c03  .variables.].(..
 000000e0: 7365 7894 8c05 6361 6269 6e94 8c08 656d  sex...cabin...em
 000000f0: 6261 726b 6564 948c 0574 6974 6c65 9465  barked...title.e
 00000100: 8c0d 7265 7475 726e 5f6f 626a 6563 7494  ..return_object.
 00000110: 898c 0d69 6d70 7574 6572 5f64 6963 745f  ...imputer_dict_
 00000120: 947d 9428 6813 6810 6814 6810 6815 6810  .}.(h.h.h.h.h.h.
 00000130: 6816 6810 758c 0c69 6e70 7574 5f73 6861  h.h.u..input_sha
-00000140: 7065 5f94 4d45 034b 0986 9475 6286 948c  pe_.ME.K...ub...
+00000140: 7065 5f94 4d17 044b 0986 9475 6286 948c  pe_.M..K...ub...
 00000150: 116d 6973 7369 6e67 5f69 6e64 6963 6174  .missing_indicat
 00000160: 6f72 948c 2b66 6561 7475 7265 5f65 6e67  or..+feature_eng
 00000170: 696e 652e 696d 7075 7461 7469 6f6e 2e6d  ine.imputation.m
 00000180: 6973 7369 6e67 5f69 6e64 6963 6174 6f72  issing_indicator
 00000190: 948c 1341 6464 4d69 7373 696e 6749 6e64  ...AddMissingInd
 000001a0: 6963 6174 6f72 9493 9429 8194 7d94 2868  icator...)..}.(h
 000001b0: 115d 9428 8c03 6167 6594 8c04 6661 7265  .].(..age...fare
 000001c0: 948c 0670 636c 6173 7394 8c05 7369 6273  ...pclass...sibs
 000001d0: 7094 8c05 7061 7263 6894 658c 0c6d 6973  p...parch.e..mis
 000001e0: 7369 6e67 5f6f 6e6c 7994 888c 0a76 6172  sing_only....var
-000001f0: 6961 626c 6573 5f94 5d94 6824 6168 1a4d  iables_.].h$ah.M
-00000200: 4503 4b09 8694 7562 8694 8c11 6d65 6469  E.K...ub....medi
-00000210: 616e 5f69 6d70 7574 6174 696f 6e94 8c25  an_imputation..%
-00000220: 6665 6174 7572 655f 656e 6769 6e65 2e69  feature_engine.i
-00000230: 6d70 7574 6174 696f 6e2e 6d65 616e 5f6d  mputation.mean_m
-00000240: 6564 6961 6e94 8c11 4d65 616e 4d65 6469  edian...MeanMedi
-00000250: 616e 496d 7075 7465 7294 9394 2981 947d  anImputer...)..}
-00000260: 9428 680d 8c06 6d65 6469 616e 9468 1168  .(h...median.h.h
-00000270: 2368 187d 9428 8c03 6167 6594 4740 3b00  #h.}.(..age.G@;.
-00000280: 0000 0000 008c 0466 6172 6594 4740 2cea  .......fare.G@,.
-00000290: a64c 2f83 7b8c 0670 636c 6173 7394 4740  .L/.{..pclass.G@
-000002a0: 0800 0000 0000 008c 0573 6962 7370 9447  .........sibsp.G
-000002b0: 0000 0000 0000 0000 8c05 7061 7263 6894  ..........parch.
-000002c0: 4700 0000 0000 0000 0075 681a 4d45 034b  G........uh.ME.K
-000002d0: 0a86 9475 6286 948c 0e65 7874 7261 6374  ...ub....extract
-000002e0: 5f6c 6574 7465 7294 8c28 636c 6173 7369  _letter..(classi
-000002f0: 6669 6361 7469 6f6e 5f6d 6f64 656c 2e70  fication_model.p
-00000300: 726f 6365 7373 696e 672e 6665 6174 7572  rocessing.featur
-00000310: 6573 948c 1845 7874 7261 6374 4c65 7474  es...ExtractLett
-00000320: 6572 5472 616e 7366 6f72 6d65 7294 9394  erTransformer...
-00000330: 2981 947d 948c 0876 6172 6961 626c 6594  )..}...variable.
-00000340: 8c05 6361 6269 6e94 7362 8694 8c12 7261  ..cabin.sb....ra
-00000350: 7265 5f6c 6162 656c 5f65 6e63 6f64 6572  re_label_encoder
-00000360: 9468 3e8c 1b52 6172 654c 6162 656c 4361  .h>..RareLabelCa
-00000370: 7465 676f 7269 6361 6c45 6e63 6f64 6572  tegoricalEncoder
-00000380: 9493 9429 8194 7d94 288c 0972 6172 655f  ...)..}.(..rare_
-00000390: 7065 7263 9447 3fa9 9999 9999 999a 6811  perc.G?.......h.
-000003a0: 6812 8c0d 656e 636f 6465 725f 6469 6374  h...encoder_dict
-000003b0: 5f94 7d94 2868 135d 9428 8c04 6d61 6c65  _.}.(h.].(..male
-000003c0: 948c 0666 656d 616c 6594 6568 145d 9428  ...female.eh.].(
-000003d0: 8c01 4d94 8c01 4394 8c01 4294 6568 155d  ..M...C...B.eh.]
-000003e0: 9428 8c01 5394 6853 8c01 5194 6568 165d  .(..S.hS..Q.eh.]
-000003f0: 9428 8c02 4d72 948c 044d 6973 7394 8c03  .(..Mr...Miss...
-00000400: 4d72 7394 6575 7562 8694 8c13 6361 7465  Mrs.euub....cate
-00000410: 676f 7269 6361 6c5f 656e 636f 6465 7294  gorical_encoder.
-00000420: 8c1f 6665 6174 7572 655f 656e 6769 6e65  ..feature_engine
-00000430: 2e65 6e63 6f64 696e 672e 6f6e 655f 686f  .encoding.one_ho
-00000440: 7494 8c0d 4f6e 6548 6f74 456e 636f 6465  t...OneHotEncode
-00000450: 7294 9394 2981 947d 9428 8c0e 746f 705f  r...)..}.(..top_
-00000460: 6361 7465 676f 7269 6573 944e 8c09 6472  categories.N..dr
-00000470: 6f70 5f6c 6173 7494 8868 1168 1268 4c7d  op_last..h.h.hL}
-00000480: 9428 6813 5d94 684f 6168 145d 9428 6853  .(h.].hOah.].(hS
-00000490: 6852 8c04 5261 7265 9465 6815 5d94 2868  hR..Rare.eh.].(h
-000004a0: 5368 5665 6816 5d94 2868 598c 0452 6172  ShVeh.].(hY..Rar
-000004b0: 6594 685a 6575 681a 4d45 034b 0a86 9475  e.hZeuh.ME.K...u
-000004c0: 6286 948c 0673 6361 6c65 7294 8c1b 736b  b....scaler...sk
-000004d0: 6c65 6172 6e2e 7072 6570 726f 6365 7373  learn.preprocess
-000004e0: 696e 672e 5f64 6174 6194 8c0e 5374 616e  ing._data...Stan
-000004f0: 6461 7264 5363 616c 6572 9493 9429 8194  dardScaler...)..
-00000500: 7d94 288c 0977 6974 685f 6d65 616e 9488  }.(..with_mean..
-00000510: 8c08 7769 7468 5f73 7464 9488 8c04 636f  ..with_std....co
-00000520: 7079 9488 8c11 6665 6174 7572 655f 6e61  py....feature_na
-00000530: 6d65 735f 696e 5f94 8c13 6a6f 626c 6962  mes_in_...joblib
-00000540: 2e6e 756d 7079 5f70 6963 6b6c 6594 8c11  .numpy_pickle...
-00000550: 4e75 6d70 7941 7272 6179 5772 6170 7065  NumpyArrayWrappe
-00000560: 7294 9394 2981 947d 9428 8c08 7375 6263  r...)..}.(..subc
-00000570: 6c61 7373 948c 056e 756d 7079 948c 076e  lass...numpy...n
-00000580: 6461 7272 6179 9493 948c 0573 6861 7065  darray.....shape
-00000590: 944b 0f85 948c 056f 7264 6572 948c 0143  .K.....order...C
-000005a0: 948c 0564 7479 7065 9468 7e8c 0564 7479  ...dtype.h~..dty
-000005b0: 7065 9493 948c 024f 3894 8988 8794 5294  pe.....O8.....R.
-000005c0: 284b 038c 017c 944e 4e4e 4aff ffff ff4a  (K...|.NNNJ....J
-000005d0: ffff ffff 4b3f 7494 628c 0a61 6c6c 6f77  ....K?t.b..allow
-000005e0: 5f6d 6d61 7094 898c 1b6e 756d 7079 5f61  _mmap....numpy_a
-000005f0: 7272 6179 5f61 6c69 676e 6d65 6e74 5f62  rray_alignment_b
-00000600: 7974 6573 944b 1075 6280 0263 6e75 6d70  ytes.K.ub..cnump
-00000610: 792e 636f 7265 2e6d 756c 7469 6172 7261  y.core.multiarra
-00000620: 790a 5f72 6563 6f6e 7374 7275 6374 0a71  y._reconstruct.q
-00000630: 0063 6e75 6d70 790a 6e64 6172 7261 790a  .cnumpy.ndarray.
-00000640: 7101 4b00 8571 0263 5f63 6f64 6563 730a  q.K..q.c_codecs.
-00000650: 656e 636f 6465 0a71 0358 0100 0000 6271  encode.q.X....bq
-00000660: 0458 0600 0000 6c61 7469 6e31 7105 8671  .X....latin1q..q
-00000670: 0652 7107 8771 0852 7109 284b 014b 0f85  .Rq..q.Rq.(K.K..
-00000680: 710a 636e 756d 7079 0a64 7479 7065 0a71  q.cnumpy.dtype.q
-00000690: 0b58 0200 0000 4f38 710c 8988 8771 0d52  .X....O8q....q.R
-000006a0: 710e 284b 0358 0100 0000 7c71 0f4e 4e4e  q.(K.X....|q.NNN
-000006b0: 4aff ffff ff4a ffff ffff 4b3f 7471 1062  J....J....K?tq.b
-000006c0: 895d 7111 2858 0600 0000 7063 6c61 7373  .]q.(X....pclass
-000006d0: 7112 5803 0000 0061 6765 7113 5805 0000  q.X....ageq.X...
-000006e0: 0073 6962 7370 7114 5805 0000 0070 6172  .sibspq.X....par
-000006f0: 6368 7115 5804 0000 0066 6172 6571 1658  chq.X....fareq.X
-00000700: 0600 0000 6167 655f 6e61 7117 5808 0000  ....age_naq.X...
-00000710: 0073 6578 5f6d 616c 6571 1858 0700 0000  .sex_maleq.X....
-00000720: 6361 6269 6e5f 4371 1958 0700 0000 6361  cabin_Cq.X....ca
-00000730: 6269 6e5f 4d71 1a58 0a00 0000 6361 6269  bin_Mq.X....cabi
-00000740: 6e5f 5261 7265 711b 580a 0000 0065 6d62  n_Rareq.X....emb
-00000750: 6172 6b65 645f 4371 1c58 0a00 0000 656d  arked_Cq.X....em
-00000760: 6261 726b 6564 5f53 711d 5808 0000 0074  barked_Sq.X....t
-00000770: 6974 6c65 5f4d 7271 1e58 0a00 0000 7469  itle_Mrq.X....ti
-00000780: 746c 655f 5261 7265 711f 580a 0000 0074  tle_Rareq.X....t
-00000790: 6974 6c65 5f4d 6973 7371 2065 7471 2162  itle_Missq etq!b
-000007a0: 2e95 ca00 0000 0000 0000 8c0e 6e5f 6665  ............n_fe
-000007b0: 6174 7572 6573 5f69 6e5f 944b 0f8c 0f6e  atures_in_.K...n
-000007c0: 5f73 616d 706c 6573 5f73 6565 6e5f 948c  _samples_seen_..
-000007d0: 156e 756d 7079 2e63 6f72 652e 6d75 6c74  .numpy.core.mult
-000007e0: 6961 7272 6179 948c 0673 6361 6c61 7294  iarray...scalar.
-000007f0: 9394 6887 8c02 6938 9489 8887 9452 9428  ..h...i8.....R.(
-00000800: 4b03 8c01 3c94 4e4e 4e4a ffff ffff 4aff  K...<.NNNJ....J.
-00000810: ffff ff4b 0074 9462 4308 4503 0000 0000  ...K.t.bC.E.....
-00000820: 0000 9486 9452 948c 056d 6561 6e5f 9468  .....R...mean_.h
-00000830: 7a29 8194 7d94 2868 7d68 8068 814b 0f85  z)..}.(h}h.h.K..
-00000840: 9468 8368 8468 8568 878c 0266 3894 8988  .h.h.h.h...f8...
-00000850: 8794 5294 284b 0368 974e 4e4e 4aff ffff  ..R.(K.h.NNNJ...
-00000860: ff4a ffff ffff 4b00 7494 6268 8d88 688e  .J....K.t.bh..h.
-00000870: 4b10 7562 0bff ffff ffff ffff ffff ffff  K.ub............
-00000880: 3df2 c823 8f3c 0240 b4e4 3c53 e72d 3d40  =..#.<.@..<S.-=@
-00000890: 9f25 41af 6749 e03f 80ac 5c1d 202b d73f  .%A.gI.?..\. +.?
-000008a0: 2814 e624 bbb7 4040 ea34 b715 e577 c83f  (..$..@@.4...w.?
-000008b0: 9c8d fd67 bcb8 e43f d383 9d59 9f0b b23f  ...g...?...Y...?
-000008c0: 4b9c 8dfd 67bc e83f ce53 16cb 48ea ba3f  K...g..?.S..H..?
-000008d0: 38a8 1267 63ff c93f 3a5a 85dc e3ab e63f  8..gc..?:Z.....?
-000008e0: 9552 4a29 a594 e23f af67 49d0 eb59 b23f  .RJ)...?.gI..Y.?
-000008f0: c618 638c 31c6 c83f 952a 0000 0000 0000  ..c.1..?.*......
-00000900: 008c 0476 6172 5f94 687a 2981 947d 9428  ...var_.hz)..}.(
-00000910: 687d 6880 6881 4b0f 8594 6883 6884 6885  h}h.h.K...h.h.h.
-00000920: 68a2 688d 8868 8e4b 1075 6204 ffff ffff  h.h..h.K.ub.....
-00000930: 795c 6c9b 15f6 e63f 14ba 85f1 e29a 6440  y\l....?......d@
-00000940: ee15 b47a 224c f23f 2027 0841 a2c8 e23f  ...z"L.? '.A...?
-00000950: 1bf4 eb57 8351 a540 b520 04e0 7eca c33f  ...W.Q.@. ..~..?
-00000960: 1cc6 fdab 9936 cd3f 5079 ee69 fcc5 b03f  .....6.?Py.i...?
-00000970: 5707 10e8 da75 c63f 19d3 ad98 db15 b83f  W....u.?.......?
-00000980: 677e 7304 a3b7 c43f 8a99 caee bc6f ca3f  g~s....?.....o.?
-00000990: b650 117f e32a cf3f 000a 2f11 2709 b13f  .P...*.?../.'..?
-000009a0: d16e 6016 acfa c33f 952c 0000 0000 0000  .n`....?.,......
-000009b0: 008c 0673 6361 6c65 5f94 687a 2981 947d  ...scale_.hz)..}
-000009c0: 9428 687d 6880 6881 4b0f 8594 6883 6884  .(h}h.h.K...h.h.
-000009d0: 6885 68a2 688d 8868 8e4b 1075 6202 ffff  h.h.h..h.K.ub...
-000009e0: 2ac6 f76a 411b eb3f 7ef0 05d9 92ad 2940  *..jA..?~.....)@
-000009f0: 1a32 340f 351c f13f cdbc 5bae 5484 e83f  .24.5..?..[.T..?
-00000a00: 4b75 5970 661e 4a40 2034 19a8 6a2a d93f  KuYpf.J@ 4..j*.?
-00000a10: 419d 8935 2d93 de3f 1f0c 6727 d361 d03f  A..5-..?..g'.a.?
-00000a20: f9ab 301f 26cf da3f 4eb8 5b71 78a1 d33f  ..0.&..?N.[qx..?
-00000a30: 50f0 50af 76bf d93f 7e16 ad63 e415 dd3f  P.P.v..?~..c...?
-00000a40: 22c6 8ffe bd94 df3f 2d94 d25b 7f82 d03f  "......?-..[...?
-00000a50: facf 2c64 f948 d93f 9573 0100 0000 0000  ..,d.H.?.s......
-00000a60: 008c 105f 736b 6c65 6172 6e5f 7665 7273  ..._sklearn_vers
-00000a70: 696f 6e94 8c05 312e 342e 3294 7562 8694  ion...1.4.2.ub..
-00000a80: 8c05 4c6f 6769 7494 8c1e 736b 6c65 6172  ..Logit...sklear
-00000a90: 6e2e 6c69 6e65 6172 5f6d 6f64 656c 2e5f  n.linear_model._
-00000aa0: 6c6f 6769 7374 6963 948c 124c 6f67 6973  logistic...Logis
-00000ab0: 7469 6352 6567 7265 7373 696f 6e94 9394  ticRegression...
-00000ac0: 2981 947d 9428 8c07 7065 6e61 6c74 7994  )..}.(..penalty.
-00000ad0: 8c02 6c32 948c 0464 7561 6c94 898c 0374  ..l2...dual....t
-00000ae0: 6f6c 9447 3f1a 36e2 eb1c 432d 6884 473f  ol.G?.6...C-h.G?
-00000af0: 4062 4dd2 f1a9 fc8c 0d66 6974 5f69 6e74  @bM......fit_int
-00000b00: 6572 6365 7074 9488 8c11 696e 7465 7263  ercept....interc
-00000b10: 6570 745f 7363 616c 696e 6794 4b01 8c0c  ept_scaling.K...
-00000b20: 636c 6173 735f 7765 6967 6874 944e 8c0c  class_weight.N..
-00000b30: 7261 6e64 6f6d 5f73 7461 7465 944b 008c  random_state.K..
-00000b40: 0673 6f6c 7665 7294 8c05 6c62 6667 7394  .solver...lbfgs.
-00000b50: 8c08 6d61 785f 6974 6572 944b 648c 0b6d  ..max_iter.Kd..m
-00000b60: 756c 7469 5f63 6c61 7373 948c 0461 7574  ulti_class...aut
-00000b70: 6f94 8c07 7665 7262 6f73 6594 4b00 8c0a  o...verbose.K...
-00000b80: 7761 726d 5f73 7461 7274 9489 8c06 6e5f  warm_start....n_
-00000b90: 6a6f 6273 944e 8c08 6c31 5f72 6174 696f  jobs.N..l1_ratio
-00000ba0: 944e 688f 4b0f 8c08 636c 6173 7365 735f  .Nh.K...classes_
-00000bb0: 9468 7a29 8194 7d94 2868 7d68 8068 814b  .hz)..}.(h}h.h.K
-00000bc0: 0285 9468 8368 8468 8568 9668 8d88 688e  ...h.h.h.h.h..h.
-00000bd0: 4b10 7562 0bff ffff ffff ffff ffff ffff  K.ub............
-00000be0: 0000 0000 0000 0000 0100 0000 0000 0000  ................
-00000bf0: 954f 0000 0000 0000 008c 076e 5f69 7465  .O.........n_ite
-00000c00: 725f 9468 7a29 8194 7d94 2868 7d68 8068  r_.hz)..}.(h}h.h
-00000c10: 814b 0185 9468 8368 8468 8568 878c 0269  .K...h.h.h.h...i
-00000c20: 3494 8988 8794 5294 284b 0368 974e 4e4e  4.....R.(K.h.NNN
-00000c30: 4aff ffff ff4a ffff ffff 4b00 7494 6268  J....J....K.t.bh
-00000c40: 8d88 688e 4b10 7562 07ff ffff ffff ffff  ..h.K.ub........
-00000c50: 0700 0000 952d 0000 0000 0000 008c 0563  .....-.........c
-00000c60: 6f65 665f 9468 7a29 8194 7d94 2868 7d68  oef_.hz)..}.(h}h
-00000c70: 8068 814b 014b 0f86 9468 8368 8468 8568  .h.K.K...h.h.h.h
-00000c80: a268 8d88 688e 4b10 7562 05ff ffff ffff  .h..h.K.ub......
-00000c90: 647d 4bfb dffe a8bf e62d 956a 92e6 7ebf  d}K......-.j..~.
-00000ca0: fa9e a152 6c8d 90bf e3df f124 9981 933f  ...Rl......$...?
-00000cb0: 291b 3b0a 0333 a13f 17a7 6d55 a5ec 8ebf  ).;..3.?..mU....
-00000cc0: c9d1 e284 b88c b7bf c53d e5c0 bbe4 883f  .........=.....?
-00000cd0: 9cdb 9356 61c1 a7bf b71d 9414 5da0 a03f  ...Va.......]..?
-00000ce0: 6589 ef14 b8d0 9e3f 6b6f 2faf 3bbf 9ebf  e......?ko/.;...
-00000cf0: dc02 89b4 f717 b7bf eff7 6385 090b 793f  ..........c...y?
-00000d00: a68d b1e2 30b3 aa3f 9530 0000 0000 0000  ....0..?.0......
-00000d10: 008c 0a69 6e74 6572 6365 7074 5f94 687a  ...intercept_.hz
-00000d20: 2981 947d 9428 687d 6880 6881 4b01 8594  )..}.(h}h.h.K...
-00000d30: 6883 6884 6885 68a2 688d 8868 8e4b 1075  h.h.h.h.h..h.K.u
-00000d40: 620e ffff ffff ffff ffff ffff ffff ffff  b...............
-00000d50: 9336 7fad 6c9c debf 951d 0000 0000 0000  .6..l...........
-00000d60: 0068 ac68 ad75 6286 9465 8c06 6d65 6d6f  .h.h.ub..e..memo
-00000d70: 7279 944e 68c2 8968 ac68 ad75 622e       ry.Nh..h.h.ub.
+000001f0: 6961 626c 6573 5f94 5d94 2868 2468 2565  iables_.].(h$h%e
+00000200: 681a 4d17 044b 0986 9475 6286 948c 116d  h.M..K...ub....m
+00000210: 6564 6961 6e5f 696d 7075 7461 7469 6f6e  edian_imputation
+00000220: 948c 2566 6561 7475 7265 5f65 6e67 696e  ..%feature_engin
+00000230: 652e 696d 7075 7461 7469 6f6e 2e6d 6561  e.imputation.mea
+00000240: 6e5f 6d65 6469 616e 948c 114d 6561 6e4d  n_median...MeanM
+00000250: 6564 6961 6e49 6d70 7574 6572 9493 9429  edianImputer...)
+00000260: 8194 7d94 2868 0d8c 066d 6564 6961 6e94  ..}.(h...median.
+00000270: 6811 6823 6818 7d94 288c 0361 6765 9447  h.h#h.}.(..age.G
+00000280: 403c 0000 0000 0000 8c04 6661 7265 9447  @<........fare.G
+00000290: 402c e88c e703 afb8 8c06 7063 6c61 7373  @,........pclass
+000002a0: 9447 4008 0000 0000 0000 8c05 7369 6273  .G@.........sibs
+000002b0: 7094 4700 0000 0000 0000 008c 0570 6172  p.G..........par
+000002c0: 6368 9447 0000 0000 0000 0000 7568 1a4d  ch.G........uh.M
+000002d0: 1704 4b0b 8694 7562 8694 8c0e 6578 7472  ..K...ub....extr
+000002e0: 6163 745f 6c65 7474 6572 948c 2863 6c61  act_letter..(cla
+000002f0: 7373 6966 6963 6174 696f 6e5f 6d6f 6465  ssification_mode
+00000300: 6c2e 7072 6f63 6573 7369 6e67 2e66 6561  l.processing.fea
+00000310: 7475 7265 7394 8c18 4578 7472 6163 744c  tures...ExtractL
+00000320: 6574 7465 7254 7261 6e73 666f 726d 6572  etterTransformer
+00000330: 9493 9429 8194 7d94 8c08 7661 7269 6162  ...)..}...variab
+00000340: 6c65 948c 0563 6162 696e 9473 6286 948c  le...cabin.sb...
+00000350: 1272 6172 655f 6c61 6265 6c5f 656e 636f  .rare_label_enco
+00000360: 6465 7294 683e 8c1b 5261 7265 4c61 6265  der.h>..RareLabe
+00000370: 6c43 6174 6567 6f72 6963 616c 456e 636f  lCategoricalEnco
+00000380: 6465 7294 9394 2981 947d 9428 8c09 7261  der...)..}.(..ra
+00000390: 7265 5f70 6572 6394 473f a999 9999 9999  re_perc.G?......
+000003a0: 9a68 1168 128c 0d65 6e63 6f64 6572 5f64  .h.h...encoder_d
+000003b0: 6963 745f 947d 9428 6813 5d94 288c 046d  ict_.}.(h.].(..m
+000003c0: 616c 6594 8c06 6665 6d61 6c65 9465 6814  ale...female.eh.
+000003d0: 5d94 288c 014d 948c 0143 9465 6815 5d94  ].(..M...C.eh.].
+000003e0: 288c 0153 9468 538c 0151 9465 6816 5d94  (..S.hS..Q.eh.].
+000003f0: 288c 024d 7294 8c04 4d69 7373 948c 034d  (..Mr...Miss...M
+00000400: 7273 9465 7575 6286 948c 1363 6174 6567  rs.euub....categ
+00000410: 6f72 6963 616c 5f65 6e63 6f64 6572 948c  orical_encoder..
+00000420: 1f66 6561 7475 7265 5f65 6e67 696e 652e  .feature_engine.
+00000430: 656e 636f 6469 6e67 2e6f 6e65 5f68 6f74  encoding.one_hot
+00000440: 948c 0d4f 6e65 486f 7445 6e63 6f64 6572  ...OneHotEncoder
+00000450: 9493 9429 8194 7d94 288c 0e74 6f70 5f63  ...)..}.(..top_c
+00000460: 6174 6567 6f72 6965 7394 4e8c 0964 726f  ategories.N..dro
+00000470: 705f 6c61 7374 9488 6811 6812 684c 7d94  p_last..h.h.hL}.
+00000480: 2868 135d 9468 4f61 6814 5d94 2868 528c  (h.].hOah.].(hR.
+00000490: 0452 6172 6594 6568 155d 9428 6855 6853  .Rare.eh.].(hUhS
+000004a0: 6856 6568 165d 9428 6858 6859 685a 6575  hVeh.].(hXhYhZeu
+000004b0: 681a 4d17 044b 0b86 9475 6286 948c 0673  h.M..K...ub....s
+000004c0: 6361 6c65 7294 8c1b 736b 6c65 6172 6e2e  caler...sklearn.
+000004d0: 7072 6570 726f 6365 7373 696e 672e 5f64  preprocessing._d
+000004e0: 6174 6194 8c0e 5374 616e 6461 7264 5363  ata...StandardSc
+000004f0: 616c 6572 9493 9429 8194 7d94 288c 0977  aler...)..}.(..w
+00000500: 6974 685f 6d65 616e 9488 8c08 7769 7468  ith_mean....with
+00000510: 5f73 7464 9488 8c04 636f 7079 9488 8c11  _std....copy....
+00000520: 6665 6174 7572 655f 6e61 6d65 735f 696e  feature_names_in
+00000530: 5f94 8c13 6a6f 626c 6962 2e6e 756d 7079  _...joblib.numpy
+00000540: 5f70 6963 6b6c 6594 8c11 4e75 6d70 7941  _pickle...NumpyA
+00000550: 7272 6179 5772 6170 7065 7294 9394 2981  rrayWrapper...).
+00000560: 947d 9428 8c08 7375 6263 6c61 7373 948c  .}.(..subclass..
+00000570: 056e 756d 7079 948c 076e 6461 7272 6179  .numpy...ndarray
+00000580: 9493 948c 0573 6861 7065 944b 1085 948c  .....shape.K....
+00000590: 056f 7264 6572 948c 0143 948c 0564 7479  .order...C...dty
+000005a0: 7065 9468 7c8c 0564 7479 7065 9493 948c  pe.h|..dtype....
+000005b0: 024f 3894 8988 8794 5294 284b 038c 017c  .O8.....R.(K...|
+000005c0: 944e 4e4e 4aff ffff ff4a ffff ffff 4b3f  .NNNJ....J....K?
+000005d0: 7494 628c 0a61 6c6c 6f77 5f6d 6d61 7094  t.b..allow_mmap.
+000005e0: 898c 1b6e 756d 7079 5f61 7272 6179 5f61  ...numpy_array_a
+000005f0: 6c69 676e 6d65 6e74 5f62 7974 6573 944b  lignment_bytes.K
+00000600: 1075 6280 0263 6e75 6d70 792e 636f 7265  .ub..cnumpy.core
+00000610: 2e6d 756c 7469 6172 7261 790a 5f72 6563  .multiarray._rec
+00000620: 6f6e 7374 7275 6374 0a71 0063 6e75 6d70  onstruct.q.cnump
+00000630: 790a 6e64 6172 7261 790a 7101 4b00 8571  y.ndarray.q.K..q
+00000640: 0263 5f63 6f64 6563 730a 656e 636f 6465  .c_codecs.encode
+00000650: 0a71 0358 0100 0000 6271 0458 0600 0000  .q.X....bq.X....
+00000660: 6c61 7469 6e31 7105 8671 0652 7107 8771  latin1q..q.Rq..q
+00000670: 0852 7109 284b 014b 1085 710a 636e 756d  .Rq.(K.K..q.cnum
+00000680: 7079 0a64 7479 7065 0a71 0b58 0200 0000  py.dtype.q.X....
+00000690: 4f38 710c 8988 8771 0d52 710e 284b 0358  O8q....q.Rq.(K.X
+000006a0: 0100 0000 7c71 0f4e 4e4e 4aff ffff ff4a  ....|q.NNNJ....J
+000006b0: ffff ffff 4b3f 7471 1062 895d 7111 2858  ....K?tq.b.]q.(X
+000006c0: 0600 0000 7063 6c61 7373 7112 5803 0000  ....pclassq.X...
+000006d0: 0061 6765 7113 5805 0000 0073 6962 7370  .ageq.X....sibsp
+000006e0: 7114 5805 0000 0070 6172 6368 7115 5804  q.X....parchq.X.
+000006f0: 0000 0066 6172 6571 1658 0600 0000 6167  ...fareq.X....ag
+00000700: 655f 6e61 7117 5807 0000 0066 6172 655f  e_naq.X....fare_
+00000710: 6e61 7118 5808 0000 0073 6578 5f6d 616c  naq.X....sex_mal
+00000720: 6571 1958 0700 0000 6361 6269 6e5f 4d71  eq.X....cabin_Mq
+00000730: 1a58 0a00 0000 6361 6269 6e5f 5261 7265  .X....cabin_Rare
+00000740: 711b 580a 0000 0065 6d62 6172 6b65 645f  q.X....embarked_
+00000750: 5371 1c58 0a00 0000 656d 6261 726b 6564  Sq.X....embarked
+00000760: 5f43 711d 580a 0000 0065 6d62 6172 6b65  _Cq.X....embarke
+00000770: 645f 5171 1e58 0800 0000 7469 746c 655f  d_Qq.X....title_
+00000780: 4d72 711f 580a 0000 0074 6974 6c65 5f4d  Mrq.X....title_M
+00000790: 6973 7371 2058 0900 0000 7469 746c 655f  issq X....title_
+000007a0: 4d72 7371 2165 7471 2262 2e95 ca00 0000  Mrsq!etq"b......
+000007b0: 0000 0000 8c0e 6e5f 6665 6174 7572 6573  ......n_features
+000007c0: 5f69 6e5f 944b 108c 0f6e 5f73 616d 706c  _in_.K...n_sampl
+000007d0: 6573 5f73 6565 6e5f 948c 156e 756d 7079  es_seen_...numpy
+000007e0: 2e63 6f72 652e 6d75 6c74 6961 7272 6179  .core.multiarray
+000007f0: 948c 0673 6361 6c61 7294 9394 6885 8c02  ...scalar...h...
+00000800: 6938 9489 8887 9452 9428 4b03 8c01 3c94  i8.....R.(K...<.
+00000810: 4e4e 4e4a ffff ffff 4aff ffff ff4b 0074  NNNJ....J....K.t
+00000820: 9462 4308 1704 0000 0000 0000 9486 9452  .bC............R
+00000830: 948c 056d 6561 6e5f 9468 7829 8194 7d94  ...mean_.hx)..}.
+00000840: 2868 7b68 7e68 7f4b 1085 9468 8168 8268  (h{h~h.K...h.h.h
+00000850: 8368 858c 0266 3894 8988 8794 5294 284b  .h...f8.....R.(K
+00000860: 0368 954e 4e4e 4aff ffff ff4a ffff ffff  .h.NNNJ....J....
+00000870: 4b00 7494 6268 8b88 688c 4b10 7562 01ff  K.t.bh..h.K.ub..
+00000880: e295 1d11 5660 0240 707a d54b eba5 3d40  ....V`.@pz.K..=@
+00000890: 93a3 95c4 84c7 e03f 2f19 cf77 5aa2 d83f  .......?/..wZ..?
+000008a0: 0eca 9a79 f8dc 4040 d3b9 38a8 302f c93f  ...y..@@..8.0/.?
+000008b0: bcb2 23c2 0a4c 4f3f f99c 32f7 7b43 e43f  ..#..LO?..2.{C.?
+000008c0: 697e bd6f e18a e83f e625 e3f9 4e4b c43f  i~.o...?.%..NK.?
+000008d0: f066 5dce 6cb5 e63f 2196 769d e40f c93f  .f].l..?!.v....?
+000008e0: 730d 1f27 a0b7 b73f 08c7 fe42 4237 e23f  s..'...?...BB7.?
+000008f0: 9e48 41d3 60ac c93f 9949 a504 9b6a c43f  .HA.`..?.I...j.?
+00000900: 952a 0000 0000 0000 008c 0476 6172 5f94  .*.........var_.
+00000910: 6878 2981 947d 9428 687b 687e 687f 4b10  hx)..}.(h{h~h.K.
+00000920: 8594 6881 6882 6883 68a0 688b 8868 8c4b  ..h.h.h.h.h..h.K
+00000930: 1075 620c ffff ffff ffff ffff ffff ffff  .ub.............
+00000940: aa85 4f49 cfa2 e63f 92e4 3f1b b2b5 6340  ..OI...?..?...c@
+00000950: a9e3 ff39 3a2e f33f 471c 86a2 9edb e63f  ...9:..?G......?
+00000960: e4ff aca2 3d69 a440 8d88 b440 b03a c43f  ....=i.@...@.:.?
+00000970: 00e2 c0bf 6344 4f3f 16e4 dfc4 4aba cd3f  ....cDO?....J..?
+00000980: 2946 2526 d2e0 c63f 6999 0efd 9913 c13f  )F%&...?i......?
+00000990: 820a 3269 ca5f ca3f fb09 c756 ad27 c43f  ..2i._.?...V.'.?
+000009a0: b859 bba9 1d85 b53f b099 422d e162 cf3f  .Y.....?..B-.b.?
+000009b0: 8fca 3adc 2286 c43f 9533 b6c9 f128 c13f  ..:."..?.3...(.?
+000009c0: 952c 0000 0000 0000 008c 0673 6361 6c65  .,.........scale
+000009d0: 5f94 6878 2981 947d 9428 687b 687e 687f  _.hx)..}.(h{h~h.
+000009e0: 4b10 8594 6881 6882 6883 68a0 688b 8868  K...h.h.h.h.h..h
+000009f0: 8c4b 1075 620a ffff ffff ffff ffff ffff  .K.ub...........
+00000a00: 3a6d 8312 ede9 ea3f 8229 98c2 2d1d 2940  :m.....?.)..-.)@
+00000a10: 3243 9847 ac84 f13f 78b4 8ee0 9d0b eb3f  2C.G...?x......?
+00000a20: 5856 bff1 908e 4940 8295 a453 5b71 d93f  XV....I@...S[q.?
+00000a30: f879 53c9 a6a1 9f3f 8b18 ea72 cad7 de3f  .yS....?...r...?
+00000a40: b172 7a6c b10e db3f 93dc 747f 5360 d73f  .rzl...?..t.S`.?
+00000a50: 7fd7 ee42 1d0d dd3f 1484 bbe5 6365 d93f  ...B...?....ce.?
+00000a60: 4e07 997d 4c8e d23f cb65 3038 0fb1 df3f  N..}L..?.e08...?
+00000a70: 7abe 3e9f a1a0 d93f b318 e3aa ea6e d73f  z.>....?.....n.?
+00000a80: 9573 0100 0000 0000 008c 105f 736b 6c65  .s........._skle
+00000a90: 6172 6e5f 7665 7273 696f 6e94 8c05 312e  arn_version...1.
+00000aa0: 342e 3294 7562 8694 8c05 4c6f 6769 7494  4.2.ub....Logit.
+00000ab0: 8c1e 736b 6c65 6172 6e2e 6c69 6e65 6172  ..sklearn.linear
+00000ac0: 5f6d 6f64 656c 2e5f 6c6f 6769 7374 6963  _model._logistic
+00000ad0: 948c 124c 6f67 6973 7469 6352 6567 7265  ...LogisticRegre
+00000ae0: 7373 696f 6e94 9394 2981 947d 9428 8c07  ssion...)..}.(..
+00000af0: 7065 6e61 6c74 7994 8c02 6c32 948c 0464  penalty...l2...d
+00000b00: 7561 6c94 898c 0374 6f6c 9447 3f1a 36e2  ual....tol.G?.6.
+00000b10: eb1c 432d 6882 473f 4062 4dd2 f1a9 fc8c  ..C-h.G?@bM.....
+00000b20: 0d66 6974 5f69 6e74 6572 6365 7074 9488  .fit_intercept..
+00000b30: 8c11 696e 7465 7263 6570 745f 7363 616c  ..intercept_scal
+00000b40: 696e 6794 4b01 8c0c 636c 6173 735f 7765  ing.K...class_we
+00000b50: 6967 6874 944e 8c0c 7261 6e64 6f6d 5f73  ight.N..random_s
+00000b60: 7461 7465 944b 008c 0673 6f6c 7665 7294  tate.K...solver.
+00000b70: 8c05 6c62 6667 7394 8c08 6d61 785f 6974  ..lbfgs...max_it
+00000b80: 6572 944b 648c 0b6d 756c 7469 5f63 6c61  er.Kd..multi_cla
+00000b90: 7373 948c 0461 7574 6f94 8c07 7665 7262  ss...auto...verb
+00000ba0: 6f73 6594 4b00 8c0a 7761 726d 5f73 7461  ose.K...warm_sta
+00000bb0: 7274 9489 8c06 6e5f 6a6f 6273 944e 8c08  rt....n_jobs.N..
+00000bc0: 6c31 5f72 6174 696f 944e 688d 4b10 8c08  l1_ratio.Nh.K...
+00000bd0: 636c 6173 7365 735f 9468 7829 8194 7d94  classes_.hx)..}.
+00000be0: 2868 7b68 7e68 7f4b 0285 9468 8168 8268  (h{h~h.K...h.h.h
+00000bf0: 8368 9468 8b88 688c 4b10 7562 03ff ffff  .h.h..h.K.ub....
+00000c00: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000c10: 954f 0000 0000 0000 008c 076e 5f69 7465  .O.........n_ite
+00000c20: 725f 9468 7829 8194 7d94 2868 7b68 7e68  r_.hx)..}.(h{h~h
+00000c30: 7f4b 0185 9468 8168 8268 8368 858c 0269  .K...h.h.h.h...i
+00000c40: 3494 8988 8794 5294 284b 0368 954e 4e4e  4.....R.(K.h.NNN
+00000c50: 4aff ffff ff4a ffff ffff 4b00 7494 6268  J....J....K.t.bh
+00000c60: 8b88 688c 4b10 7562 07ff ffff ffff ffff  ..h.K.ub........
+00000c70: 0700 0000 952d 0000 0000 0000 008c 0563  .....-.........c
+00000c80: 6f65 665f 9468 7829 8194 7d94 2868 7b68  oef_.hx)..}.(h{h
+00000c90: 7e68 7f4b 014b 1086 9468 8168 8268 8368  ~h.K.K...h.h.h.h
+00000ca0: a068 8b88 688c 4b10 7562 05ff ffff ffff  .h..h.K.ub......
+00000cb0: dcfb 0c5f c756 adbf 4431 6af5 7c47 7dbf  ..._.V..D1j.|G}.
+00000cc0: f3d0 e762 8214 91bf 91c7 f6b5 9874 7d3f  ...b.........t}?
+00000cd0: be27 f77b c79a a43f 39a5 fa9d c447 98bf  .'.{...?9....G..
+00000ce0: 482a 08ee 12e0 71bf 130d 7484 d752 b9bf  H*....q...t..R..
+00000cf0: 4e87 25e0 9bbf a9bf a3d5 3e61 db85 a73f  N.%.......>a...?
+00000d00: d352 a95a b516 9cbf 8b8f 6f44 382c a03f  .R.Z......oD8,.?
+00000d10: 3f2a e835 7109 5ebf 709f db0a 791c b9bf  ?*.5q.^.p...y...
+00000d20: e343 5da1 064c ac3f c708 e845 58ef b03f  .C]..L.?...EX..?
+00000d30: 9530 0000 0000 0000 008c 0a69 6e74 6572  .0.........inter
+00000d40: 6365 7074 5f94 6878 2981 947d 9428 687b  cept_.hx)..}.(h{
+00000d50: 687e 687f 4b01 8594 6881 6882 6883 68a0  h~h.K...h.h.h.h.
+00000d60: 688b 8868 8c4b 1075 6206 ffff ffff ffff  h..h.K.ub.......
+00000d70: 796a 946a 1895 dfbf 951d 0000 0000 0000  yj.j............
+00000d80: 0068 aa68 ab75 6286 9465 8c06 6d65 6d6f  .h.h.ub..e..memo
+00000d90: 7279 944e 68c0 8968 aa68 ab75 622e       ry.Nh..h.h.ub.
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/PKG-INFO` & `classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classmodeltitanicdavidanthony
-Version: 0.0.1
+Version: 0.0.2
 Summary: Classification model package from Train In Data.
 Home-page: https://github.com/davidanthony-ai/Deployment-titanic-package-MLOPS
 Author: DavidAnthony
 Author-email: daouedraogo@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,9 +22,10 @@
 Requires-Dist: pandas==2.0.2
 Requires-Dist: pydantic<2.0.0,>=1.8.1
 Requires-Dist: scikit-learn<2.0.0,>=1.1.3
 Requires-Dist: strictyaml<2.0.0,>=1.3.2
 Requires-Dist: ruamel.yaml<1.0.0,>=0.16.12
 Requires-Dist: feature-engine==1.0.2
 Requires-Dist: joblib<2.0.0,>=1.0.1
+Requires-Dist: matplotlib
 
 Classification model package from Train In Data.
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/classmodeltitanicdavidanthony.egg-info/SOURCES.txt` & `classmodeltitanicdavidanthony-0.0.2/classmodeltitanicdavidanthony.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 classification_model/config.yml
 classification_model/pipeline.py
 classification_model/predict.py
 classification_model/train_pipeline.py
 classification_model/config/__init__.py
 classification_model/config/core.py
 classification_model/datasets/__init__.py
-classification_model/datasets/test_titanic.csv
-classification_model/datasets/train_titanic.csv
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
-classification_model/trained_models/classification_model_output_v0.0.1.pkl
+classification_model/trained_models/classification_model_output_v0.0.2.pkl
 classmodeltitanicdavidanthony.egg-info/PKG-INFO
 classmodeltitanicdavidanthony.egg-info/SOURCES.txt
 classmodeltitanicdavidanthony.egg-info/dependency_links.txt
 classmodeltitanicdavidanthony.egg-info/requires.txt
 classmodeltitanicdavidanthony.egg-info/top_level.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/pyproject.toml` & `classmodeltitanicdavidanthony-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/requirements/requirements.txt` & `classmodeltitanicdavidanthony-0.0.2/requirements/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 #pandas>=1.3.5,<2.0.0
 pandas==2.0.2
 pydantic>=1.8.1,<2.0.0
 scikit-learn>=1.1.3,<2.0.0
 strictyaml>=1.3.2,<2.0.0
 ruamel.yaml>=0.16.12,<1.0.0
 feature-engine==1.0.2  # breaking change in v1.6.0
-joblib>=1.0.1,<2.0.0
+joblib>=1.0.1,<2.0.0
+matplotlib
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/setup.py` & `classmodeltitanicdavidanthony-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `classmodeltitanicdavidanthony-0.0.1/tests/test_features.py` & `classmodeltitanicdavidanthony-0.0.2/tests/test_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from classification_model.config.core import config
 from classification_model.processing.features import ExtractLetterTransformer
 
 
 def test_extractletter_variable_transformer(sample_input_data):
     # Given
-    #print(sample_input_data.loc[10,'cabin'])
+    #print(sample_input_data.loc[5,'cabin'])
     transformer = ExtractLetterTransformer(
         variable=config.model_config.CABIN,  # cabin
     )
-    assert sample_input_data[config.model_config.CABIN].iat[10] == 'A6'
+    assert sample_input_data[config.model_config.CABIN].iat[5] == 'G6'
 
     # When
     subject = transformer.fit_transform(sample_input_data)
 
     # Then
-    assert subject[config.model_config.CABIN].iat[10] == 'A'
+    assert subject[config.model_config.CABIN].iat[5] == 'G'
```

### Comparing `classmodeltitanicdavidanthony-0.0.1/tests/test_prediction.py` & `classmodeltitanicdavidanthony-0.0.2/tests/test_prediction.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 from sklearn.metrics import accuracy_score
 from classification_model.config.core import config
 
 
 def test_make_prediction(sample_input_data):
     y_true = sample_input_data[config.model_config.target]
     sample_input_data.drop(columns=[config.model_config.target],inplace=True)
-    print(sample_input_data.columns)
     # Given
     expected_no_predictions = 262
 
     # When
     result = make_prediction(data_input=sample_input_data)
-    print(result.get("errors"))
+    #print(result.get("errors"))
 
     # Then
     predictions = result.get("predictions")
     assert isinstance(predictions, np.ndarray)
     assert isinstance(predictions[0], np.int64)
     assert result.get("errors") is None
     assert len(predictions) == expected_no_predictions
     _predictions = list(predictions)
     accuracy = accuracy_score(_predictions, y_true)
-    assert accuracy > 0.6
+    assert accuracy > 0.7 #accuracy = 0.7137
```

