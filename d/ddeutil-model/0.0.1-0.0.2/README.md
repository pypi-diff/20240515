# Comparing `tmp/ddeutil_model-0.0.1.tar.gz` & `tmp/ddeutil_model-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_model-0.0.1.tar", last modified: Sun May  5 07:58:06 2024, max compression
+gzip compressed data, was "ddeutil_model-0.0.2.tar", last modified: Wed May 15 14:17:41 2024, max compression
```

## Comparing `ddeutil_model-0.0.1.tar` & `ddeutil_model-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.599022 ddeutil_model-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-05 07:58:06.599022 ddeutil_model-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:58:06.599022 ddeutil_model-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.591022 ddeutil_model-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.591022 ddeutil_model-0.0.1/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.595022 ddeutil_model-0.0.1/src/ddeutil/model/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/__base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/__enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/__types.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.595022 ddeutil_model-0.0.1/src/ddeutil/model/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/datasets/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/datasets/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/datasets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/trans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/src/ddeutil/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.599022 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-05 07:58:06.000000 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 07:58:06.000000 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:58:06.000000 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 07:58:06.000000 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 07:58:06.000000 ddeutil_model-0.0.1/src/ddeutil_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:58:06.599022 ddeutil_model-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_dataset_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_lineage_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_lineage_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_trans.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-05 07:58:02.000000 ddeutil_model-0.0.1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.541697 ddeutil_model-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.541697 ddeutil_model-0.0.2/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.545697 ddeutil_model-0.0.2/src/ddeutil/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.545697 ddeutil_model-0.0.2/src/ddeutil/model/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_types.py
```

### Comparing `ddeutil_model-0.0.1/LICENSE` & `ddeutil_model-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.1/PKG-INFO` & `ddeutil_model-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
-Keywords: data,model,utility
+Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ddeutil
 Requires-Dist: tzdata
 Requires-Dist: pydantic==2.7.1
-Requires-Dist: pyyaml==6.0.1
 
 # Data Utility Package: *Model*
 
 **Table of Contents**:
 
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This models package, **Armored**, implements any model objects for **Data Pipeline**
+This is **Model Utility**, implements any model objects for **Data Pipeline**
 or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
@@ -70,57 +71,48 @@
 ```
 
 ### Datasets
 
 ```python
 from ddeutil.model.datasets import Col, Tbl
 
-col = Col(name="foo", dtype="varchar( 100 )")
-assert "foo" == col.name
-assert "varchar" == col.dtype.type
-assert 100 == col.dtype.max_length
-
 tbl = Tbl(
-  name="foo",
-  feature=[
+  name="table_foo",
+  features=[
     Col(name="id", dtype="integer primary key"),
     Col(name="foo", dtype="varchar( 10 )"),
   ],
 )
-assert "foo" == tbl.name
-assert "id" == tbl.feature[0].name
+assert tbl.name == "table_foo"
+assert tbl.features[0].name == "id"
+assert tbl.features[0].dtype.type == "integer"
 ```
 
 ## Usecase
 
 If I have some catalog config, it easy to pass this config to model object.
 
 ```python
 import yaml
-from pydantic import BaseModel
-from ddeutil.model.datasets import Tbl
-
-
-class Schema(BaseModel):
-  name: str
-  objects: list[Tbl]
+from ddeutil.model.datasets import Scm
 
 
 config = yaml.safe_load("""
 name: "warehouse"
-objects:
+tables:
   - name: "customer_master"
-    feature:
+    features:
       - name: "id"
         dtype: "integer"
         pk: true
       - name: "name"
         dtype: "varchar( 256 )"
         nullable: false
 """)
-feature = Schema.model_validate(config)
-assert 1 == len(feature.objects)
+schema = Scm.model_validate(config)
+assert len(schema.tables) == 1
+assert schema.tables[0].name == 'customer_master'
 ```
 
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `ddeutil_model-0.0.1/README.md` & `ddeutil_model-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This models package, **Armored**, implements any model objects for **Data Pipeline**
+This is **Model Utility**, implements any model objects for **Data Pipeline**
 or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
@@ -44,57 +44,48 @@
 ```
 
 ### Datasets
 
 ```python
 from ddeutil.model.datasets import Col, Tbl
 
-col = Col(name="foo", dtype="varchar( 100 )")
-assert "foo" == col.name
-assert "varchar" == col.dtype.type
-assert 100 == col.dtype.max_length
-
 tbl = Tbl(
-  name="foo",
-  feature=[
+  name="table_foo",
+  features=[
     Col(name="id", dtype="integer primary key"),
     Col(name="foo", dtype="varchar( 10 )"),
   ],
 )
-assert "foo" == tbl.name
-assert "id" == tbl.feature[0].name
+assert tbl.name == "table_foo"
+assert tbl.features[0].name == "id"
+assert tbl.features[0].dtype.type == "integer"
 ```
 
 ## Usecase
 
 If I have some catalog config, it easy to pass this config to model object.
 
 ```python
 import yaml
-from pydantic import BaseModel
-from ddeutil.model.datasets import Tbl
-
-
-class Schema(BaseModel):
-  name: str
-  objects: list[Tbl]
+from ddeutil.model.datasets import Scm
 
 
 config = yaml.safe_load("""
 name: "warehouse"
-objects:
+tables:
   - name: "customer_master"
-    feature:
+    features:
       - name: "id"
         dtype: "integer"
         pk: true
       - name: "name"
         dtype: "varchar( 256 )"
         nullable: false
 """)
-feature = Schema.model_validate(config)
-assert 1 == len(feature.objects)
+schema = Scm.model_validate(config)
+assert len(schema.tables) == 1
+assert schema.tables[0].name == 'customer_master'
 ```
 
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `ddeutil_model-0.0.1/pyproject.toml` & `ddeutil_model-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [project]
 name = "ddeutil-model"
 description = "Data Developer & Engineer Model Utility Objects"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT"}
 authors = [{ name = "ddeutils", email = "korawich.anu@gmail.com" }]
-keywords = ['data', 'model', 'utility']
+keywords = ['data', 'model', 'utility', 'pipeline']
 classifiers = [
     "Topic :: Utilities",
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.9.13"
 dependencies = [
+    "ddeutil",
     "tzdata",
     "pydantic==2.7.1",
-    "pyyaml==6.0.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/ddeutils/ddeutil-model/"
 "Source Code" = "https://github.com/ddeutils/ddeutil-model/"
 
@@ -41,27 +42,19 @@
 
 [tool.shelf.version]
 version = "./src/ddeutil/model/__about__.py"
 changelog = "CHANGELOG.md"
 
 [tool.coverage.run]
 branch = true
-concurrency = ["thread", "multiprocessing"]
 source = ["ddeutil", "tests"]
-omit = [
-    "*/perfs/",
-    "scripts/",
-    "perf_*.py",
-]
 relative_files = true
 
 [tool.coverage.report]
-exclude_lines = [
-    "raise NotImplementedError"
-]
+exclude_lines = ["raise NotImplementedError"]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 console_output_style = "count"
 addopts = [
     "--strict-config",
     "--strict-markers",
@@ -85,14 +78,15 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.black]
 line-length = 80
+preview = true
 target-version = ['py39']
 exclude = """
 /(
     \\.git
     | \\.__pycache__
     | \\.idea
     | \\.ruff_cache
@@ -129,9 +123,9 @@
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/__base.py` & `ddeutil_model-0.0.2/src/ddeutil/model/__base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from __future__ import annotations
+
+import logging
 from typing import (
     AbstractSet,
     Any,
     Union,
 )
 
 from pydantic import BaseModel, ConfigDict
+from typing_extensions import Self
 
 AbstractSetOrDict = Union[
     AbstractSet[Union[int, str]],
     dict[Union[int, str], Any],
 ]
 
 
 class __BaseModel(BaseModel):
-    # This config allow to validate before assign new data to any field
+    # NOTE:
+    #   This config allow to validate before assign new data to any field
     model_config = ConfigDict(
         validate_assignment=True,
         use_enum_values=True,
         populate_by_name=True,
     )
 
 
@@ -67,18 +72,21 @@
             props: list = [prop for prop in props if prop not in exclude]
 
         # Update the attribute dict with the properties
         if props:
             attribs.update({prop: getattr(self, prop) for prop in props})
         return attribs
 
-    def update(self, data: dict):
+    def update(self, data: dict) -> Self:
         """Updatable method for update data to existing model data.
         docs: https://github.com/pydantic/pydantic/discussions/3139
         """
         update = self.dict()
         update.update(data)
         for k, v in (
             self.model_validate(update).dict(exclude_defaults=True).items()
         ):
+            logging.debug(
+                f"Updating value '{k}' from '{getattr(self, k, None)}' to '{v}'"
+            )
             setattr(self, k, v)
         return self
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/__enums.py` & `ddeutil_model-0.0.2/src/ddeutil/model/__enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
 from enum import Enum, IntEnum
 from functools import total_ordering
+from typing import TypeVar
 
+T = TypeVar("T")
 
-def enum_ordering(cls):
+
+def enum_ordering(cls: T) -> T:
     """Add order property to Enum object."""
 
-    def __lt__(self, other):
-        if type(other) is type(self):
+    def __lt__(self, other) -> bool:
+        if isinstance(other, type(self)):
             return self.value < other.value
         raise ValueError("Cannot compare different Enums")
 
     cls.__lt__ = __lt__
     return total_ordering(cls)
 
 
 class StrEnum(str, Enum):
-    """
-    StrEnum where enum.auto() returns the field name.
-    See https://docs.python.org/3.9/library/enum.html#using-automatic-values
+    """StrEnum where enum.auto() returns the field name.
+
+    Reference:
+        (https://docs.python.org/3.9/library/enum.html#using-automatic-values)
     """
 
     @staticmethod
     def _generate_next_value_(
         name: str,
         start: int,
         count: int,
@@ -36,36 +40,48 @@
     ) -> str:
         return name
 
     def __str__(self) -> str:
         return self.value
 
 
-@enum_ordering
-class Status(IntEnum):
-    SUCCESS: int = 0
-    APPROVED: int = 0
-    FAILED: int = 1
-    WAITING: int = 2
-    PROCESSING: int = 2
-    TRIGGERED: int = 2
+class Status(StrEnum):
+    SUCCESS: str = "SUCCESS"
+    APPROVED: str = "APPROVED"
+    FAILED: str = "FAILED"
+    WAITING: str = "WAITING"
+    PROCESSING: str = "PROCESSING"
+    TRIGGERED: str = "TRIGGERED"
 
     def in_process(self) -> bool:
-        return self.value == 2
+        return self.value in ("WAITING", "PROCESSING")
+
+    def is_done(self) -> bool:
+        return self.value == "SUCCESS"
+
+    def is_failed(self) -> bool:
+        return self.value == "FAILED"
 
 
 class Loading(StrEnum):
     FULL_DUMP = "F"
     DELTA = "D"
     MERGE = "D"
     TRANSACTION = "T"
     SCD_DELTA = "SCD_D"
     SCD_DUMP = "SCD_F"
     SCD_TRANS = "SCD_T"
 
+    def is_delta(self) -> bool:
+        return self.value == "D" or self.value == "SCD_D"
+
+    def is_scd(self) -> bool:
+        return self.value.startswith("SCD")
+
 
 class DataLayer(IntEnum):
     RAW: int = 0
     STAGING: int = 1
     PERSISTED: int = 2
     CURATED: int = 3
     MART: int = 4
+    REPORT: int = 5
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/conn.py` & `ddeutil_model-0.0.2/src/ddeutil/model/conn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
+from __future__ import annotations
+
 from typing import (
     Annotated,
     Any,
     Literal,
     Optional,
     Union,
 )
 
-from pydantic import (
-    Field,
-)
-from pydantic.functional_validators import (
-    field_validator,
-)
+from pydantic import Field
+from pydantic.functional_validators import field_validator
 from pydantic.types import SecretStr
 
 from .__base import BaseUpdatableModel
 from .__types import CustomUrl, FileUrl
+from .utils import unquote_str
 
 
 class BaseConn(BaseUpdatableModel):
     type: str = "base"
 
 
 class FlConn(BaseConn):
@@ -34,28 +33,25 @@
     port: Optional[int] = None
     user: Optional[str] = None
     pwd: Optional[SecretStr] = None
     path: str
     options: Annotated[dict[str, Any], Field(default_factory=dict)]
 
     @classmethod
-    def from_url(
-        cls,
-        url: Union[FileUrl, str],
-    ) -> "FlConn":
+    def from_url(cls, url: Union[FileUrl, str]) -> FlConn:
         if isinstance(url, str):
             url = FileUrl(url=url)
         elif not isinstance(url, FileUrl):
             raise ValueError("A url value must be string or `FileUrl` object")
         return cls(
             sys=url.scheme,
-            pointer=url.host,
+            pointer=unquote_str(url.password),
             port=url.port,
-            user=url.username,
-            pwd=url.password,
+            user=unquote_str(url.username),
+            pwd=unquote_str(url.password),
             path=url.path,
             options=dict(url.query_params()),
         )
 
 
 class DbConn(BaseConn):
     """Database Connection Model
@@ -73,28 +69,25 @@
     port: int
     user: str
     pwd: SecretStr
     db: str
     options: Annotated[dict[str, Any], Field(default_factory=dict)]
 
     @classmethod
-    def from_url(
-        cls,
-        url: Union[CustomUrl, str],
-    ) -> "DbConn":
+    def from_url(cls, url: Union[CustomUrl, str]) -> DbConn:
         if isinstance(url, str):
             url = CustomUrl(url=url)
         elif not isinstance(url, CustomUrl):
             raise ValueError("A url value must be string or `CustomUrl` object")
         return cls(
             driver=url.scheme,
-            host=url.host,
+            host=unquote_str(url.host),
             port=url.port,
-            user=url.username,
-            pwd=url.password,
+            user=unquote_str(url.username),
+            pwd=unquote_str(url.password),
             db=url.path,
             options=dict(url.query_params()),
         )
 
     @field_validator("db")
-    def check_db_name(cls, v: str) -> str:
-        return v.lstrip("/").split("/")[0]
+    def __check_db_name(cls, v: str) -> str:
+        return v.split("/")[0]
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/const.py` & `ddeutil_model-0.0.2/src/ddeutil/model/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
+from __future__ import annotations
+
 from typing import (
     Annotated,
     Optional,
 )
 
 from pydantic import BaseModel, Field
 
 
 class Const(BaseModel):
     """Constraint Model"""
 
     of: Annotated[
         Optional[str],
-        Field(description="Owner of this Constraint"),
+        Field(description="Owner of Constraint"),
     ] = None
 
     @property
     def name(self) -> str:
         if not self.of:
             raise ValueError(
                 "This constraint does not pass `of` value for take ownership."
@@ -28,18 +30,16 @@
         return f"{self.of}_const"
 
 
 class Pk(Const):
     """Primary Key Model.
 
     Examples:
-        *   {
-                "of": "foo",
-                "cols": ["bar", "baz"],
-            }
+        >>> Pk(of="foo", cols=["bar", "baz"]).name
+        'foo_bar_baz_pk'
     """
 
     cols: Annotated[
         list[str],
         Field(default_factory=list, description="List of primary key columns"),
     ]
 
@@ -68,29 +68,24 @@
     col: str
 
 
 class Fk(Const):
     """Foreign Key Model.
 
     Examples:
-        *   {
-                "of": "foo",
-                "to": "bar",
-                "ref": {
-                    "table": "ref_table",
-                    "column": "ref_column"
-                }
-            }
-        *   {
-                "to": "bar",
-                "ref": {
-                    "table": "ref_table",
-                    "column": "ref_column"
-                }
-            }
+        >>> data={
+        ...     "of": "foo",
+        ...     "to": "bar",
+        ...     "ref": {
+        ...         "tbl": "ref_table",
+        ...         "col": "ref_column"
+        ...     }
+        ... }
+        >>> Fk.model_validate(data).name
+        'foo_bar_ref_table_ref_column_fk'
     """
 
     to: str
     ref: Ref
 
     @property
     def name(self) -> str:
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/datasets/col.py` & `ddeutil_model-0.0.2/src/ddeutil/model/datasets/col.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
+from __future__ import annotations
+
 import re
 from typing import (
     Annotated,
     Any,
     Optional,
     Union,
 )
 
+from ddeutil.core import onlyone
 from pydantic import Field
 from pydantic.functional_validators import (
     field_validator,
     model_validator,
 )
 
 from ..__base import BaseUpdatableModel
 from ..const import Ref
 from ..dtype import Dtype
-from ..settings import ColumnSetting
+from ..settings import ColConf
 from ..utils import (
     catch_str,
     extract_dtype,
-    only_one,
     split_dtype,
 )
 
 
 class BaseCol(BaseUpdatableModel):
     """Base Column Model"""
 
     name: Annotated[
         str,
         Field(
             description="Name of Column",
-            alias="ColumnName",
+            alias="Name",
         ),
     ]
+    desc: Annotated[
+        Optional[str], Field(description="Description of Column")
+    ] = None
     dtype: Annotated[
         Dtype,
         Field(
             union_mode="left_to_right",
             description="Data Type of Column",
             alias="DataType",
         ),
     ]
 
     @field_validator("name")
-    def prepare_name(cls, value: str) -> str:
+    def __after_name(cls, value: str) -> str:
         """Prepare string value of name"""
         return "".join(value.strip().split())
 
     @field_validator("dtype", mode="before")
-    def prepare_str2dtype(cls, value: Union[str, dict, Dtype]):
+    def __before_str2dtype(cls, value: Union[str, dict, Dtype]) -> Dtype:
         """Prepare string value of dtype"""
         if isinstance(value, str):
             return extract_dtype(value)
         return value
 
 
 class Col(BaseCol):
@@ -89,15 +94,16 @@
         Optional[str],
         Field(
             description="Check Statement",
             alias="Check",
         ),
     ] = None
 
-    # Special value that effect to parent model that include this model
+    # NOTE:
+    #   Special value that effect to parent model that include this model
     pk: Annotated[
         bool,
         Field(
             description="Primary key flag which can not contain null value",
             alias="PrimaryKey",
             repr=False,
         ),
@@ -109,15 +115,19 @@
             description="Foreign key reference",
             alias="ForeignKey",
             repr=False,
         ),
     ]
 
     @classmethod
-    def extract_column_from_dtype(cls, value: str) -> dict[str, Any]:
+    def extract_column_from_dtype(
+        cls,
+        value: str,
+    ) -> dict[str, Union[str, bool]]:
+        """Extract a mapping column model from a string datatype."""
         values: dict[str, Any] = {"nullable": False}
         _dtype, _nullable = split_dtype(value)
 
         # Remove unique value from datatype
         _dtype, values["unique"] = catch_str(_dtype, key="unique")
 
         # Remove primary key value from datatype
@@ -145,49 +155,49 @@
             values["dtype"] = _dtype.strip()
             values["default"] = _default.strip()
         else:
             values["dtype"] = _dtype
 
             if serial_flag:
                 _nullable: str = "not null"
+                # TODO:
+                #   Change this default value for serial to dynamic value.
                 values["default"] = "nextval('tablename_colname_seq')"
 
         if not values["pk"]:
             values["nullable"] = not re.search("not null", _nullable)
         return values
 
     @model_validator(mode="before")
-    def prepare_dtype(cls, values):
+    def __before_dtype(cls, values):
         """Prepare datatype value that parsing to this model with different
         types, string or dict type.
 
         This filter will prepare datatype value from the format,
             {DATATYPE} {UNIQUE} {NULLABLE} {DEFAULT}
             {PRIMARY KEY|FOREIGN KEY} {CHECK}
 
         Examples:
         - varchar( 100 ) not null default 'O' check( <name> <> 'test' )
         - serial not null primary key
         """
-        if not (
-            dtype_key := only_one(values, ColumnSetting.dtype, default=False)
-        ):
+        if not (dtype_key := onlyone(values, ColConf.dtype, default=False)):
             raise ValueError("dtype key does not contain in values")
 
         pre_dtype: Any = values.pop(dtype_key)
         values_update: dict[str, Any] = {}
         if isinstance(pre_dtype, str):
             values_update = cls.extract_column_from_dtype(pre_dtype)
         else:
             values["dtype"] = pre_dtype
 
         return values_update | values
 
     @model_validator(mode="after")
-    def validate_logic(self):
+    def __validate_logic(self):
         """Validate and check logic of values"""
         nullable: bool = self.nullable
         default: Union[int, str, None] = self.default
 
         # RULE: primary key and nullable does not True together
         if self.pk and nullable:
             # Raise: ValueError("`pk` and `nullable` can not be True together")
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/datasets/file.py` & `ddeutil_model-0.0.2/src/ddeutil/model/datasets/file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/dtype.py` & `ddeutil_model-0.0.2/src/ddeutil/model/dtype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
+from __future__ import annotations
+
 from typing import (
     Annotated,
     Literal,
     Union,
 )
 
 from pydantic import BaseModel, Field
@@ -52,15 +54,15 @@
 
     Note: variable-length strings with limit
     """
 
     type: Literal["varchar"] = "varchar"
 
 
-class TextType(BaseType):
+class TextType(StringType):
     """Text Type
 
     Note: variable unlimited length strings
     """
 
     type: Literal["text"] = "text"
 
@@ -77,36 +79,46 @@
     def prepare_for_short_name(
         cls,
         value: Literal["integer", "int"],
     ) -> Literal["integer"]:
         return "integer" if value == "int" else value
 
 
-class SmallIntType(BaseType):
+class SmallIntType(IntegerType):
     """Small Range Integer
 
     Note: Storage size, 2 bytes, -32768 to +32767
     """
 
     type: Literal["smallint"] = "smallint"
 
 
-class BigIntType(BaseType):
+class BigIntType(IntegerType):
     """Big Range Integer
 
     Note: Storage size, 8 bytes, -9223372036854775808 to +9223372036854775807
     """
 
     type: Literal["bigint"] = "bigint"
 
 
-class ShortType(BaseType): ...
+class ShortType(SmallIntType):
+
+    type: Literal["short"] = "short"
+
+
+class LongType(BigIntType):
 
+    type: Literal["long"] = "long"
 
-class LongType(BaseType): ...
+
+class SerialType(IntegerType):
+    """Serial Type"""
+
+    type: Literal["serial"] = "serial"
 
 
 class NumericType(BaseType):
     """Numeric Type"""
 
     type: Literal["numeric"] = "numeric"
     precision: Annotated[int, Field(ge=-1)] = -1
@@ -137,33 +149,30 @@
 
 
 class TimestampType(BaseType):
     """Timestamp Type"""
 
     type: Literal["timestamp"] = "timestamp"
     precision: Annotated[int, Field(ge=-1, le=6)] = -1
-    timezone: Annotated[
-        bool,
-        Field(description="Time zone flag"),
-    ] = False
+    timezone: Annotated[bool, Field(description="Timezone flag")] = False
 
 
-class TimeType(BaseType): ...
+class TimeType(BaseType):
 
+    type: Literal["time"] = "time"
 
-class DateType(BaseType): ...
 
+class DateType(BaseType):
 
-class DateTimeType(BaseType): ...
+    type: Literal["date"] = "date"
 
 
-class SerialType(BaseType):
-    """Serial Type"""
+class DateTimeType(BaseType):
 
-    type: Literal["serial"]
+    type: Literal["datetime"] = "datetime"
 
 
 Dtype = Union[
     StringType,
     CharType,
     VarcharType,
     TextType,
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil/model/lineage.py` & `ddeutil_model-0.0.2/src/ddeutil/model/lineage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,116 @@
 # ------------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # ------------------------------------------------------------------------------
-from datetime import date, datetime
+from __future__ import annotations
+
+from datetime import date, datetime, timezone
 from typing import (
     Annotated,
+    Any,
     Optional,
 )
 from zoneinfo import ZoneInfo
 
-from pydantic import (
-    BaseModel,
-    Field,
-    field_validator,
-    model_validator,
-)
+from pydantic import BaseModel, Field
+from pydantic.functional_validators import field_validator, model_validator
 
 from .__base import BaseUpdatableModel
 from .__enums import Status
-from .settings import TSSetting
+from .settings import TSConf
+
+
+def dt_now() -> datetime:
+    return datetime.now(timezone.utc)
 
 
 class TS(BaseModel):
     """Time Model"""
 
-    ts: Annotated[
-        datetime,
-        Field(default_factory=lambda: datetime.utcnow(), alias="Timestamp"),
-    ]
-    tz: Annotated[str, Field(alias="TimeZone")] = TSSetting.tz
-
-    @property
-    def upts(self) -> datetime:
-        """Return updated timestamp"""
-        return datetime.now(tz=self.tz)
+    ts: Annotated[datetime, Field(default_factory=dt_now, alias="Timestamp")]
+    tz: Annotated[str, Field(alias="TimeZone")] = TSConf.tz
 
     @model_validator(mode="after")
-    def prepare_time(self):
+    def __prepare_time(self):
         self.ts: datetime = self.ts.astimezone(ZoneInfo(self.tz))
         return self
 
+    def now(self) -> datetime:
+        """Return updated timestamp"""
+        return datetime.now(tz=self.tz)
+
 
 class Tag(TS):
     """Tag Model"""
 
     author: Annotated[
         Optional[str],
         Field(validate_default=True, description="Author"),
     ] = None
     desc: Annotated[
         Optional[str],
         Field(repr=False, description="Description"),
     ] = None
     labels: Annotated[
         list[str],
-        Field(default_factory=list, description="Labels"),
+        Field(default_factory=list, description="Labels of Tag"),
     ]
     vs: Annotated[
         Optional[date],
-        Field(validate_default=True, alias="TagVersion"),
+        Field(validate_default=True, description="Version of Tag"),
     ] = None
 
     @field_validator("author")
-    def set_author(cls, value: Optional[str]):
+    def __set_author(cls, value: Optional[str]):
         return value or "undefined"
 
     @field_validator("vs")
-    def set_version(cls, value: Optional[date]):
+    def __set_version(cls, value: Optional[date]):
         """Pre initialize the `version` value that parsing from default"""
         return value if value else date(year=1990, month=1, day=1)
 
 
 class BaseTask(BaseUpdatableModel):
     """Base Task Model"""
 
-    st: Status
+    st: Status = Field(default=Status.WAITING, description="Status")
+    dt: Annotated[
+        datetime,
+        Field(default_factory=dt_now, alias="Datetime"),
+    ]
+
+
+class Task(BaseTask): ...
 
 
 class BaseMsg(BaseUpdatableModel):
     level: int
     msg: str
 
 
 class Msg(BaseMsg): ...
 
 
 class Log(BaseUpdatableModel):
+    """Log Model"""
+
     msgs: list[Msg]
+
+
+class BaseParam(BaseUpdatableModel):
+    extras: dict[str, Any]
+
+    @model_validator(mode="before")
+    def __prepare_extras(cls, values):
+        extras: dict[str, Any] = {
+            k: values.pop(k) for k in values.copy() if k not in cls.model_fields
+        } | values.pop("extras", {})
+        return {
+            "extras": extras,
+            **values,
+        }
+
+
+class NormalParam(BaseParam):
+    run_date: datetime
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil_model.egg-info/PKG-INFO` & `ddeutil_model-0.0.2/src/ddeutil_model.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
-Keywords: data,model,utility
+Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ddeutil
 Requires-Dist: tzdata
 Requires-Dist: pydantic==2.7.1
-Requires-Dist: pyyaml==6.0.1
 
 # Data Utility Package: *Model*
 
 **Table of Contents**:
 
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
 - [Usecase](#usecase)
 
-This models package, **Armored**, implements any model objects for **Data Pipeline**
+This is **Model Utility**, implements any model objects for **Data Pipeline**
 or **Data Platform**. The Model objects was implemented from the [Pydantic V2](https://docs.pydantic.dev/latest/).
 
 The model able to handle common logic validations and able to adjust by custom code
 for your specific requirements (Yeah, it just inherits Sub-Class from `BaseModel`).
 
 ## Installation
 
@@ -70,57 +71,48 @@
 ```
 
 ### Datasets
 
 ```python
 from ddeutil.model.datasets import Col, Tbl
 
-col = Col(name="foo", dtype="varchar( 100 )")
-assert "foo" == col.name
-assert "varchar" == col.dtype.type
-assert 100 == col.dtype.max_length
-
 tbl = Tbl(
-  name="foo",
-  feature=[
+  name="table_foo",
+  features=[
     Col(name="id", dtype="integer primary key"),
     Col(name="foo", dtype="varchar( 10 )"),
   ],
 )
-assert "foo" == tbl.name
-assert "id" == tbl.feature[0].name
+assert tbl.name == "table_foo"
+assert tbl.features[0].name == "id"
+assert tbl.features[0].dtype.type == "integer"
 ```
 
 ## Usecase
 
 If I have some catalog config, it easy to pass this config to model object.
 
 ```python
 import yaml
-from pydantic import BaseModel
-from ddeutil.model.datasets import Tbl
-
-
-class Schema(BaseModel):
-  name: str
-  objects: list[Tbl]
+from ddeutil.model.datasets import Scm
 
 
 config = yaml.safe_load("""
 name: "warehouse"
-objects:
+tables:
   - name: "customer_master"
-    feature:
+    features:
       - name: "id"
         dtype: "integer"
         pk: true
       - name: "name"
         dtype: "varchar( 256 )"
         nullable: false
 """)
-feature = Schema.model_validate(config)
-assert 1 == len(feature.objects)
+schema = Scm.model_validate(config)
+assert len(schema.tables) == 1
+assert schema.tables[0].name == 'customer_master'
 ```
 
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `ddeutil_model-0.0.1/src/ddeutil_model.egg-info/SOURCES.txt` & `ddeutil_model-0.0.2/src/ddeutil_model.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,35 +2,34 @@
 README.md
 pyproject.toml
 src/ddeutil/model/__about__.py
 src/ddeutil/model/__base.py
 src/ddeutil/model/__enums.py
 src/ddeutil/model/__init__.py
 src/ddeutil/model/__types.py
-src/ddeutil/model/cli.py
+src/ddeutil/model/action.py
 src/ddeutil/model/conn.py
 src/ddeutil/model/const.py
 src/ddeutil/model/dtype.py
 src/ddeutil/model/lineage.py
 src/ddeutil/model/settings.py
-src/ddeutil/model/trans.py
 src/ddeutil/model/utils.py
 src/ddeutil/model/datasets/__init__.py
 src/ddeutil/model/datasets/col.py
 src/ddeutil/model/datasets/db.py
 src/ddeutil/model/datasets/file.py
 src/ddeutil_model.egg-info/PKG-INFO
 src/ddeutil_model.egg-info/SOURCES.txt
 src/ddeutil_model.egg-info/dependency_links.txt
 src/ddeutil_model.egg-info/requires.txt
 src/ddeutil_model.egg-info/top_level.txt
+tests/test_action.py
 tests/test_base.py
 tests/test_conn.py
 tests/test_const.py
 tests/test_dataset_column.py
+tests/test_dataset_schema.py
 tests/test_dataset_table.py
 tests/test_dtype.py
 tests/test_enums.py
-tests/test_lineage_tag.py
-tests/test_lineage_task.py
-tests/test_trans.py
+tests/test_lineage.py
 tests/test_types.py
```

### Comparing `ddeutil_model-0.0.1/tests/test_base.py` & `ddeutil_model-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.1/tests/test_dataset_column.py` & `ddeutil_model-0.0.2/tests/test_dataset_column.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,140 @@
-import unittest
-
 import ddeutil.model.datasets.col as col
 import ddeutil.model.dtype as dtype
 
 
-class TestBaseColumn(unittest.TestCase):
-    def setUp(self):
-        self.maxDiff = None
-
-    def test_base_column_init(self):
-        t = col.BaseCol(name="foo", dtype={"type": "base"})
-        self.assertEqual("foo", t.name)
-        self.assertEqual("base", t.dtype.type)
-
-        t = col.BaseCol(name="foo", dtype="varchar( 100 )")
-        self.assertEqual("foo", t.name)
-        self.assertEqual("varchar", t.dtype.type)
-        self.assertEqual(100, t.dtype.max_length)
-
-        t = col.BaseCol(
-            name="foo", dtype={"type": "varchar", "max_length": 100}
-        )
-        self.assertEqual("foo", t.name)
-        self.assertEqual("varchar", t.dtype.type)
-        self.assertEqual(100, t.dtype.max_length)
-
-    def test_base_column_model_validate(self):
-        t = col.BaseCol.model_validate(
-            {
-                "name": "foo",
-                "dtype": {
-                    "type": "varchar",
-                    "max_length": 1000,
-                },
-            }
-        )
-        self.assertEqual("foo", t.name)
-        self.assertEqual("varchar", t.dtype.type)
-        self.assertEqual(1000, t.dtype.max_length)
-
-        t = col.BaseCol.model_validate(
-            {
-                "name": "foo",
-                "dtype": {"type": "int"},
-            }
-        )
-        self.assertEqual("foo", t.name)
-        self.assertEqual("integer", t.dtype.type)
-
-
-class TestColumn(unittest.TestCase):
-    def setUp(self):
-        self.maxDiff = None
-
-    def test_column_init(self):
-        t = col.Col(name="foo", dtype=dtype.BaseType())
-        self.assertDictEqual(
-            {
-                "name": "foo",
-                "dtype": {"type": "base"},
-                "nullable": True,
-                "unique": False,
-                "default": None,
-                "check": None,
-                "pk": False,
-                "fk": {},
-            },
-            t.model_dump(by_alias=False),
-        )
-
-        t = col.Col(name="foo", dtype={"type": "base"})
-        self.assertDictEqual(
-            {
-                "name": "foo",
-                "dtype": {"type": "base"},
-                "nullable": True,
-                "unique": False,
-                "default": None,
-                "check": None,
-                "pk": False,
-                "fk": {},
-            },
-            t.model_dump(by_alias=False),
-        )
-
-        t = col.Col(name="foo", dtype="base")
-        self.assertDictEqual(
-            {
-                "name": "foo",
-                "dtype": {"type": "base"},
-                "nullable": True,
-                "unique": False,
-                "default": None,
-                "check": None,
-                "pk": False,
-                "fk": {},
-            },
-            t.model_dump(by_alias=False),
-        )
-
-        t = col.Col(
-            name="foo",
-            dtype="varchar( 20 )",
-            fk={"table": "bar", "column": "baz"},
-        )
-        self.assertDictEqual(
-            {
-                "name": "foo",
-                "dtype": {"max_length": 20, "type": "varchar"},
-                "nullable": True,
-                "unique": False,
-                "default": None,
-                "check": None,
-                "pk": False,
-                "fk": {"table": "bar", "column": "baz"},
-            },
-            t.model_dump(by_alias=False),
-        )
-
-    def test_column_extract_column_from_dtype(self):
-        t = col.Col.extract_column_from_dtype("numeric( 10, 2 )")
-        self.assertEqual(
-            t,
-            {
-                "unique": False,
-                "pk": False,
-                "nullable": True,
-                "dtype": "numeric( 10, 2 )",
-            },
-        )
-
-        t = col.Col.extract_column_from_dtype(
-            "varchar( 100 ) not null default 'Empty' check( <name> <> 'test' )"
-        )
-        self.assertDictEqual(
-            t,
-            {
-                "unique": False,
-                "pk": False,
-                "nullable": False,
-                "check": "check( <name> <> 'test' )",
-                "dtype": "varchar( 100 )",
-                "default": "'Empty'",
-            },
-        )
-
-        t = col.Col.extract_column_from_dtype("serial primary key")
-        self.assertDictEqual(
-            t,
-            {
-                "unique": False,
-                "pk": True,
-                "nullable": False,
-                "dtype": "integer",
-                "default": "nextval('tablename_colname_seq')",
-            },
-        )
-
-        t = col.Col.extract_column_from_dtype("integer null default 1")
-        self.assertDictEqual(
-            t,
-            {
-                "unique": False,
-                "pk": False,
-                "nullable": True,
-                "dtype": "integer",
-                "default": "1",
-            },
-        )
+def test_base_column_init():
+    t = col.BaseCol(name="foo", dtype={"type": "base"})
+    assert "foo" == t.name
+    assert "base" == t.dtype.type
+
+    t = col.BaseCol(name="foo", dtype="varchar( 100 )")
+    assert "foo" == t.name
+    assert "varchar" == t.dtype.type
+    assert 100 == t.dtype.max_length
+
+    t = col.BaseCol(name="foo", dtype={"type": "varchar", "max_length": 100})
+    assert "foo" == t.name
+    assert "varchar" == t.dtype.type
+    assert 100 == t.dtype.max_length
+
+
+def test_base_column_model_validate():
+    t = col.BaseCol.model_validate(
+        {
+            "name": "foo",
+            "dtype": {
+                "type": "varchar",
+                "max_length": 1000,
+            },
+        }
+    )
+    assert "foo" == t.name
+    assert "varchar" == t.dtype.type
+    assert 1000 == t.dtype.max_length
+
+    t = col.BaseCol.model_validate(
+        {
+            "name": "foo",
+            "dtype": {"type": "int"},
+        }
+    )
+    assert "foo" == t.name
+    assert "integer" == t.dtype.type
+
+
+def test_column_init():
+    t = col.Col(name="foo", dtype=dtype.BaseType())
+    assert {
+        "name": "foo",
+        "dtype": {"type": "base"},
+        "desc": None,
+        "nullable": True,
+        "unique": False,
+        "default": None,
+        "check": None,
+        "pk": False,
+        "fk": {},
+    } == t.model_dump(by_alias=False)
+
+    t = col.Col(name="foo", dtype={"type": "base"})
+    assert {
+        "name": "foo",
+        "dtype": {"type": "base"},
+        "desc": None,
+        "nullable": True,
+        "unique": False,
+        "default": None,
+        "check": None,
+        "pk": False,
+        "fk": {},
+    } == t.model_dump(by_alias=False)
+
+    t = col.Col(name="foo", dtype="base")
+    assert {
+        "name": "foo",
+        "dtype": {"type": "base"},
+        "desc": None,
+        "nullable": True,
+        "unique": False,
+        "default": None,
+        "check": None,
+        "pk": False,
+        "fk": {},
+    } == t.model_dump(by_alias=False)
+
+    t = col.Col(
+        name="foo",
+        dtype="varchar( 20 )",
+        fk={"table": "bar", "column": "baz"},
+    )
+    assert {
+        "name": "foo",
+        "dtype": {"max_length": 20, "type": "varchar"},
+        "desc": None,
+        "nullable": True,
+        "unique": False,
+        "default": None,
+        "check": None,
+        "pk": False,
+        "fk": {"table": "bar", "column": "baz"},
+    } == t.model_dump(by_alias=False)
+
+
+def test_column_extract_column_from_dtype():
+    t = col.Col.extract_column_from_dtype("numeric( 10, 2 )")
+    assert t == {
+        "unique": False,
+        "pk": False,
+        "nullable": True,
+        "dtype": "numeric( 10, 2 )",
+    }
+
+    t = col.Col.extract_column_from_dtype(
+        "varchar( 100 ) not null default 'Empty' check( <name> <> 'test' )"
+    )
+    assert t == {
+        "unique": False,
+        "pk": False,
+        "nullable": False,
+        "check": "check( <name> <> 'test' )",
+        "dtype": "varchar( 100 )",
+        "default": "'Empty'",
+    }
+
+    t = col.Col.extract_column_from_dtype("serial primary key")
+    assert t == {
+        "unique": False,
+        "pk": True,
+        "nullable": False,
+        "dtype": "integer",
+        "default": "nextval('tablename_colname_seq')",
+    }
+
+    t = col.Col.extract_column_from_dtype("integer null default 1")
+    assert t == {
+        "unique": False,
+        "pk": False,
+        "nullable": True,
+        "dtype": "integer",
+        "default": "1",
+    }
```

### Comparing `ddeutil_model-0.0.1/tests/test_lineage_tag.py` & `ddeutil_model-0.0.2/tests/test_lineage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,78 @@
 import datetime
-import unittest
 from unittest import mock
 from zoneinfo import ZoneInfo
 
+import ddeutil.model.__enums as enum
 import ddeutil.model.lineage as lineages
 import ddeutil.model.settings as st
 
 
-class TestTS(unittest.TestCase):
-    @mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
-    def test_ts_init(self, mock_datetime):
-        mock_datetime.utcnow.return_value = datetime.datetime(
-            2023, 1, 1, 0, 0, 0
-        )
-        t = lineages.TS()
-        self.assertDictEqual(
-            t.model_dump(by_alias=False),
-            {
-                "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
-                    tz=ZoneInfo(st.TSSetting.tz)
-                ),
-                "tz": "Asia/Bangkok",
-            },
-        )
+@mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
+def test_ts_init(mock_datetime):
+    mock_datetime.now.return_value = datetime.datetime(2023, 1, 1, 0, 0, 0)
+    t = lineages.TS()
+    assert t.model_dump(by_alias=False) == {
+        "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
+            tz=ZoneInfo(st.TSConf.tz)
+        ),
+        "tz": "Asia/Bangkok",
+    }
+
+
+@mock.patch("ddeutil.model.lineage.date", wraps=datetime.date)
+@mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
+def test_tag_init(mock_datetime, mock_date):
+    mock_date.return_value = datetime.date(2023, 1, 1)
+    mock_datetime.now.return_value = datetime.datetime(2023, 1, 1, 0, 0, 0)
+    t = lineages.Tag()
+    assert t.model_dump(by_alias=False) == {
+        "author": "undefined",
+        "desc": None,
+        "labels": [],
+        "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
+            tz=ZoneInfo(st.TSConf.tz)
+        ),
+        "vs": datetime.date(2023, 1, 1),
+        "tz": "Asia/Bangkok",
+    }
+
+
+def test_task_init():
+    t = lineages.Task()
+    assert t.st == enum.Status.WAITING
 
 
-class TestTag(unittest.TestCase):
-    @mock.patch("ddeutil.model.lineage.date", wraps=datetime.date)
-    @mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
-    def test_tag_init(self, mock_datetime, mock_date):
-        mock_date.return_value = datetime.date(2023, 1, 1)
-        mock_datetime.utcnow.return_value = datetime.datetime(
-            2023, 1, 1, 0, 0, 0
-        )
-        t = lineages.Tag()
-        self.assertDictEqual(
-            t.model_dump(by_alias=False),
-            {
-                "author": "undefined",
-                "desc": None,
-                "labels": [],
-                "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
-                    tz=ZoneInfo(st.TSSetting.tz)
-                ),
-                "vs": datetime.date(2023, 1, 1),
-                "tz": "Asia/Bangkok",
+def test_base_param_init():
+    t = lineages.BaseParam.model_validate(
+        obj={
+            "foo": "bar",
+            "test": "demo",
+        }
+    )
+    assert t.extras == {
+        "foo": "bar",
+        "test": "demo",
+    }
+
+
+def test_normal_param():
+    t = lineages.NormalParam.model_validate(
+        obj={
+            "run_date": "2023-01-01 00:00:00",
+            "foo": "bar",
+            "test": "demo",
+            "extras": {
+                "test": "replace",
             },
-        )
+        }
+    )
+    assert t.run_date == datetime.datetime(2023, 1, 1, 0)
+    assert t.extras == {
+        "foo": "bar",
+        "test": "replace",
+    }
+
+
+def test_base_task_init():
+    t = lineages.BaseTask(st=enum.Status.WAITING)
+    print(t.model_dump())
```

