# Comparing `tmp/pypdb-2.3.tar.gz` & `tmp/pypdb-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdb-2.3.tar", last modified: Mon Jul 24 02:29:43 2023, max compression
+gzip compressed data, was "pypdb-2.4.tar", last modified: Wed May 15 13:54:35 2024, max compression
```

## Comparing `pypdb-2.3.tar` & `pypdb-2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608676 pypdb-2.3/
--rwxrwxrwx   0 william    (503) staff       (20)     1082 2015-05-13 05:20:06.000000 pypdb-2.3/LICENSE
--rw-r--r--   0 william    (503) staff       (20)      351 2023-07-24 02:29:43.608725 pypdb-2.3/PKG-INFO
--rwxr-xr-x   0 william    (503) staff       (20)     2578 2023-07-24 02:23:45.000000 pypdb-2.3/README.md
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.603598 pypdb-2.3/pypdb/
--rwxrwxrwx   0 william    (503) staff       (20)       49 2020-11-11 23:44:19.000000 pypdb-2.3/pypdb/__init__.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604457 pypdb-2.3/pypdb/clients/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/__init__.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604750 pypdb-2.3/pypdb/clients/data/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/data/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     6236 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/data_types.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.605063 pypdb-2.3/pypdb/clients/data/graphql/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/data/graphql/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     1126 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/graphql/graphql.py
--rw-r--r--   0 william    (503) staff       (20)      976 2023-07-15 03:42:36.000000 pypdb-2.3/pypdb/clients/data/graphql/test_graphql.py
--rw-r--r--   0 william    (503) staff       (20)     3980 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/clients/data/test_data_types.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.605599 pypdb-2.3/pypdb/clients/fasta/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/fasta/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     2825 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/fasta/fasta_client.py
--rw-r--r--   0 william    (503) staff       (20)     2527 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/fasta/fasta_client_test.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.606067 pypdb-2.3/pypdb/clients/pdb/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     2706 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/pdb_client.py
--rw-r--r--   0 william    (503) staff       (20)     3703 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/pdb/pdb_client_test.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.606458 pypdb-2.3/pypdb/clients/search/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/__init__.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.607977 pypdb-2.3/pypdb/clients/search/operators/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-07-15 03:42:36.000000 pypdb-2.3/pypdb/clients/search/operators/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     1555 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/chemical_operators.py
--rw-r--r--   0 william    (503) staff       (20)     1499 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/chemical_operators_test.py
--rw-r--r--   0 william    (503) staff       (20)      907 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators.py
--rw-r--r--   0 william    (503) staff       (20)      746 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators_test.py
--rw-r--r--   0 william    (503) staff       (20)     2443 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/sequence_operators.py
--rw-r--r--   0 william    (503) staff       (20)     1480 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/sequence_operators_test.py
--rw-r--r--   0 william    (503) staff       (20)     1140 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/structure_operators.py
--rw-r--r--   0 william    (503) staff       (20)     1216 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/structure_operators_test.py
--rw-r--r--   0 william    (503) staff       (20)     5901 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/search/operators/text_operators.py
--rw-r--r--   0 william    (503) staff       (20)      764 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/operators/text_operators_test.py
--rw-r--r--   0 william    (503) staff       (20)    12663 2023-06-12 21:14:50.000000 pypdb-2.3/pypdb/clients/search/search_client.py
--rw-r--r--   0 william    (503) staff       (20)    21180 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/clients/search/search_client_test.py
--rw-r--r--   0 william    (503) staff       (20)       57 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/conftest.py
--rwxr-xr-x   0 william    (503) staff       (20)    34307 2023-07-24 02:12:08.000000 pypdb-2.3/pypdb/pypdb.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608329 pypdb-2.3/pypdb/util/
--rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/__init__.py
--rw-r--r--   0 william    (503) staff       (20)     1892 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/http_requests.py
--rw-r--r--   0 william    (503) staff       (20)     4165 2023-06-12 21:14:45.000000 pypdb-2.3/pypdb/util/test_http_requests.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604210 pypdb-2.3/pypdb.egg-info/
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.604319 pypdb-2.3/pypdb.egg-info/.ipynb_checkpoints/
--rwxrwxrwx   0 william    (503) staff       (20)        1 2020-11-15 12:06:33.000000 pypdb-2.3/pypdb.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rwxrwxrwx   0 william    (503) staff       (20)      351 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/PKG-INFO
--rwxrwxrwx   0 william    (503) staff       (20)     1563 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/SOURCES.txt
--rwxrwxrwx   0 william    (503) staff       (20)        1 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/dependency_links.txt
--rwxrwxrwx   0 william    (503) staff       (20)       16 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/requires.txt
--rwxrwxrwx   0 william    (503) staff       (20)        6 2023-07-24 02:29:43.000000 pypdb-2.3/pypdb.egg-info/top_level.txt
--rwxrwxrwx   0 william    (503) staff       (20)       79 2023-07-24 02:29:43.608904 pypdb-2.3/setup.cfg
--rwxr-xr-x   0 william    (503) staff       (20)      793 2023-07-24 02:28:39.000000 pypdb-2.3/setup.py
-drwxr-xr-x   0 william    (503) staff       (20)        0 2023-07-24 02:29:43.608467 pypdb-2.3/tests/
--rw-r--r--   0 william    (503) staff       (20)     2397 2023-07-15 05:37:14.000000 pypdb-2.3/tests/test_pypdb.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.325843 pypdb-2.4/
+-rwxrwxrwx   0 william    (503) staff       (20)     1082 2015-05-13 05:20:06.000000 pypdb-2.4/LICENSE
+-rw-r--r--   0 william    (503) staff       (20)     2994 2024-05-15 13:54:35.325785 pypdb-2.4/PKG-INFO
+-rwxr-xr-x   0 william    (503) staff       (20)     2578 2023-07-24 02:23:45.000000 pypdb-2.4/README.md
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.319626 pypdb-2.4/pypdb/
+-rwxrwxrwx   0 william    (503) staff       (20)       49 2020-11-11 23:44:19.000000 pypdb-2.4/pypdb/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.320843 pypdb-2.4/pypdb/clients/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.321185 pypdb-2.4/pypdb/clients/data/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/data/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     6189 2024-05-15 13:50:42.000000 pypdb-2.4/pypdb/clients/data/data_types.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.321594 pypdb-2.4/pypdb/clients/data/graphql/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/data/graphql/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1126 2023-07-24 02:12:08.000000 pypdb-2.4/pypdb/clients/data/graphql/graphql.py
+-rw-r--r--   0 william    (503) staff       (20)      976 2023-07-15 03:42:36.000000 pypdb-2.4/pypdb/clients/data/graphql/test_graphql.py
+-rw-r--r--   0 william    (503) staff       (20)     3980 2023-07-24 02:12:08.000000 pypdb-2.4/pypdb/clients/data/test_data_types.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.322160 pypdb-2.4/pypdb/clients/fasta/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/fasta/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     2825 2023-06-12 21:14:50.000000 pypdb-2.4/pypdb/clients/fasta/fasta_client.py
+-rw-r--r--   0 william    (503) staff       (20)     2527 2023-06-12 21:14:50.000000 pypdb-2.4/pypdb/clients/fasta/fasta_client_test.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.322744 pypdb-2.4/pypdb/clients/pdb/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/pdb/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     2706 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/pdb/pdb_client.py
+-rw-r--r--   0 william    (503) staff       (20)     3703 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/pdb/pdb_client_test.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.323165 pypdb-2.4/pypdb/clients/search/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/__init__.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.324819 pypdb-2.4/pypdb/clients/search/operators/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-07-15 03:42:36.000000 pypdb-2.4/pypdb/clients/search/operators/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1555 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/chemical_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1499 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/chemical_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)      907 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/seqmotif_operators.py
+-rw-r--r--   0 william    (503) staff       (20)      746 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/seqmotif_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     2443 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/sequence_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1480 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/sequence_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     1140 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/structure_operators.py
+-rw-r--r--   0 william    (503) staff       (20)     1216 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/structure_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)     5901 2023-06-12 21:14:50.000000 pypdb-2.4/pypdb/clients/search/operators/text_operators.py
+-rw-r--r--   0 william    (503) staff       (20)      764 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/operators/text_operators_test.py
+-rw-r--r--   0 william    (503) staff       (20)    12699 2023-10-19 18:18:09.000000 pypdb-2.4/pypdb/clients/search/search_client.py
+-rw-r--r--   0 william    (503) staff       (20)    21180 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/clients/search/search_client_test.py
+-rw-r--r--   0 william    (503) staff       (20)       57 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/conftest.py
+-rwxr-xr-x   0 william    (503) staff       (20)    34307 2023-07-24 02:12:08.000000 pypdb-2.4/pypdb/pypdb.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.325176 pypdb-2.4/pypdb/util/
+-rw-r--r--   0 william    (503) staff       (20)        0 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/util/__init__.py
+-rw-r--r--   0 william    (503) staff       (20)     1892 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/util/http_requests.py
+-rw-r--r--   0 william    (503) staff       (20)     4165 2023-06-12 21:14:45.000000 pypdb-2.4/pypdb/util/test_http_requests.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.325601 pypdb-2.4/pypdb.egg-info/
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.320698 pypdb-2.4/pypdb.egg-info/.ipynb_checkpoints/
+-rwxrwxrwx   0 william    (503) staff       (20)        1 2020-11-15 12:06:33.000000 pypdb-2.4/pypdb.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 william    (503) staff       (20)     2994 2024-05-15 13:54:35.000000 pypdb-2.4/pypdb.egg-info/PKG-INFO
+-rwxrwxrwx   0 william    (503) staff       (20)     1563 2024-05-15 13:54:35.000000 pypdb-2.4/pypdb.egg-info/SOURCES.txt
+-rwxrwxrwx   0 william    (503) staff       (20)        1 2024-05-15 13:54:35.000000 pypdb-2.4/pypdb.egg-info/dependency_links.txt
+-rwxrwxrwx   0 william    (503) staff       (20)        9 2024-05-15 13:54:35.000000 pypdb-2.4/pypdb.egg-info/requires.txt
+-rwxrwxrwx   0 william    (503) staff       (20)        6 2024-05-15 13:54:35.000000 pypdb-2.4/pypdb.egg-info/top_level.txt
+-rwxrwxrwx   0 william    (503) staff       (20)       79 2024-05-15 13:54:35.326116 pypdb-2.4/setup.cfg
+-rwxr-xr-x   0 william    (503) staff       (20)     1117 2024-05-15 13:52:56.000000 pypdb-2.4/setup.py
+drwxr-xr-x   0 william    (503) staff       (20)        0 2024-05-15 13:54:35.325329 pypdb-2.4/tests/
+-rw-r--r--   0 william    (503) staff       (20)     2397 2023-07-15 05:37:14.000000 pypdb-2.4/tests/test_pypdb.py
```

### Comparing `pypdb-2.3/LICENSE` & `pypdb-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/README.md` & `pypdb-2.4/README.md`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/data/data_types.py` & `pypdb-2.4/pypdb/clients/data/data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 - chemical component
 (currently not implemented:)
 - PubMed integrated data
 - UniProt integrated data
 - DrugBank integrated data
 """
 from dataclasses import dataclass, field
-import pandas as pd
 from enum import Enum
 
 #TODO: handle batch requests
 
 from pypdb.clients.data.graphql.graphql import search_graphql
 
 class DataType(Enum):
@@ -158,17 +157,17 @@
             return
 
         self.response = response
 
         if len(self.response['data'][self.data_type.value]) != len(self.id):
             print("WARNING: one or more IDs not found in the PDB.")
 
-    def return_data_as_pandas_df(self):
+    def return_data_as_df_dict(self):
         """
-        Return the fetched data as a pandas dataframe.
+        Return the fetched data as a dict usable by pandas or polars.
         """
         if not self.response:
             return None
 
         data = self.response['data'][self.data_type.value]
 
         # flatten data dictionary by joining property and subproperty names
@@ -186,8 +185,8 @@
                     curr_dict[new_key] = v
                 else:
                     for subprop, val in v.items():
                         new_key = f"{key}.{subprop}"
                         curr_dict[new_key] = val
             data_flat[id] = curr_dict
 
-        return pd.DataFrame.from_dict(data_flat, orient='index')
+        return data_flat
```

### Comparing `pypdb-2.3/pypdb/clients/data/graphql/graphql.py` & `pypdb-2.4/pypdb/clients/data/graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/data/graphql/test_graphql.py` & `pypdb-2.4/pypdb/clients/data/graphql/test_graphql.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/data/test_data_types.py` & `pypdb-2.4/pypdb/clients/data/test_data_types.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/fasta/fasta_client.py` & `pypdb-2.4/pypdb/clients/fasta/fasta_client.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/fasta/fasta_client_test.py` & `pypdb-2.4/pypdb/clients/fasta/fasta_client_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/pdb/pdb_client.py` & `pypdb-2.4/pypdb/clients/pdb/pdb_client.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/pdb/pdb_client_test.py` & `pypdb-2.4/pypdb/clients/pdb/pdb_client_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/chemical_operators.py` & `pypdb-2.4/pypdb/clients/search/operators/chemical_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/chemical_operators_test.py` & `pypdb-2.4/pypdb/clients/search/operators/chemical_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators.py` & `pypdb-2.4/pypdb/clients/search/operators/seqmotif_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/seqmotif_operators_test.py` & `pypdb-2.4/pypdb/clients/search/operators/seqmotif_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/sequence_operators.py` & `pypdb-2.4/pypdb/clients/search/operators/sequence_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/sequence_operators_test.py` & `pypdb-2.4/pypdb/clients/search/operators/sequence_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/structure_operators.py` & `pypdb-2.4/pypdb/clients/search/operators/structure_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/structure_operators_test.py` & `pypdb-2.4/pypdb/clients/search/operators/structure_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/text_operators.py` & `pypdb-2.4/pypdb/clients/search/operators/text_operators.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/operators/text_operators_test.py` & `pypdb-2.4/pypdb/clients/search/operators/text_operators_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/clients/search/search_client.py` & `pypdb-2.4/pypdb/clients/search/search_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,15 @@
         If `return_with_scores=True`, returns a list of ScoredResult instead.
         If `return_raw_json_dict=True`, returns the raw JSON response from RCSB.
     """
 
     if type(query_object) in _SEARCH_OPERATORS:
         cast_query_object = _QueryNode(query_object)  # type: ignore
     else:
+        # print(type(query_object))
         cast_query_object = query_object  # type: ignore
 
     if request_options is not None:
         request_options_dict = request_options._to_dict()
     else:
         request_options_dict = {'return_all_hits': True}
```

### Comparing `pypdb-2.3/pypdb/clients/search/search_client_test.py` & `pypdb-2.4/pypdb/clients/search/search_client_test.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/pypdb.py` & `pypdb-2.4/pypdb/pypdb.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/util/http_requests.py` & `pypdb-2.4/pypdb/util/http_requests.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb/util/test_http_requests.py` & `pypdb-2.4/pypdb/util/test_http_requests.py`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/pypdb.egg-info/SOURCES.txt` & `pypdb-2.4/pypdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypdb-2.3/tests/test_pypdb.py` & `pypdb-2.4/tests/test_pypdb.py`

 * *Files identical despite different names*

