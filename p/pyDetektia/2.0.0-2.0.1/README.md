# Comparing `tmp/pyDetektia-2.0.0.tar.gz` & `tmp/pyDetektia-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDetektia-2.0.0.tar", last modified: Fri Apr 19 13:26:08 2024, max compression
+gzip compressed data, was "pyDetektia-2.0.1.tar", last modified: Wed May 15 08:06:22 2024, max compression
```

## Comparing `pyDetektia-2.0.0.tar` & `pyDetektia-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-2.0.0/LICENSE.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-2.0.0/README.md
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/pyDetektia/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-2.0.0/pyDetektia/__init__.py
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    45611 2024-04-19 13:07:38.000000 pyDetektia-2.0.0/pyDetektia/manager.py
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/pyDetektia.egg-info/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/requires.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/top_level.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/setup.cfg
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2024-04-19 13:08:00.000000 pyDetektia-2.0.0/setup.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 08:06:22.000145 pyDetektia-2.0.1/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-2.0.1/LICENSE.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-15 08:06:22.000145 pyDetektia-2.0.1/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-2.0.1/README.md
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 08:06:21.996144 pyDetektia-2.0.1/pyDetektia/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-2.0.1/pyDetektia/__init__.py
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    45275 2024-04-30 13:13:23.000000 pyDetektia-2.0.1/pyDetektia/manager.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-05-15 08:06:22.000145 pyDetektia-2.0.1/pyDetektia.egg-info/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-05-15 08:06:21.000000 pyDetektia-2.0.1/pyDetektia.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2024-05-15 08:06:21.000000 pyDetektia-2.0.1/pyDetektia.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2024-05-15 08:06:21.000000 pyDetektia-2.0.1/pyDetektia.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2024-05-15 08:06:21.000000 pyDetektia-2.0.1/pyDetektia.egg-info/requires.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2024-05-15 08:06:21.000000 pyDetektia-2.0.1/pyDetektia.egg-info/top_level.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2024-05-15 08:06:22.000145 pyDetektia-2.0.1/setup.cfg
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2024-05-15 08:03:45.000000 pyDetektia-2.0.1/setup.py
```

### Comparing `pyDetektia-2.0.0/pyDetektia/manager.py` & `pyDetektia-2.0.1/pyDetektia/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self._role = self._get_user_role()
         self._organization = self._get_user_organization()
 
 
     def _get_token(self):
 
         ret = requests.post(
-            f"http://{self._ip}/auth/token",
+            f"{self._ip}/auth/token",
             data={
                 "username": self._user,
                 "password": self._password
             }
         )
         response = ret.json()
 
@@ -76,15 +76,15 @@
     
 
     def _get_user_role(self):
         '''
         Returns the role of the user.
         '''
 
-        url = f"http://{self._ip}/users/role"
+        url = f"{self._ip}/users/role"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
             
         jsonret = ret.json()
@@ -93,15 +93,15 @@
     
 
     def _get_user_organization(self):
         '''
         Returns user's organization.
         '''
 
-        url = f"http://{self._ip}/users/organization"
+        url = f"{self._ip}/users/organization"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
         
         jsonret = ret.json()
@@ -113,15 +113,15 @@
         '''
         Returns the datasetname of the given title and scenario.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/datasetname"
+        url = f"{self._ip}/organization/{organization}/datasetname"
         params = {
             "title": title,
             "scenario": scenario
         }
 
         ret = requests.get(url, params=params, headers=self._headers)
 
@@ -150,15 +150,15 @@
         '''
         Returns the id of the given layer.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/layer_id"
+        url = f"{self._ip}/organization/{organization}/polygons/layer_id"
         params = {
             "layer": layer,
             "scenario": scenario
         }
 
         ret = requests.get(url, params=params, headers=self._headers)
         
@@ -187,15 +187,15 @@
         '''
         Returns the ids of the polygons with the given names.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/geometry_ids"
+        url = f"{self._ip}/organization/{organization}/polygons/geometry_ids"
         params = {
             "layer_id": layer_id,
             "names": names
         }
 
         ret = requests.get(url, params=params, headers=self._headers)
 
@@ -227,15 +227,15 @@
         '''
         Returns a list of metadata dictionaries.
         '''
 
         if organization is None:
             organization = self._organization
         
-        url = f"http://{self._ip}/organization/{organization}/datasets"
+        url = f"{self._ip}/organization/{organization}/datasets"
 
         ret = requests.get(url, headers=self._headers)
         
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -277,15 +277,15 @@
         '''
         Returns a list of scenarios names.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url =  f"http://{self._ip}/organization/{organization}/datasets"
+        url = f"{self._ip}/organization/{organization}/datasets"
 
         ret = requests.get(url, headers=self._headers)
         
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -299,15 +299,15 @@
         '''
         Returns a list of dataset names.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/datasets"
+        url = f"{self._ip}/organization/{organization}/datasets"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -323,15 +323,15 @@
         '''
 
         if organization is None:
             organization = self._organization
             
         dataset = self._select_datasetname(dataset, title, scenario, organization)
         
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -360,15 +360,15 @@
         It is not necessary to include all the values, only the ones to be changed.
         If other different values are included, they will be ignored.
         """
         
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
 
         ret = requests.post(url, json=metadata, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.post(url, json=metadata, headers=self._headers)
 
         return {"status_code": ret.status_code, "detail": ret.json()}
@@ -383,15 +383,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
         
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/metadata"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -420,15 +420,15 @@
             params = {'date_span': (dates[0], dates[-1])}
         else:
             params = {'date_span': (date_span[0], date_span[1])}
 
         if polygon is not None:
             params['polygon'] = json.dumps(polygon)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}"
 
         ret = requests.get(url, headers=self._headers, params = params)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers, params = params)
 
         jsonret = ret.json()
@@ -473,15 +473,15 @@
         params = {}
         if polygon is not None:
             params['polygon'] = json.dumps(polygon)
 
         if extended:
             params['extended'] = extended
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}"
 
         ret = requests.get(url, headers=self._headers, params=params)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers, params=params)
 
         jsonret = ret.json()
@@ -495,15 +495,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}"
         if polygon is None:
             params = {}
         else:
             params = {'polygon': polygon}
 
         ret = requests.get(url, headers=self._headers, params=params)
 
@@ -524,15 +524,15 @@
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
         
         if len(ids) != 0:
-            url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/details"
+            url = f"{self._ip}/organization/{organization}/datasets/{dataset}/details"
             params = {"ids": ids}
 
             ret = requests.get(url, headers=self._headers, params=params)
 
             if self._check_status_code(ret, 200) == 1:
                 ret = requests.get(url, headers=self._headers, params=params)
 
@@ -552,15 +552,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/extended/{dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/extended/{dataset}/metadata"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -589,15 +589,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/extended"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/extended"
         params = {'key': key}
 
         ret = requests.get(url, params=params, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, params=params, headers=self._headers)
 
@@ -612,15 +612,15 @@
         '''
         Returns a list of polygons layers.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/layers"
+        url = f"{self._ip}/organization/{organization}/polygons/layers"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -635,15 +635,15 @@
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization)
         geom_ids = self._select_polygon_geometry_ids(geom_ids, names, layer_id, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/geometries/{layer_id}"
+        url = f"{self._ip}/organization/{organization}/polygons/geometries/{layer_id}"
         params = {}
         if polygon is not None:
             params['polygon'] = json.dumps(polygon)
         if len(geom_ids) != 0:
             params['geom_ids'] = geom_ids
 
         ret = requests.get(url, headers=self._headers, params=params)
@@ -666,15 +666,15 @@
             organization = self._organization
 
         if layer_id is None and layer is None and scenario is None:
             layer_id = None
         else:
             layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization=organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/metrics"
+        url = f"{self._ip}/organization/{organization}/polygons/metrics"
         params = {'layer_id': layer_id, 'type': type, 'metric': metric}
 
         ret = requests.get(url, headers=self._headers, params=params)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers, params=params)
 
@@ -687,15 +687,15 @@
         '''
         Returns the polygons metrics complete json, ready for uploading it to another database.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/metrics/{metric}"
+        url = f"{self._ip}/organization/{organization}/polygons/metrics/{metric}"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -709,15 +709,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization=organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/relations"
+        url = f"{self._ip}/organization/{organization}/polygons/relations"
         params = {}
         if metric is not None:
             params['metric'] = metric
         if layer_id is not None:
             params['layer_id'] = layer_id
 
         ret = requests.get(url, headers=self._headers, params=params)
@@ -737,15 +737,15 @@
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization=organization)
         geom_ids = self._select_polygon_geometry_ids(geom_ids, names, layer_id, organization)
         
-        url = f"http://{self._ip}/organization/{organization}/polygons/data/{layer_id}/{metric}"
+        url = f"{self._ip}/organization/{organization}/polygons/data/{layer_id}/{metric}"
         params = {'time_format': time_format}
         if len(geom_ids) != 0:
             params['geom_ids'] = geom_ids
         if polygon is not None:
             params['polygon'] = json.dumps(polygon)
         if date_span is not None:
             params['date_span'] = date_span
@@ -767,15 +767,15 @@
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization=organization)
         geom_ids = self._select_polygon_geometry_ids(geom_ids, names, layer_id, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/time_series/{layer_id}/{metric}"
+        url = f"{self._ip}/organization/{organization}/polygons/time_series/{layer_id}/{metric}"
         params = {'parent_process_dates': parent_process_dates, 'time_format': time_format}
         if len(geom_ids) != 0:
             params['geom_ids'] = geom_ids
         if polygon is not None:
             params['polygon'] = json.dumps(polygon)
         if date_span is not None:
             params['date_span'] = date_span
@@ -796,15 +796,15 @@
         '''
         Returns a list of scenarios names.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons"
+        url = f"{self._ip}/organization/{organization}/polygons"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -818,15 +818,15 @@
         '''
         Returns a list of the loaded polygons metadata in this organization and scenario.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons"
+        url = f"{self._ip}/organization/{organization}/polygons"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -840,15 +840,15 @@
         '''
         Returns a json object with the polygons and indices loaded in polygon_dataset.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/_polygons/{polygon_dataset}"
+        url = f"{self._ip}/organization/{organization}/_polygons/{polygon_dataset}"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -860,15 +860,15 @@
         '''
         Returns a json object with the polygons metadata loaded in polygon_dataset.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/_polygons/{polygon_dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/_polygons/{polygon_dataset}/metadata"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -880,15 +880,15 @@
         '''
         Returns a json object with all the polygons metadata.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/_polygons"
+        url = f"{self._ip}/organization/{organization}/_polygons"
 
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -900,15 +900,15 @@
         """
         Returns the indices metadata of polygon_dataset and organization
         """
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/indices/{polygon_dataset}/metadata"
+        url = f"{self._ip}/organization/{organization}/indices/{polygon_dataset}/metadata"
 
         params = {}
         if date_span is not None:
             params['date_span'] = (date_span[0], date_span[1])
             if index_types is not None:
                 params['index_types'] = index_types
         else:
@@ -954,15 +954,15 @@
                 'bbox': None
             }
 
             #--- loop over index types
             for index_type in index_types:
 
                 #--- query
-                url = f"http://{self._ip}/organization/{organization}/_polygons/{polygon_dataset}/details"
+                url = f"{self._ip}/organization/{organization}/_polygons/{polygon_dataset}/details"
                 params = {"ids": ids, "indices": list(index_dict[index_type].keys())}
 
                 ret = requests.get(url, headers=self._headers, params=params)
 
                 if self._check_status_code(ret, 200) == 1:
                     ret = requests.get(url, headers=self._headers, params=params)
 
@@ -994,15 +994,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/process"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/process"
         _json={
             "name": plugin_name,
             "data": parameters_dict
         }
 
         ret = requests.put(url, headers=self._headers, json=_json)
         
@@ -1070,15 +1070,15 @@
 
         if organization is None:
             organization = self._organization
 
         dataset_json['metadata']['title'] = title
         dataset_json['metadata']['scenario'] = scenario
         
-        url = f"http://{self._ip}/organization/{organization}/datasets"
+        url = f"{self._ip}/organization/{organization}/datasets"
 
         ret = requests.put(url, json=dataset_json, headers=self._headers)
 
         if  self._check_status_code(ret, 201) == 1:
             ret = requests.put(url, json=dataset_json, headers=self._headers)
 
         return ret.status_code
@@ -1090,15 +1090,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}"
 
         ret = requests.delete(url, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers)
 
         return ret.status_code
@@ -1112,15 +1112,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/datasets/{dataset}/extended"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/extended"
 
         ret = requests.patch(url, json=extended_dict, headers=self._headers)
         
         if self._check_status_code(ret, 200) == 1:
             ret = requests.patch(url, json=extended_dict, headers=self._headers)
 
         return ret.status_code
@@ -1132,15 +1132,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         dataset = self._select_datasetname(dataset, title, scenario, organization)
         
-        url =f"http://{self._ip}/organization/{organization}/datasets/{dataset}/extended"
+        url = f"{self._ip}/organization/{organization}/datasets/{dataset}/extended"
         params={'key': key}
 
         ret = requests.delete(url, params=params, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, params=params, headers=self._headers)
 
@@ -1155,15 +1155,15 @@
             - Table polygons_layer: if one of the polygons belongs to a new layer, it is created.
             - Table polygons_geometry: if one of the polygons is new, it is created.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/geometry"
+        url = f"{self._ip}/organization/{organization}/polygons/geometry"
 
         ret = requests.patch(url, json=geometries_json, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.patch(url, json=geometries_json, headers=self._headers)
 
         return {"status_code": ret.status_code, "detail": ret.json()}
@@ -1176,15 +1176,15 @@
             - Table polygons_data: if there is data for that metric and for an existing polygon, rows are added.
             - Table polygons_relation: if data is added to polygons_data table, rows are added.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/metric"
+        url = f"{self._ip}/organization/{organization}/polygons/metric"
 
         ret = requests.patch(url, json=metrics_json, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.patch(url, json=metrics_json, headers=self._headers)
 
         return {"status_code": ret.status_code, "detail": ret.json()}
@@ -1196,15 +1196,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/layer/{layer_id}"
+        url = f"{self._ip}/organization/{organization}/polygons/layer/{layer_id}"
 
         ret = requests.delete(url, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers)
 
         return ret.status_code
@@ -1216,15 +1216,15 @@
         """
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/geometries/{layer_id}"
+        url = f"{self._ip}/organization/{organization}/polygons/geometries/{layer_id}"
         _json = geom_ids
 
         ret = requests.delete(url, headers=self._headers, json=_json)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers, json=_json)
         
@@ -1235,15 +1235,15 @@
         '''
         This method deletes the polygons metric with name 'metric', together with its data and polygons_relation table rows.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/metric/{metric}"
+        url = f"{self._ip}/organization/{organization}/polygons/metric/{metric}"
 
         ret = requests.delete(url, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers)
 
         return ret.status_code
@@ -1255,15 +1255,15 @@
         '''
 
         if organization is None:
             organization = self._organization
 
         layer_id = self._select_polygon_layer_id(layer_id, layer, scenario, organization)
 
-        url = f"http://{self._ip}/organization/{organization}/polygons/data"
+        url = f"{self._ip}/organization/{organization}/polygons/data"
         json_data = {"ids": ids, "data_ids": data_ids, "geom_ids": geom_ids, "layer_id": layer_id, "metric": metric}
 
         ret = requests.delete(url, headers=self._headers, json=json_data)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers, json=json_data)
 
@@ -1276,15 +1276,15 @@
         '''
         This method adds polygons to the dataset with name dataset_name.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/_polygons/{polygons_dataset}"
+        url = f"{self._ip}/organization/{organization}/_polygons/{polygons_dataset}"
         polygons_json = self._reformat_polygons(polygons_json)
 
         ret = requests.put(url, json=polygons_json, headers=self._headers)
 
         if self._check_status_code(ret, 201) == 1:
             ret = requests.put(url, json=polygons_json, headers=self._headers)
 
@@ -1295,15 +1295,15 @@
         '''
         This method delete polygons of dataset with name polygons_dataset.
         '''
 
         if organization is None:
             organization = self._organization
 
-        url = f"http://{self._ip}/organization/{organization}/_polygons/{polygons_dataset}"
+        url = f"{self._ip}/organization/{organization}/_polygons/{polygons_dataset}"
 
         ret = requests.delete(url, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers)
 
         return ret.status_code
@@ -1337,15 +1337,15 @@
     #--------------------#
     #--- manage users ---#
     def get_users_info(self):
         '''
         Returns a list of dictionaries. Each dictionary has the information.
         '''
 
-        url = f"http://{self._ip}/users"
+        url = f"{self._ip}/users"
         
         ret = requests.get(url, headers=self._headers)
 
         if self._check_status_code(ret, 200) == 1:
             ret = requests.get(url, headers=self._headers)
 
         jsonret = ret.json()
@@ -1370,15 +1370,15 @@
         This mehotd creates a new user.
         '''
 
         is_admin = "TRUE" if _is_admin else "FALSE" 
         root = "TRUE" if _root else "FALSE"
         email = e_mail or f"{new_user}@detektia.com"
 
-        url = f"http://{self._ip}/users"
+        url = f"{self._ip}/users"
         _json = {
             "organization": organization,
             "name": new_user,
             "password": new_pwd,
             "email": email,
             "is_admin": is_admin,
             "root": root
@@ -1393,15 +1393,15 @@
 
 
     def delete_user(self, user_to_delete):
         '''
         This mehotd deletes user.
         '''
 
-        url = f"http://{self._ip}/users/{user_to_delete}"
+        url = f"{self._ip}/users/{user_to_delete}"
 
         ret = requests.delete(url, headers=self._headers)
 
         if self._check_status_code(ret, 204) == 1:
             ret = requests.delete(url, headers=self._headers)
 
         return ret.status_code
```

