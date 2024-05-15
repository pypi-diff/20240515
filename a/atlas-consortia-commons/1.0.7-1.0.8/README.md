# Comparing `tmp/atlas-consortia-commons-1.0.7.tar.gz` & `tmp/atlas-consortia-commons-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-consortia-commons-1.0.7.tar", last modified: Wed Feb 14 20:08:54 2024, max compression
+gzip compressed data, was "atlas-consortia-commons-1.0.8.tar", last modified: Wed May 15 17:43:19 2024, max compression
```

## Comparing `atlas-consortia-commons-1.0.7.tar` & `atlas-consortia-commons-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.849704 atlas-consortia-commons-1.0.7/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1338 2024-02-14 20:08:54.849297 atlas-consortia-commons-1.0.7/PKG-INFO
--rw-r--r--   0 maxsibilla   (503) staff       (20)      910 2023-03-21 17:48:33.000000 atlas-consortia-commons-1.0.7/README.md
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.834121 atlas-consortia-commons-1.0.7/atlas_consortia_commons/
--rw-r--r--   0 maxsibilla   (503) staff       (20)        0 2023-03-15 17:35:40.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.845625 atlas-consortia-commons-1.0.7/atlas_consortia_commons/file/
--rw-r--r--   0 maxsibilla   (503) staff       (20)      535 2023-03-17 17:41:40.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/file/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.846346 atlas-consortia-commons-1.0.7/atlas_consortia_commons/object/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1835 2023-08-10 16:39:53.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/object/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.846924 atlas-consortia-commons-1.0.7/atlas_consortia_commons/rest/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     3539 2023-03-21 14:58:41.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/rest/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.847506 atlas-consortia-commons-1.0.7/atlas_consortia_commons/string/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1466 2023-04-17 14:52:57.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/string/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.848820 atlas-consortia-commons-1.0.7/atlas_consortia_commons/ubkg/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     3052 2023-03-21 17:48:46.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/ubkg/__init__.py
--rw-r--r--   0 maxsibilla   (503) staff       (20)     5177 2024-02-14 20:08:47.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons/ubkg/ubkg_sdk.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-02-14 20:08:54.845077 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1338 2024-02-14 20:08:54.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/PKG-INFO
--rw-r--r--   0 maxsibilla   (503) staff       (20)      538 2024-02-14 20:08:54.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/SOURCES.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)        1 2024-02-14 20:08:54.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/dependency_links.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)      163 2024-02-14 20:08:54.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/requires.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)       24 2024-02-14 20:08:54.000000 atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/top_level.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)       38 2024-02-14 20:08:54.849774 atlas-consortia-commons-1.0.7/setup.cfg
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1768 2024-02-14 20:08:47.000000 atlas-consortia-commons-1.0.7/setup.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.682394 atlas-consortia-commons-1.0.8/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1496 2024-05-15 17:43:19.682068 atlas-consortia-commons-1.0.8/PKG-INFO
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1068 2024-05-15 17:42:41.000000 atlas-consortia-commons-1.0.8/README.md
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.646267 atlas-consortia-commons-1.0.8/atlas_consortia_commons/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)        0 2023-03-15 17:35:40.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.655782 atlas-consortia-commons-1.0.8/atlas_consortia_commons/converter/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     2609 2024-05-15 17:42:41.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/converter/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.656541 atlas-consortia-commons-1.0.8/atlas_consortia_commons/decorator/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)    10289 2024-05-15 17:42:41.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/decorator/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.660410 atlas-consortia-commons-1.0.8/atlas_consortia_commons/file/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      535 2023-03-17 17:41:40.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/file/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.664013 atlas-consortia-commons-1.0.8/atlas_consortia_commons/object/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1835 2024-05-14 14:29:24.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/object/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.667912 atlas-consortia-commons-1.0.8/atlas_consortia_commons/rest/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     3539 2023-03-21 14:58:41.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/rest/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.672110 atlas-consortia-commons-1.0.8/atlas_consortia_commons/string/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1466 2023-04-17 14:52:57.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/string/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.680216 atlas-consortia-commons-1.0.8/atlas_consortia_commons/ubkg/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     3052 2023-03-21 17:48:46.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/ubkg/__init__.py
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     5177 2024-05-14 14:29:24.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons/ubkg/ubkg_sdk.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.655080 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1496 2024-05-15 17:43:19.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/PKG-INFO
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      676 2024-05-15 17:43:19.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)        1 2024-05-15 17:43:19.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      186 2024-05-15 17:43:19.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/requires.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)       24 2024-05-15 17:43:19.000000 atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/top_level.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)       38 2024-05-15 17:43:19.682471 atlas-consortia-commons-1.0.8/setup.cfg
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1889 2024-05-15 17:42:55.000000 atlas-consortia-commons-1.0.8/setup.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2024-05-15 17:43:19.681496 atlas-consortia-commons-1.0.8/test/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     3443 2024-05-15 17:42:41.000000 atlas-consortia-commons-1.0.8/test/test_converter.py
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     5103 2024-05-15 17:42:41.000000 atlas-consortia-commons-1.0.8/test/test_decorator.py
```

### Comparing `atlas-consortia-commons-1.0.7/PKG-INFO` & `atlas-consortia-commons-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-commons
-Version: 1.0.7
+Version: 1.0.8
 Summary: The common code supporting the web services in the consortia.
 Home-page: https://github.com/x-atlas-consortia/commons
 Author: Atlas Consortia
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -34,7 +34,18 @@
 
 
 ### Coding Conventions
 - Please use:
   - `snake_case` to name methods and variables. 
   - `PascalCase` for class names.
 - Do follow any additional code formatting and styles as seen in the project
+
+
+### Running Tests
+- Install `pytest` using the command
+```bash
+pip install -r requirements.dev.txt
+```
+- Run the tests using the command
+```bash
+pytest
+```
```

### Comparing `atlas-consortia-commons-1.0.7/README.md` & `atlas-consortia-commons-1.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -21,8 +21,19 @@
 - [REST](atlas_consortia_commons/rest/README.md): For making standardised rest responses
 
 
 ### Coding Conventions
 - Please use:
   - `snake_case` to name methods and variables. 
   - `PascalCase` for class names.
-- Do follow any additional code formatting and styles as seen in the project
+- Do follow any additional code formatting and styles as seen in the project
+
+
+### Running Tests
+- Install `pytest` using the command
+```bash
+pip install -r requirements.dev.txt
+```
+- Run the tests using the command
+```bash
+pytest
+```
```

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/file/__init__.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/file/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/object/__init__.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/object/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/rest/__init__.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/string/__init__.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/string/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/ubkg/__init__.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/ubkg/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons/ubkg/ubkg_sdk.py` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons/ubkg/ubkg_sdk.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.7/atlas_consortia_commons.egg-info/PKG-INFO` & `atlas-consortia-commons-1.0.8/atlas_consortia_commons.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-commons
-Version: 1.0.7
+Version: 1.0.8
 Summary: The common code supporting the web services in the consortia.
 Home-page: https://github.com/x-atlas-consortia/commons
 Author: Atlas Consortia
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -34,7 +34,18 @@
 
 
 ### Coding Conventions
 - Please use:
   - `snake_case` to name methods and variables. 
   - `PascalCase` for class names.
 - Do follow any additional code formatting and styles as seen in the project
+
+
+### Running Tests
+- Install `pytest` using the command
+```bash
+pip install -r requirements.dev.txt
+```
+- Run the tests using the command
+```bash
+pytest
+```
```

### Comparing `atlas-consortia-commons-1.0.7/setup.py` & `atlas-consortia-commons-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from setuptools import find_packages, setup
+from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="atlas-consortia-commons",
     # Test PyPi version
-    # version="1.0.10",
+    # version="1.0.11",
     # Prod PyPi version
-    version="1.0.7",
+    version="1.0.8",
     author="Atlas Consortia",
     author_email="api-developers@hubmapconsortium.org",
     description="The common code supporting the web services in the consortia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/x-atlas-consortia/commons",
     packages=['atlas_consortia_commons',
               'atlas_consortia_commons.rest',
               'atlas_consortia_commons.ubkg',
               'atlas_consortia_commons.file',
               'atlas_consortia_commons.string',
-              'atlas_consortia_commons.object'],
+              'atlas_consortia_commons.object',
+              'atlas_consortia_commons.converter',
+              'atlas_consortia_commons.decorator'],
     package_data={'': ['*.json']},
     include_package_data=True,
     install_requires=[
         'Flask==2.1.3',
         'Werkzeug==2.3.7',
+        'hubmap-commons>=2.1.14',
         # For now use pinned version of jsonref due to breaking changes made in 1.0.0
         'jsonref==0.3.0',
         'jsonschema>=3.2.0',
         'neo4j>=4.2.1',
         'pytz>=2021.1',
         'property>=2.2',
         # Airflow dependes on globus_sdk==1.9.0
```

