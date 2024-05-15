# Comparing `tmp/parameterframe-0.1.2.tar.gz` & `tmp/parameterframe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parameterframe-0.1.2.tar", last modified: Mon May 13 21:35:15 2024, max compression
+gzip compressed data, was "parameterframe-0.1.3.tar", last modified: Wed May 15 00:09:33 2024, max compression
```

## Comparing `parameterframe-0.1.2.tar` & `parameterframe-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 21:31:50.000000 parameterframe-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-13 21:35:15.268926 parameterframe-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-13 21:31:50.000000 parameterframe-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/parameterframe/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 21:34:48.000000 parameterframe-0.1.2/parameterframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96932 2024-05-13 21:34:48.000000 parameterframe-0.1.2/parameterframe/parameterframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 21:35:14.000000 parameterframe-0.1.2/parameterframe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:35:15.268926 parameterframe-0.1.2/parameterframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40400 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 21:35:15.000000 parameterframe-0.1.2/parameterframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:35:15.268926 parameterframe-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 00:06:06.000000 parameterframe-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42951 2024-05-15 00:09:33.055855 parameterframe-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-15 00:06:06.000000 parameterframe-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/parameterframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 00:09:06.000000 parameterframe-0.1.3/parameterframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98684 2024-05-15 00:09:06.000000 parameterframe-0.1.3/parameterframe/parameterframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:09:33.055855 parameterframe-0.1.3/parameterframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42951 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 00:09:33.000000 parameterframe-0.1.3/parameterframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 00:09:32.000000 parameterframe-0.1.3/parameterframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:09:33.055855 parameterframe-0.1.3/setup.cfg
```

### Comparing `parameterframe-0.1.2/LICENSE` & `parameterframe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.2/PKG-INFO` & `parameterframe-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,18 +25,22 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
+    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
+      from .autonotebook import tqdm as notebook_tqdm
+
+
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
@@ -48,18 +52,20 @@
 ### 1. Adding new solution and uploading it
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
+when using SqlAlchemyDatabaseManager with database for the first time, it might be useful to create tables with `SqlAlchemyDatabaseManager.create_tables` and if schema of the database needs to be reset `SqlAlchemyDatabaseManager.drop_tables`
+
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
     database_connector = SqlAlchemyDatabaseManager(connection_details = {
     'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
@@ -204,14 +210,17 @@
 ```python
 pf.push_solution(
     # either solution id or solution name should be provided
     solution_name = "new_example_solution"
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
+
+
 
 
 
     True
 
 
 
@@ -223,15 +232,15 @@
 ```
 
 
 ```python
 pf = ParameterFrame(
     params_path = params_path,
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 pf = ParameterFrame(
     params_path = params_path,
@@ -312,27 +321,27 @@
 ```python
 pf.add_parameter_set_to_solution(
     solution_id = 'b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_name="test_set")
 ```
 
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca is not in solutions saved to memory!
-    Name pink_bright_toaster_706 is assigned to b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca temporarily!
+    Name pink_happy_car_642 is assigned to b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca temporarily!
 
 
 
 
 
     True
 
 
 
 
 ```python
-pf.commit_solution(solution_name="pink_bright_toaster_706",
+pf.commit_solution(solution_name="pink_happy_car_642",
                     parameter_set_names=["test_set"])
 ```
 
     Commited solution tables for b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
 
 
 
@@ -431,15 +440,15 @@
   <tbody>
     <tr>
       <th>0</th>
       <td>a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5</td>
       <td>test_set</td>
       <td>example parameters for test purposes</td>
       <td>STAGING</td>
-      <td>2024-05-07 19:51:13</td>
+      <td>2024-05-15 00:09:10</td>
       <td>5</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
@@ -519,15 +528,15 @@
     <tr>
       <th>4</th>
       <td>1a4f19ee9e186ee739daecbc778501c5851d3fb5d05c4a3c1200e599855e8689</td>
       <td>param_21</td>
       <td></td>
       <td>param_21.ipynb</td>
       <td>other</td>
-      <td>4</td>
+      <td>2</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -535,29 +544,32 @@
 
 
 ```python
 pf.push_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                  parameter_set_names=["test_set"])
 ```
 
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
+
+
 
 
 
     True
 
 
 
 ### 5. Getting latest parameter set id for solution
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
@@ -568,42 +580,48 @@
 
 
 ```python
 pf.get_parameter_set_id_for_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                                                         deployment_status="STAGING")
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     ['a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5']
 
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'STAGING'
 
 
 
 ### 6. Changing parameter set status
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
@@ -618,38 +636,51 @@
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_ids = 'a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5',
     current_deployment_status = "PRODUCTION",
     new_deployment_status = "STAGING"
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
+
+
+    No deployed parameter_set_ids with PRODUCTION from selected!
 
 
 
-    True
+
+
+    False
 
 
 
 
 ```python
 pf.change_status_from_staging_to_production(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : STAGING -> PRODUCTION
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'PRODUCTION'
 
 
 
@@ -657,23 +688,29 @@
 ```python
 pf.change_status_from_production_to_archived(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : PRODUCTION -> ARCHIVED
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'ARCHIVED'
 
 
 
@@ -681,24 +718,34 @@
 ```python
 pf.change_status_from_archived_production(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
     No deployed parameter_set_ids with PRODUCTION from selected!
+
+
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : ARCHIVED -> PRODUCTION
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'PRODUCTION'
 
 
 
@@ -711,15 +758,15 @@
 
 
 ```python
 # - with database connector for MockerDB
 pf2 = ParameterFrame(
     params_path = params_path,
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf2 = ParameterFrame(
@@ -767,35 +814,63 @@
   <tbody>
   </tbody>
 </table>
 </div>
 
 
 
+When pulling information with database handler, one could pull specific parameter sets, solutions and everything.
+
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
+    No solutions with b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca could be pulled!
+
+
 
 
 
     True
 
 
 
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id=None)
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
+
+
+
+    True
+
+
+
+
+```python
+pf2.pull_solution()
+```
+
 
 
 
     True
 
 
 
@@ -833,31 +908,31 @@
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca</td>
+      <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
-      <td>1</td>
+      <td>2</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
 
 ```python
-pf2.show_parameter_sets(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca')
+pf2.show_parameter_sets(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5')
 ```
 
 
 
 
 <div>
 <style scoped>
@@ -884,31 +959,40 @@
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5</td>
-      <td>test_set</td>
-      <td>example parameters for test purposes</td>
-      <td>PRODUCTION</td>
-      <td>2024-05-07 19:51:13</td>
-      <td>5</td>
+      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
+      <td>blue_tiny_television_381</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 00:37:50</td>
+      <td>2</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
+      <td>yellow_shiny_microwave_931</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 00:36:04</td>
+      <td>3</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
 
 ```python
-pf2.show_parameters(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
-                    parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5')
 ```
 
 
 
 
 <div>
 <style scoped>
@@ -935,56 +1019,38 @@
       <th>file_type</th>
       <th>commited_attributes</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>4cea5b09e77da310c5105978f2ceea5c5d8c9c7b65d0e00b45135ea90fc011af</td>
-      <td>param_1</td>
+      <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
+      <td>Screenshot 2024-05-04 at 02</td>
       <td></td>
-      <td>param_1.yaml</td>
-      <td>yaml</td>
-      <td>3</td>
+      <td>Screenshot 2024-05-04 at 02.59.31.png</td>
+      <td>other</td>
+      <td>35</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>bf11768decb1d0204e2636edd05c354573d473e67f1b048369b2ee99c865bf5f</td>
-      <td>param_2</td>
-      <td></td>
-      <td>param_2.yaml</td>
-      <td>yaml</td>
-      <td>6</td>
-    </tr>
-    <tr>
-      <th>2</th>
-      <td>9a4a3ace265c9bf2facc0044ca24260c42805c6e7b2a608dfd2f56a54d9d36be</td>
-      <td>param_10</td>
-      <td></td>
-      <td>param_10.txt</td>
-      <td>txt</td>
-      <td>9</td>
-    </tr>
-    <tr>
-      <th>3</th>
-      <td>ace2f31433212fbf9e764069a30a7675ca78f496d31f061d06d0a0420fc52768</td>
-      <td>param_11</td>
+      <td>4d8ca206d9bd09296b69a95f0c3c62d233282025964c356811510cc074cc2c49</td>
+      <td>1</td>
       <td></td>
-      <td>param_11.dill</td>
+      <td>1. AF - opis projektu.pdf</td>
       <td>other</td>
-      <td>1</td>
+      <td>34</td>
     </tr>
     <tr>
-      <th>4</th>
-      <td>1a4f19ee9e186ee739daecbc778501c5851d3fb5d05c4a3c1200e599855e8689</td>
-      <td>param_21</td>
+      <th>2</th>
+      <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
+      <td>uploads</td>
       <td></td>
-      <td>param_21.ipynb</td>
+      <td>uploads.zip</td>
       <td>other</td>
-      <td>4</td>
+      <td>61</td>
     </tr>
   </tbody>
 </table>
 </div>
```

### Comparing `parameterframe-0.1.2/README.md` & `parameterframe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `parameterframe-0.1.2/parameterframe/parameterframe.py` & `parameterframe-0.1.3/parameterframe/parameterframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,22 +220,21 @@
                       solution_id : str = None,
                       parameter_set_id : str = None):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
-        if solution_id is None:
-            raise ValueError("Provide solution_id!")
-
         fetch_filters = {'table_name' : ['solution_description',
                                           'solution_parameter_set',
                                           'parameter_set',
-                                          'parameter_set_description'],
-                          'solution_id': [solution_id, None]}
+                                          'parameter_set_description']}
+
+        if solution_id:
+            fetch_filters['solution_id'] = [solution_id, None]
 
         if parameter_set_id:
             fetch_filters['parameter_set_id'] = [parameter_set_id, None]
 
         # fetch tables with solution and parameter_set_ids
         self.fetch_entries(
             filters = fetch_filters)
@@ -558,33 +557,43 @@
                     solution_id : str = None,
                     parameter_set_id : str = None):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
-        if solution_id is None:
-            raise ValueError("Provide solution_id!")
+        # if solution_id is None:
+        #     raise ValueError("Provide solution_id!")
 
         session = self.Session()
         try:
             # Fetch related entries based on solution_id and parameter_set_id
-            solution_descriptions = session.query(self.SolutionDescription).filter(
-                self.SolutionDescription.solution_id == solution_id).all()
+            if solution_id:
+                solution_descriptions = session.query(self.SolutionDescription).filter(
+                    self.SolutionDescription.solution_id == solution_id).all()
+            else:
+                solution_descriptions = session.query(self.SolutionDescription).filter().all()
+
             if parameter_set_id:
-                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
-                    self.SolutionParameterSet.solution_id == solution_id,
-                    self.SolutionParameterSet.parameter_set_id == parameter_set_id).all()
+                if solution_id:
+                    solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                        self.SolutionParameterSet.solution_id == solution_id,
+                        self.SolutionParameterSet.parameter_set_id == parameter_set_id).all()
+
                 parameter_sets = session.query(self.ParameterSet).filter(
                     self.ParameterSet.parameter_set_id == parameter_set_id).all()
                 parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
                     self.ParameterSetDescription.parameter_set_id == parameter_set_id).all()
             else:
-                solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
-                    self.SolutionParameterSet.solution_id == solution_id).all()
+
+                if solution_id:
+                    solution_parameter_sets = session.query(self.SolutionParameterSet).filter(
+                        self.SolutionParameterSet.solution_id == solution_id).all()
+                else:
+                    solution_parameter_sets = session.query(self.SolutionParameterSet).filter().all()
 
                 parameter_set_ids = [solution_parameter_set.parameter_set_id for solution_parameter_set in solution_parameter_sets]
 
                 parameter_sets = session.query(self.ParameterSet).filter(
                     self.ParameterSet.parameter_set_id.in_(parameter_set_ids)).all()
                 parameter_set_descriptions = session.query(self.ParameterSetDescription).filter(
                     self.ParameterSetDescription.parameter_set_id.in_(parameter_set_ids)).all()
@@ -1443,15 +1452,15 @@
 
         if seed is None:
             seed = self.seed
 
         if isinstance(seed, int):
             # Set the seed value
             random.seed(seed)
-            self.seed += 1
+            self.seed = seed + 1
 
         # Randomly choose a word from each list
         color = random.choice(colors)
         adj = random.choice(adjectives)
         noun = random.choice(nouns)
         digits = random.randint(100, 999)
         # Combine them to form a name
@@ -1480,15 +1489,15 @@
 
     # dependancies
     database_connector = attr.ib(default=None, type=MockerDatabaseConnector)
     file_type_handler = attr.ib(default=FileTypeHandler)
     name_generator = attr.ib(default=ComplexNameGenerator)
 
     # inner
-    seed = attr.ib(default=23, type=int)
+    seed = attr.ib(default=None, type=int)
     solutions = attr.ib(default={})
     param_sets = attr.ib(default={})
     param_attributes = attr.ib(default={})
 
     commited_tables = attr.ib(default={})
 
 
@@ -1649,15 +1658,15 @@
 
         # trim solution name
         solution_name = solution_name[:100]
 
         if solution_id is None:
             # if solution id not provided create new
             solution_id = self._generate_unique_id(
-                txt = self.name_generator.generate_random_name(seed = seed) \
+                txt = self.name_generator.generate_random_name(seed = 23) \
                     + solution_name)
 
         if solution_name not in self.solutions.keys():
             self.solutions[solution_name] = {}
 
         if 'solution_id' not in self.solutions[solution_name].keys():
             self.solutions[solution_name]['solution_id'] = solution_id
@@ -2234,49 +2243,75 @@
                       solution_id : str = None,
                       parameter_set_id : str = None):
 
         """
         Pulls commited tables from database for selected solutions
         """
 
-        if solution_id is None:
-            raise ValueError("Provide solution_id!")
-
-
-        (solution_description,
+        (solution_descriptions,
          solution_parameter_sets,
          parameter_sets,
          parameter_set_descriptions,
          parameter_descriptions,
          parameter_attributes,
          attribute_values) = self.database_connector.pull_tables(
             solution_id = solution_id,
             parameter_set_id = parameter_set_id
         )
 
-        if len(solution_description) == 0:
+        if len(solution_descriptions) == 0:
             self.logger.warning(f"No solutions with {solution_id} could be pulled!")
 
-        parameter_set_ids = [solution_parameter_set['parameter_set_id'] for solution_parameter_set in solution_parameter_sets]
+        parameter_set_ids = [solution_parameter_set['parameter_set_id'] \
+            for solution_parameter_set in solution_parameter_sets]
 
         if len(parameter_set_ids) == 0:
             self.logger.warning(f"No parameter sets were pulled for solution_id {solution_id}")
 
-        # get table lists into commited
-        self._rebuild_tables_from_pulled_data(
-            solution_id = solution_id,
-            parameter_set_ids = parameter_set_ids,
-            solution_description = solution_description,
-            solution_parameter_sets = solution_parameter_sets,
-            parameter_sets = parameter_sets,
-            parameter_set_descriptions = parameter_set_descriptions,
-            parameter_descriptions = parameter_descriptions,
-            parameter_attributes = parameter_attributes,
-            attribute_values = attribute_values
-        )
+        solution_ids = list(set([solution_descriptions['solution_id'] \
+            for solution_descriptions in solution_descriptions]))
+
+        if solution_parameter_sets:
+
+            for solution_id in solution_ids:
+
+                solution_description = [sd for sd in solution_descriptions if sd['solution_id'] == solution_id]
+                parameter_set_ids = list(set([sp['parameter_set_id'] for sp in solution_parameter_sets \
+                    if sp['solution_id'] == solution_id]))
+
+                for parameter_set_id in parameter_set_ids:
+
+                    solution_parameter_set = [sp for sp in solution_parameter_sets \
+                        if sp['solution_id'] == solution_id and sp['parameter_set_id'] == parameter_set_id]
+
+                    parameter_set_description = [sp for sp in parameter_set_descriptions \
+                        if sp['parameter_set_id'] == parameter_set_id]
+
+                    parameter_set = [sp for sp in parameter_sets \
+                        if sp['parameter_set_id'] == parameter_set_id]
+
+                    parameter_ids = [sp['parameter_id'] for sp in parameter_set]
+
+                    parameter_description = [sp for sp in parameter_descriptions \
+                        if sp['parameter_id'] in parameter_ids]
+
+                    # get table lists into commited
+                    self._rebuild_tables_from_pulled_data(
+                        solution_id = solution_id,
+                        parameter_set_ids = [parameter_set_id],
+                        solution_description = solution_description,
+                        solution_parameter_sets = solution_parameter_set,
+                        parameter_sets = parameter_set,
+                        parameter_set_descriptions = parameter_set_description,
+                        parameter_descriptions = parameter_description,
+                        parameter_attributes = parameter_attributes,
+                        attribute_values = attribute_values
+                    )
+        else:
+            self.logger.warning(f"Nothing was pulled for {solution_id}")
 
         return True
 
     def _change_deployment_status(self,
                                  deployment_status : str,
                                  solution_id : str = None,
                                 solution_name : str = None,
```

### Comparing `parameterframe-0.1.2/parameterframe/setup.py` & `parameterframe-0.1.3/parameterframe/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="parameterframe",
     packages=["parameterframe"],
-    install_requires=['### parameterframe.py', 'dill', 'attrs', 'pyyaml', 'sqlalchemy', 'pandas', 'mocker_db==0.1.1', 'cryptography'],
+    install_requires=['### parameterframe.py', 'pyyaml', 'pandas', 'attrs', 'sqlalchemy', 'cryptography', 'mocker_db==0.1.1', 'dill'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.2"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.", keywords="['python', 'parameter storage']", version="0.1.3"
 )
```

### Comparing `parameterframe-0.1.2/parameterframe.egg-info/PKG-INFO` & `parameterframe-0.1.3/parameterframe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parameterframe
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to manage parameters in a form of files, process them, upload to param storage, pull and reconstrut as files.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','parameter storage']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,18 +25,22 @@
 
 
 ```python
 import sys
 import pandas as pd
 import os
 sys.path.append('../')
-from parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
+from python_modules.parameterframe import ParameterFrame, MockerDatabaseConnector, SqlAlchemyDatabaseManager
 
 ```
 
+    /Users/insani_dei/miniconda3/envs/parameterframe/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html
+      from .autonotebook import tqdm as notebook_tqdm
+
+
 ## Content
 
 1. Adding new solution and uploading it
 2. Processing new files and creating parameter set
 3. Adding parameter set to solution and commiting
 4. Uploading parameter sets
 5. Getting latest parameter set id for solution
@@ -48,18 +52,20 @@
 ### 1. Adding new solution and uploading it
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
+when using SqlAlchemyDatabaseManager with database for the first time, it might be useful to create tables with `SqlAlchemyDatabaseManager.create_tables` and if schema of the database needs to be reset `SqlAlchemyDatabaseManager.drop_tables`
+
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
     database_connector = SqlAlchemyDatabaseManager(connection_details = {
     'base_url' : 'postgresql+psycopg2://postgres:mysecretpassword@localhost:5432/mytestdb'})
 )
@@ -204,14 +210,17 @@
 ```python
 pf.push_solution(
     # either solution id or solution name should be provided
     solution_name = "new_example_solution"
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
+
+
 
 
 
     True
 
 
 
@@ -223,15 +232,15 @@
 ```
 
 
 ```python
 pf = ParameterFrame(
     params_path = params_path,
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 pf = ParameterFrame(
     params_path = params_path,
@@ -312,27 +321,27 @@
 ```python
 pf.add_parameter_set_to_solution(
     solution_id = 'b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_name="test_set")
 ```
 
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca is not in solutions saved to memory!
-    Name pink_bright_toaster_706 is assigned to b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca temporarily!
+    Name pink_happy_car_642 is assigned to b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca temporarily!
 
 
 
 
 
     True
 
 
 
 
 ```python
-pf.commit_solution(solution_name="pink_bright_toaster_706",
+pf.commit_solution(solution_name="pink_happy_car_642",
                     parameter_set_names=["test_set"])
 ```
 
     Commited solution tables for b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca
 
 
 
@@ -431,15 +440,15 @@
   <tbody>
     <tr>
       <th>0</th>
       <td>a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5</td>
       <td>test_set</td>
       <td>example parameters for test purposes</td>
       <td>STAGING</td>
-      <td>2024-05-07 19:51:13</td>
+      <td>2024-05-15 00:09:10</td>
       <td>5</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
@@ -519,15 +528,15 @@
     <tr>
       <th>4</th>
       <td>1a4f19ee9e186ee739daecbc778501c5851d3fb5d05c4a3c1200e599855e8689</td>
       <td>param_21</td>
       <td></td>
       <td>param_21.ipynb</td>
       <td>other</td>
-      <td>4</td>
+      <td>2</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
@@ -535,29 +544,32 @@
 
 
 ```python
 pf.push_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                  parameter_set_names=["test_set"])
 ```
 
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
+
+
 
 
 
     True
 
 
 
 ### 5. Getting latest parameter set id for solution
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
@@ -568,42 +580,48 @@
 
 
 ```python
 pf.get_parameter_set_id_for_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                                                         deployment_status="STAGING")
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     ['a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5']
 
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'STAGING'
 
 
 
 ### 6. Changing parameter set status
 
 
 ```python
 # - with database connector for MockerDB
 pf = ParameterFrame(
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf = ParameterFrame(
@@ -618,38 +636,51 @@
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_ids = 'a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5',
     current_deployment_status = "PRODUCTION",
     new_deployment_status = "STAGING"
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
+
+
+    No deployed parameter_set_ids with PRODUCTION from selected!
 
 
 
-    True
+
+
+    False
 
 
 
 
 ```python
 pf.change_status_from_staging_to_production(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : STAGING -> PRODUCTION
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'PRODUCTION'
 
 
 
@@ -657,23 +688,29 @@
 ```python
 pf.change_status_from_production_to_archived(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : PRODUCTION -> ARCHIVED
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'ARCHIVED'
 
 
 
@@ -681,24 +718,34 @@
 ```python
 pf.change_status_from_archived_production(
     solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
     parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5'
 )
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
     No deployed parameter_set_ids with PRODUCTION from selected!
+
+
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/delete "HTTP/1.1 200 OK"
     b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca + a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5 : ARCHIVED -> PRODUCTION
+    HTTP Request: POST http://localhost:8001/insert "HTTP/1.1 200 OK"
 
 
 
 ```python
 pf.get_deployment_status(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                          parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
 
 
 
     'PRODUCTION'
 
 
 
@@ -711,15 +758,15 @@
 
 
 ```python
 # - with database connector for MockerDB
 pf2 = ParameterFrame(
     params_path = params_path,
     database_connector = MockerDatabaseConnector(connection_details = {
-    'base_url' : 'http://localhost:8000'})
+    'base_url' : 'http://localhost:8001'})
 )
 ```
 
 
 ```python
 # - with SqlAlchemy database connector
 pf2 = ParameterFrame(
@@ -767,35 +814,63 @@
   <tbody>
   </tbody>
 </table>
 </div>
 
 
 
+When pulling information with database handler, one could pull specific parameter sets, solutions and everything.
+
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    No data was found with applied filters!
+    No solutions with b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca could be pulled!
+
+
 
 
 
     True
 
 
 
 
 ```python
 pf2.pull_solution(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
                   # optionally specify parameter_set_id
                  parameter_set_id=None)
 ```
 
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
+    HTTP Request: POST http://localhost:8001/search "HTTP/1.1 200 OK"
+
+
+
+
+
+    True
+
+
+
+
+```python
+pf2.pull_solution()
+```
+
 
 
 
     True
 
 
 
@@ -833,31 +908,31 @@
       <th>maintainers</th>
       <th>commited_parameter_sets</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca</td>
+      <td>cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5</td>
       <td>new_example_solution</td>
       <td>Description of new example solution.</td>
       <td>2024-xx-xx</td>
       <td>None</td>
       <td>some text about maintainers credentials</td>
-      <td>1</td>
+      <td>2</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
 
 ```python
-pf2.show_parameter_sets(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca')
+pf2.show_parameter_sets(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5')
 ```
 
 
 
 
 <div>
 <style scoped>
@@ -884,31 +959,40 @@
       <th>insertion_datetime</th>
       <th>commited_parameters</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5</td>
-      <td>test_set</td>
-      <td>example parameters for test purposes</td>
-      <td>PRODUCTION</td>
-      <td>2024-05-07 19:51:13</td>
-      <td>5</td>
+      <td>3940d6dd4c0d817625a31141874c54cf0c8d88b24994f7915deb4096b3c8d0cf</td>
+      <td>blue_tiny_television_381</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 00:37:50</td>
+      <td>2</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5</td>
+      <td>yellow_shiny_microwave_931</td>
+      <td></td>
+      <td>STAGING</td>
+      <td>2024-05-15 00:36:04</td>
+      <td>3</td>
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
 
 ```python
-pf2.show_parameters(solution_id='b5c2e4a9bdcb57cc70bdb7310c7909cc1549550add79e3fbcc8aa1cf323cd8ca',
-                    parameter_set_id='a54f04d2ff154294309403206e059aec556cdcfa51120649ce663f3230a970d5')
+pf2.show_parameters(solution_id='cec89c4cbb8c891d388407ea93d84a5cd4f996af6d5c1b0cc5fe1cb12101acf5',
+                    parameter_set_id='5779bbf896ebb8f09a6ea252b09f8adb1a416e8780cf1424fb9bb93dbec8deb5')
 ```
 
 
 
 
 <div>
 <style scoped>
@@ -935,56 +1019,38 @@
       <th>file_type</th>
       <th>commited_attributes</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
-      <td>4cea5b09e77da310c5105978f2ceea5c5d8c9c7b65d0e00b45135ea90fc011af</td>
-      <td>param_1</td>
+      <td>3386ebc962b1c57745ca24320bf873df6eb84a2b9cb733607d72006347bf95b8</td>
+      <td>Screenshot 2024-05-04 at 02</td>
       <td></td>
-      <td>param_1.yaml</td>
-      <td>yaml</td>
-      <td>3</td>
+      <td>Screenshot 2024-05-04 at 02.59.31.png</td>
+      <td>other</td>
+      <td>35</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>bf11768decb1d0204e2636edd05c354573d473e67f1b048369b2ee99c865bf5f</td>
-      <td>param_2</td>
-      <td></td>
-      <td>param_2.yaml</td>
-      <td>yaml</td>
-      <td>6</td>
-    </tr>
-    <tr>
-      <th>2</th>
-      <td>9a4a3ace265c9bf2facc0044ca24260c42805c6e7b2a608dfd2f56a54d9d36be</td>
-      <td>param_10</td>
-      <td></td>
-      <td>param_10.txt</td>
-      <td>txt</td>
-      <td>9</td>
-    </tr>
-    <tr>
-      <th>3</th>
-      <td>ace2f31433212fbf9e764069a30a7675ca78f496d31f061d06d0a0420fc52768</td>
-      <td>param_11</td>
+      <td>4d8ca206d9bd09296b69a95f0c3c62d233282025964c356811510cc074cc2c49</td>
+      <td>1</td>
       <td></td>
-      <td>param_11.dill</td>
+      <td>1. AF - opis projektu.pdf</td>
       <td>other</td>
-      <td>1</td>
+      <td>34</td>
     </tr>
     <tr>
-      <th>4</th>
-      <td>1a4f19ee9e186ee739daecbc778501c5851d3fb5d05c4a3c1200e599855e8689</td>
-      <td>param_21</td>
+      <th>2</th>
+      <td>5afae3951544cd3736685a3b2daa31c00106191a799b96b0c636cd35e9a416ff</td>
+      <td>uploads</td>
       <td></td>
-      <td>param_21.ipynb</td>
+      <td>uploads.zip</td>
       <td>other</td>
-      <td>4</td>
+      <td>61</td>
     </tr>
   </tbody>
 </table>
 </div>
```

