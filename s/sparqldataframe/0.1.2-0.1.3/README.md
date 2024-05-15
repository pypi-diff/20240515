# Comparing `tmp/sparqldataframe-0.1.2.tar.gz` & `tmp/sparqldataframe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparqldataframe-0.1.2.tar", last modified: Sat Jul 29 12:05:09 2023, max compression
+gzip compressed data, was "sparqldataframe-0.1.3.tar", last modified: Wed May 15 14:19:51 2024, max compression
```

## Comparing `sparqldataframe-0.1.2.tar` & `sparqldataframe-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1073 2023-07-26 15:02:34.000000 sparqldataframe-0.1.2/LICENSE
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/PKG-INFO
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1351 2023-07-29 11:51:46.000000 sparqldataframe-0.1.2/README.md
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       38 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/setup.cfg
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2294 2023-07-29 11:25:59.000000 sparqldataframe-0.1.2/setup.py
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/sparqldataframe/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1875 2023-07-29 12:03:10.000000 sparqldataframe-0.1.2/sparqldataframe/__init__.py
-drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2023-07-29 12:05:09.366138 sparqldataframe-0.1.2/sparqldataframe.egg-info/
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2023-07-29 12:05:08.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/PKG-INFO
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)      248 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/SOURCES.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)        1 2023-07-29 12:05:08.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/dependency_links.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       27 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/requires.txt
--rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       16 2023-07-29 12:05:09.000000 sparqldataframe-0.1.2/sparqldataframe.egg-info/top_level.txt
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2024-05-15 14:19:51.455741 sparqldataframe-0.1.3/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1073 2023-07-26 15:02:34.000000 sparqldataframe-0.1.3/LICENSE
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2024-05-15 14:19:51.455741 sparqldataframe-0.1.3/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     1351 2023-07-29 11:51:46.000000 sparqldataframe-0.1.3/README.md
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       38 2024-05-15 14:19:51.455741 sparqldataframe-0.1.3/setup.cfg
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2294 2023-07-29 11:25:59.000000 sparqldataframe-0.1.3/setup.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2024-05-15 14:19:51.455741 sparqldataframe-0.1.3/sparqldataframe/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2078 2024-05-15 14:17:21.000000 sparqldataframe-0.1.3/sparqldataframe/__init__.py
+drwxrwxr-x   0 nikolai   (1000) nikolai   (1000)        0 2024-05-15 14:19:51.455741 sparqldataframe-0.1.3/sparqldataframe.egg-info/
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)     2357 2024-05-15 14:19:50.000000 sparqldataframe-0.1.3/sparqldataframe.egg-info/PKG-INFO
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)      248 2024-05-15 14:19:51.000000 sparqldataframe-0.1.3/sparqldataframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)        1 2024-05-15 14:19:50.000000 sparqldataframe-0.1.3/sparqldataframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       27 2024-05-15 14:19:51.000000 sparqldataframe-0.1.3/sparqldataframe.egg-info/requires.txt
+-rw-rw-r--   0 nikolai   (1000) nikolai   (1000)       16 2024-05-15 14:19:51.000000 sparqldataframe-0.1.3/sparqldataframe.egg-info/top_level.txt
```

### Comparing `sparqldataframe-0.1.2/LICENSE` & `sparqldataframe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparqldataframe-0.1.2/PKG-INFO` & `sparqldataframe-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
```

### Comparing `sparqldataframe-0.1.2/README.md` & `sparqldataframe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sparqldataframe-0.1.2/setup.py` & `sparqldataframe-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sparqldataframe-0.1.2/sparqldataframe/__init__.py` & `sparqldataframe-0.1.3/sparqldataframe/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
+import requests
 import pandas as pd
+from typing import Optional, Dict, Any
 from simplejson import JSONDecodeError
-import requests
-
 
 DEFAULT_PREFIXES = """
 PREFIX foaf: <http://xmlns.com/foaf/0.1/>
 PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
 PREFIX owl: <http://www.w3.org/2002/07/owl#>
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
@@ -22,37 +22,42 @@
 PREFIX p: <http://www.wikidata.org/prop/>
 PREFIX ps: <http://www.wikidata.org/prop/statement/>
 PREFIX pq: <http://www.wikidata.org/prop/qualifier/>
 PREFIX bd: <http://www.bigdata.com/rdf#>
 """
 
 
-def dbpedia_query(sparql_query):
+def dbpedia_query(sparql_query: str):
     url = 'http://dbpedia.org/sparql'
     return query(url, DEFAULT_PREFIXES + sparql_query)
 
 
-def wikidata_query(sparql_query):
+def wikidata_query(sparql_query: str):
     url = 'https://query.wikidata.org/sparql'
     return query(url, DEFAULT_PREFIXES + sparql_query)
 
 
-def query(url, sparql_query):
+def query(url: str, sparql_query: str, headers: Optional[Dict[str, str]] = None):
+    default_headers = {
+        "accept": "application/sparql-results+json"
+    }
+    if headers:
+        default_headers.update(headers)
+
     try:
         r = requests.get(
             url,
             params={
                 'format': 'json',
                 'query': sparql_query
             },
-            headers={
-                "accept": "application/sparql-results+json"
-            })
+            headers=default_headers)
+        r.raise_for_status()
         data = r.json()
-    except JSONDecodeError as e:
+    except JSONDecodeError:
         print(r.content)
         raise Exception('Invalid query')
 
     if ('results' in data) and ('bindings' in data['results']):
         columns = data['head']['vars']
         rows = [[binding[col]['value'] if col in binding else None
                 for col in columns]
```

### Comparing `sparqldataframe-0.1.2/sparqldataframe.egg-info/PKG-INFO` & `sparqldataframe-0.1.3/sparqldataframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparqldataframe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Get a Pandas dataframe from SPARQL queries
 Home-page: https://github.com/njanakiev/sparqldataframe
 Author: Nikolai Janakiev
 Author-email: nikolai.janakiev@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Console
```

