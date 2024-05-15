# Comparing `tmp/timescale-vector-0.0.4.tar.gz` & `tmp/timescale-vector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timescale-vector-0.0.4.tar", last modified: Thu Nov 30 22:16:29 2023, max compression
+gzip compressed data, was "timescale-vector-0.0.5.tar", last modified: Wed May 15 20:01:40 2024, max compression
```

## Comparing `timescale-vector-0.0.4.tar` & `timescale-vector-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 cevian     (501) staff       (20)        0 2023-11-30 22:16:29.760171 timescale-vector-0.0.4/
--rw-rw-r--   0 cevian     (501) staff       (20)    11337 2023-04-27 10:12:58.000000 timescale-vector-0.0.4/LICENSE
--rw-rw-r--   0 cevian     (501) staff       (20)      111 2023-04-27 10:12:58.000000 timescale-vector-0.0.4/MANIFEST.in
--rw-r--r--   0 cevian     (501) staff       (20)      639 2023-09-14 17:01:33.000000 timescale-vector-0.0.4/NOTICE
--rw-r--r--   0 cevian     (501) staff       (20)    37639 2023-11-30 22:16:29.759984 timescale-vector-0.0.4/PKG-INFO
--rw-r--r--   0 cevian     (501) staff       (20)    36818 2023-11-30 19:01:28.000000 timescale-vector-0.0.4/README.md
--rw-r--r--   0 cevian     (501) staff       (20)      928 2023-10-31 19:21:11.000000 timescale-vector-0.0.4/settings.ini
--rw-r--r--   0 cevian     (501) staff       (20)       38 2023-11-30 22:16:29.760216 timescale-vector-0.0.4/setup.cfg
--rw-rw-r--   0 cevian     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 timescale-vector-0.0.4/setup.py
-drwxr-xr-x   0 cevian     (501) staff       (20)        0 2023-11-30 22:16:29.757881 timescale-vector-0.0.4/timescale_vector/
--rw-r--r--   0 cevian     (501) staff       (20)       22 2023-11-20 17:25:28.000000 timescale-vector-0.0.4/timescale_vector/__init__.py
--rw-r--r--   0 cevian     (501) staff       (20)    23933 2023-11-30 18:53:11.000000 timescale-vector-0.0.4/timescale_vector/_modidx.py
--rw-r--r--   0 cevian     (501) staff       (20)    50390 2023-11-30 18:54:10.000000 timescale-vector-0.0.4/timescale_vector/client.py
--rw-r--r--   0 cevian     (501) staff       (20)     5310 2023-11-20 17:25:28.000000 timescale-vector-0.0.4/timescale_vector/pgvectorizer.py
-drwxr-xr-x   0 cevian     (501) staff       (20)        0 2023-11-30 22:16:29.759650 timescale-vector-0.0.4/timescale_vector.egg-info/
--rw-r--r--   0 cevian     (501) staff       (20)    37639 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/PKG-INFO
--rw-r--r--   0 cevian     (501) staff       (20)      456 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/SOURCES.txt
--rw-r--r--   0 cevian     (501) staff       (20)        1 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/dependency_links.txt
--rw-r--r--   0 cevian     (501) staff       (20)       54 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/entry_points.txt
--rw-r--r--   0 cevian     (501) staff       (20)        1 2023-08-16 16:50:55.000000 timescale-vector-0.0.4/timescale_vector.egg-info/not-zip-safe
--rw-r--r--   0 cevian     (501) staff       (20)       57 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/requires.txt
--rw-r--r--   0 cevian     (501) staff       (20)       17 2023-11-30 22:16:29.000000 timescale-vector-0.0.4/timescale_vector.egg-info/top_level.txt
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-15 20:01:40.149875 timescale-vector-0.0.5/
+-rw-r--r--   0 john       (501) staff       (20)    11337 2023-10-18 21:18:47.000000 timescale-vector-0.0.5/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)      111 2023-10-18 21:18:47.000000 timescale-vector-0.0.5/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)      639 2023-10-18 21:18:47.000000 timescale-vector-0.0.5/NOTICE
+-rw-r--r--   0 john       (501) staff       (20)    38374 2024-05-15 20:01:40.149551 timescale-vector-0.0.5/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)    37348 2024-05-15 19:50:14.000000 timescale-vector-0.0.5/README.md
+-rw-r--r--   0 john       (501) staff       (20)      945 2024-05-15 19:54:08.000000 timescale-vector-0.0.5/settings.ini
+-rw-r--r--   0 john       (501) staff       (20)       38 2024-05-15 20:01:40.149935 timescale-vector-0.0.5/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     2596 2023-10-18 21:18:47.000000 timescale-vector-0.0.5/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-15 20:01:40.147669 timescale-vector-0.0.5/timescale_vector/
+-rw-r--r--   0 john       (501) staff       (20)       22 2024-05-15 19:49:42.000000 timescale-vector-0.0.5/timescale_vector/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    23933 2024-05-15 19:49:42.000000 timescale-vector-0.0.5/timescale_vector/_modidx.py
+-rw-r--r--   0 john       (501) staff       (20)    51080 2024-05-15 19:49:42.000000 timescale-vector-0.0.5/timescale_vector/client.py
+-rw-r--r--   0 john       (501) staff       (20)     5310 2024-05-15 19:49:42.000000 timescale-vector-0.0.5/timescale_vector/pgvectorizer.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2024-05-15 20:01:40.149088 timescale-vector-0.0.5/timescale_vector.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)    38374 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      456 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       54 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2024-04-08 18:37:53.000000 timescale-vector-0.0.5/timescale_vector.egg-info/not-zip-safe
+-rw-r--r--   0 john       (501) staff       (20)       74 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       17 2024-05-15 20:01:40.000000 timescale-vector-0.0.5/timescale_vector.egg-info/top_level.txt
```

### Comparing `timescale-vector-0.0.4/LICENSE` & `timescale-vector-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timescale-vector-0.0.4/NOTICE` & `timescale-vector-0.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `timescale-vector-0.0.4/PKG-INFO` & `timescale-vector-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-Metadata-Version: 2.1
-Name: timescale-vector
-Version: 0.0.4
-Summary: Python library for storing vector data in Postgres
-Home-page: https://github.com/timescale/python-vector
-Author: Matvey Arye
-Author-email: mat@timescale.com
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-License-File: NOTICE
-
 # Timescale Vector
 
+
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 PostgreSQL++ for AI Applications.
 
 - [Signup for Timescale
   Vector](https://console.cloud.timescale.com/signup?utm_campaign=vectorlaunch&utm_source=github&utm_medium=direct):
   Get 90 days free to try Timescale Vector on the Timescale cloud data
@@ -58,14 +36,24 @@
 We also use `dotenv` in our examples for passing around secrets and
 keys. You can install that with:
 
 ``` sh
 pip install python-dotenv
 ```
 
+If you run into installation errors related to the psycopg2 package, you
+will need to install some prerequisites. The timescale-vector package
+explicitly depends on psycopg2 (the non-binary version). This adheres to
+[the advice provided by
+psycopg2](https://www.psycopg.org/docs/install.html#psycopg-vs-psycopg-binary).
+Building psycopg from source [requires a few prerequisites to be
+installed](https://www.psycopg.org/docs/install.html#build-prerequisites).
+Make sure these are installed before trying to
+`pip install timescale_vector`.
+
 ## Basic usage
 
 First, import all the necessary libraries:
 
 ``` python
 from dotenv import load_dotenv, find_dotenv
 import os
@@ -128,20 +116,20 @@
 
 Now, you can query for similar items:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('73d05d6e-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('45ecb350-0f15-11ef-8d89-e666703872d0'),
       {'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 There are many search options which we will cover below in the
 `Advanced search` section.
@@ -149,15 +137,15 @@
 As one example, we will return one item using a similarity search
 constrained by a metadata filter.
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The returned records contain 5 fields:
 
@@ -173,15 +161,15 @@
 keyed on the field name:
 
 ``` python
 records = vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 (records[0]["id"],records[0]["metadata"], records[0]["contents"], records[0]["embedding"], records[0]["distance"])
 ```
 
-    (UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    (UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
      {'action': 'jump', 'animal': 'fox'},
      'jumped over the',
      array([ 1. , 10.8], dtype=float32),
      0.00016793422934946456)
 
 You can delete by ID:
 
@@ -236,32 +224,32 @@
 
 The basic query looks like:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You could provide a limit for the number of items returned:
 
 ``` python
 vec.search([1.0, 9.0], limit=1)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Narrowing your search by metadata
 
@@ -278,48 +266,48 @@
 have to match the provided values (keys not in the filter are
 unconstrained):
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "sit"})
 ```
 
-    [[UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You can also specify a list of filter dictionaries, where an item is
 returned if it matches any dict:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, filter=[{"action": "jump"}, {"animal": "fox"}])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ##### Predicates
 
 Predicates allow for more complex search conditions. For example, you
 could use greater than and less than conditions on numeric values.
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates)
 objects are defined by the name of the metadata key, an operator, and a
@@ -335,29 +323,29 @@
 use the right type. Supported Python types are: `str`, `int`, and
 `float`. One more example with a string comparison:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump"))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The real power of predicates is that they can also be combined using the
 `&` operator (for combining predicates with AND semantics) and `|`(for
 combining using OR semantic). So you can do:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump") & client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Just for sanity, let’s show a case where no results are returned because
 or predicates:
@@ -372,29 +360,29 @@
 use grouping with parenthesis:
 
 ``` python
 my_predicates = client.Predicates("action", "==", "jump") & (client.Predicates("times", "==", 1) | client.Predicates("times", ">", 1))
 vec.search([1.0, 9.0], limit=2, predicates=my_predicates)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 We also have some semantic sugar for combining many predicates with AND
 semantics. You can pass in multiple 3-tuples to
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates):
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates(("action", "==", "jump"), ("times", ">", 10)))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Filter your search by time
 
@@ -418,15 +406,15 @@
 Then, you can filter using the timestamps by specifing a
 `uuid_time_filter`:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(specific_datetime, specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 A
 [`UUIDTimeRange`](https://timescale.github.io/python-vector/vector.html#uuidtimerange)
@@ -434,20 +422,20 @@
 Specifying only the start_date or end_date leaves the other end
 unconstrained.
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+     [UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You have the option to define the inclusivity of the start and end dates
 with the `start_inclusive` and `end_inclusive` parameters. Setting
@@ -456,15 +444,15 @@
 default, the start date is inclusive, while the end date is exclusive.
 One example:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime, start_inclusive=False))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Notice how the results are different when we use the
 `start_inclusive=False` option because the first row has the exact
@@ -478,26 +466,26 @@
 systems). The reserved key names are `__start_date` and `__end_date` for
 filters and `__uuid_timestamp` for predicates. Some examples below:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, filter={ "__start_date": specific_datetime, "__end_date": specific_datetime+timedelta(days=1)})
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, 
              predicates=client.Predicates("__uuid_timestamp", ">", specific_datetime) & client.Predicates("__uuid_timestamp", "<", specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ### Indexing
 
@@ -858,15 +846,15 @@
 blog table defined in the following way:
 
 ``` python
 import psycopg2
 from langchain.docstore.document import Document
 from langchain.text_splitter import CharacterTextSplitter
 from timescale_vector import client, pgvectorizer
-from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain_openai import OpenAIEmbeddings
 from langchain.vectorstores.timescalevector import TimescaleVector
 from datetime import timedelta
 ```
 
 ``` python
 with psycopg2.connect(service_url) as conn:
     with conn.cursor() as cursor:
@@ -971,14 +959,14 @@
     time_partition_interval=timedelta(days=30),
 )
 
 res = vector_store.similarity_search_with_score("Blogs about cats")
 res
 ```
 
-    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-855a-06302dbc8ce7', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
-      0.12595687795193833)]
+    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-979c-e8748f6439f2', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
+      0.12657619616729976)]
 
 ## Development
 
 This project is developed with [nbdev](https://nbdev.fast.ai/). Please
 see that website for the development process.
```

### Comparing `timescale-vector-0.0.4/README.md` & `timescale-vector-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,39 @@
+Metadata-Version: 2.1
+Name: timescale-vector
+Version: 0.0.5
+Summary: Python library for storing vector data in Postgres
+Home-page: https://github.com/timescale/python-vector
+Author: Matvey Arye
+Author-email: mat@timescale.com
+License: Apache Software License 2.0
+Keywords: nbdev jupyter notebook python
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+Requires-Dist: asyncpg
+Requires-Dist: psycopg2
+Requires-Dist: pgvector
+Provides-Extra: dev
+Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: langchain; extra == "dev"
+Requires-Dist: langchain-openai; extra == "dev"
+
 # Timescale Vector
 
+
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 PostgreSQL++ for AI Applications.
 
 - [Signup for Timescale
   Vector](https://console.cloud.timescale.com/signup?utm_campaign=vectorlaunch&utm_source=github&utm_medium=direct):
   Get 90 days free to try Timescale Vector on the Timescale cloud data
@@ -35,14 +65,24 @@
 We also use `dotenv` in our examples for passing around secrets and
 keys. You can install that with:
 
 ``` sh
 pip install python-dotenv
 ```
 
+If you run into installation errors related to the psycopg2 package, you
+will need to install some prerequisites. The timescale-vector package
+explicitly depends on psycopg2 (the non-binary version). This adheres to
+[the advice provided by
+psycopg2](https://www.psycopg.org/docs/install.html#psycopg-vs-psycopg-binary).
+Building psycopg from source [requires a few prerequisites to be
+installed](https://www.psycopg.org/docs/install.html#build-prerequisites).
+Make sure these are installed before trying to
+`pip install timescale_vector`.
+
 ## Basic usage
 
 First, import all the necessary libraries:
 
 ``` python
 from dotenv import load_dotenv, find_dotenv
 import os
@@ -105,20 +145,20 @@
 
 Now, you can query for similar items:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('73d05d6e-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('45ecb350-0f15-11ef-8d89-e666703872d0'),
       {'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 There are many search options which we will cover below in the
 `Advanced search` section.
@@ -126,15 +166,15 @@
 As one example, we will return one item using a similarity search
 constrained by a metadata filter.
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The returned records contain 5 fields:
 
@@ -150,15 +190,15 @@
 keyed on the field name:
 
 ``` python
 records = vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 (records[0]["id"],records[0]["metadata"], records[0]["contents"], records[0]["embedding"], records[0]["distance"])
 ```
 
-    (UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    (UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
      {'action': 'jump', 'animal': 'fox'},
      'jumped over the',
      array([ 1. , 10.8], dtype=float32),
      0.00016793422934946456)
 
 You can delete by ID:
 
@@ -213,32 +253,32 @@
 
 The basic query looks like:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You could provide a limit for the number of items returned:
 
 ``` python
 vec.search([1.0, 9.0], limit=1)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Narrowing your search by metadata
 
@@ -255,48 +295,48 @@
 have to match the provided values (keys not in the filter are
 unconstrained):
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "sit"})
 ```
 
-    [[UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You can also specify a list of filter dictionaries, where an item is
 returned if it matches any dict:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, filter=[{"action": "jump"}, {"animal": "fox"}])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ##### Predicates
 
 Predicates allow for more complex search conditions. For example, you
 could use greater than and less than conditions on numeric values.
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates)
 objects are defined by the name of the metadata key, an operator, and a
@@ -312,29 +352,29 @@
 use the right type. Supported Python types are: `str`, `int`, and
 `float`. One more example with a string comparison:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump"))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The real power of predicates is that they can also be combined using the
 `&` operator (for combining predicates with AND semantics) and `|`(for
 combining using OR semantic). So you can do:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump") & client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Just for sanity, let’s show a case where no results are returned because
 or predicates:
@@ -349,29 +389,29 @@
 use grouping with parenthesis:
 
 ``` python
 my_predicates = client.Predicates("action", "==", "jump") & (client.Predicates("times", "==", 1) | client.Predicates("times", ">", 1))
 vec.search([1.0, 9.0], limit=2, predicates=my_predicates)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 We also have some semantic sugar for combining many predicates with AND
 semantics. You can pass in multiple 3-tuples to
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates):
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates(("action", "==", "jump"), ("times", ">", 10)))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Filter your search by time
 
@@ -395,15 +435,15 @@
 Then, you can filter using the timestamps by specifing a
 `uuid_time_filter`:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(specific_datetime, specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 A
 [`UUIDTimeRange`](https://timescale.github.io/python-vector/vector.html#uuidtimerange)
@@ -411,20 +451,20 @@
 Specifying only the start_date or end_date leaves the other end
 unconstrained.
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+     [UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You have the option to define the inclusivity of the start and end dates
 with the `start_inclusive` and `end_inclusive` parameters. Setting
@@ -433,15 +473,15 @@
 default, the start date is inclusive, while the end date is exclusive.
 One example:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime, start_inclusive=False))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Notice how the results are different when we use the
 `start_inclusive=False` option because the first row has the exact
@@ -455,26 +495,26 @@
 systems). The reserved key names are `__start_date` and `__end_date` for
 filters and `__uuid_timestamp` for predicates. Some examples below:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, filter={ "__start_date": specific_datetime, "__end_date": specific_datetime+timedelta(days=1)})
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, 
              predicates=client.Predicates("__uuid_timestamp", ">", specific_datetime) & client.Predicates("__uuid_timestamp", "<", specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ### Indexing
 
@@ -835,15 +875,15 @@
 blog table defined in the following way:
 
 ``` python
 import psycopg2
 from langchain.docstore.document import Document
 from langchain.text_splitter import CharacterTextSplitter
 from timescale_vector import client, pgvectorizer
-from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain_openai import OpenAIEmbeddings
 from langchain.vectorstores.timescalevector import TimescaleVector
 from datetime import timedelta
 ```
 
 ``` python
 with psycopg2.connect(service_url) as conn:
     with conn.cursor() as cursor:
@@ -948,14 +988,14 @@
     time_partition_interval=timedelta(days=30),
 )
 
 res = vector_store.similarity_search_with_score("Blogs about cats")
 res
 ```
 
-    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-855a-06302dbc8ce7', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
-      0.12595687795193833)]
+    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-979c-e8748f6439f2', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
+      0.12657619616729976)]
 
 ## Development
 
 This project is developed with [nbdev](https://nbdev.fast.ai/). Please
 see that website for the development process.
```

### Comparing `timescale-vector-0.0.4/settings.ini` & `timescale-vector-0.0.5/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = python-vector
 lib_name = timescale-vector
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = timescale_vector
 nbs_path = nbs
 recursive = True
@@ -23,15 +23,15 @@
 copyright = 2023 onwards, Matvey Arye
 description = Python library for storing vector data in Postgres
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = timescale
 requirements = asyncpg psycopg2 pgvector
-dev_requirements = python-dotenv langchain
+dev_requirements = python-dotenv langchain langchain-openai
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `timescale-vector-0.0.4/setup.py` & `timescale-vector-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `timescale-vector-0.0.4/timescale_vector/_modidx.py` & `timescale-vector-0.0.5/timescale_vector/_modidx.py`

 * *Files identical despite different names*

### Comparing `timescale-vector-0.0.4/timescale_vector/client.py` & `timescale-vector-0.0.5/timescale_vector/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,17 +324,18 @@
         "=": "=",
         "==": "=",
         ">=": ">=",
         ">": ">",
         "<=": "<=",
         "<": "<",
         "!=": "<>",
+        "@>": "@>", # array contains
     }
 
-    PredicateValue = Union[str, int, float, datetime]
+    PredicateValue = Union[str, int, float, datetime, list, tuple]
 
     def __init__(self, *clauses: Union['Predicates', Tuple[str, PredicateValue], Tuple[str, str, PredicateValue], str, PredicateValue], operator: str = 'AND'):
         """
         Predicates class defines predicates on the object metadata. Predicates can be combined using logical operators (&, |, and ~).
 
         Parameters
         ----------
@@ -427,26 +428,32 @@
                 if field == '__uuid_timestamp':
                     #convert str to timestamp in the database, it's better at it than python
                     if isinstance(value, str):
                         where_conditions.append(f"uuid_timestamp(id) {operator} ({param_name}::text)::timestamptz")
                     else:
                         where_conditions.append(f"uuid_timestamp(id) {operator} {param_name}")
                     params.append(value)
-                    continue
-
-                field_cast = ''
-                if isinstance(value, int):
-                    field_cast = '::int'
-                elif isinstance(value, float):
-                    field_cast = '::numeric'
-                elif isinstance(value, datetime):
-                    field_cast = '::timestamptz'   
-
-                where_conditions.append(f"(metadata->>'{field}'){field_cast} {operator} {param_name}")
-                params.append(value) 
+                
+                elif operator == "@>" and (isinstance(value, list) or isinstance(value, tuple)):
+                    if len(value) == 0:
+                        raise ValueError("Invalid value. Empty lists and empty tuples are not supported.")
+                    json_value = json.dumps(value)
+                    where_conditions.append(f"metadata @> jsonb_build_object('{field}', {param_name}::jsonb)")
+                    params.append(json_value)
+                
+                else:
+                    field_cast = ''
+                    if isinstance(value, int):
+                        field_cast = '::int'
+                    elif isinstance(value, float):
+                        field_cast = '::numeric'
+                    elif isinstance(value, datetime):
+                        field_cast = '::timestamptz'
+                    where_conditions.append(f"(metadata->>'{field}'){field_cast} {operator} {param_name}")
+                    params.append(value) 
 
         if self.operator == 'NOT':
             or_clauses = (" OR ").join(where_conditions)
             #use IS DISTINCT FROM to treat all-null clauses as False and pass the filter
             where_clause = f"TRUE IS DISTINCT FROM ({or_clauses})"
         else:
             where_clause = (" "+self.operator+" ").join(where_conditions)
@@ -968,15 +975,15 @@
 
         Parameters
         ----------
         index
             The index to create.
 
         Returns
-        --------
+        -------
             None
         """
         #todo: can we make geting the records lazy?
         num_records = await self._get_approx_count()
         query = self.builder.create_embedding_index_query(index, lambda: num_records)
         
         async with await self.connect() as pool:
@@ -999,17 +1006,20 @@
             The query embedding vector.
         limit 
             The number of nearest neighbors to retrieve.
         filter 
             A filter for metadata. Should be specified as a key-value object or a list of key-value objects (where any objects in the list are matched).
         predicates
             A Predicates object to filter the results. Predicates support more complex queries than the filter parameter. Predicates can be combined using logical operators (&, |, and ~).
+        uuid_time_filter
+            A UUIDTimeRange object to filter the results by time using the id column.
+        query_params
 
         Returns
-        --------
+        -------
             List: List of similar records.
         """
         (query, params) = self.builder.search_query(
             query_embedding, limit, filter, predicates, uuid_time_filter)
         if query_params is not None:
             async with await self.connect() as pool:
                 async with pool.transaction():
```

### Comparing `timescale-vector-0.0.4/timescale_vector/pgvectorizer.py` & `timescale-vector-0.0.5/timescale_vector/pgvectorizer.py`

 * *Files identical despite different names*

### Comparing `timescale-vector-0.0.4/timescale_vector.egg-info/PKG-INFO` & `timescale-vector-0.0.5/timescale_vector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescale-vector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for storing vector data in Postgres
 Home-page: https://github.com/timescale/python-vector
 Author: Matvey Arye
 Author-email: mat@timescale.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,27 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: asyncpg
+Requires-Dist: psycopg2
+Requires-Dist: pgvector
+Provides-Extra: dev
+Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: langchain; extra == "dev"
+Requires-Dist: langchain-openai; extra == "dev"
 
 # Timescale Vector
 
+
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 PostgreSQL++ for AI Applications.
 
 - [Signup for Timescale
   Vector](https://console.cloud.timescale.com/signup?utm_campaign=vectorlaunch&utm_source=github&utm_medium=direct):
   Get 90 days free to try Timescale Vector on the Timescale cloud data
@@ -58,14 +65,24 @@
 We also use `dotenv` in our examples for passing around secrets and
 keys. You can install that with:
 
 ``` sh
 pip install python-dotenv
 ```
 
+If you run into installation errors related to the psycopg2 package, you
+will need to install some prerequisites. The timescale-vector package
+explicitly depends on psycopg2 (the non-binary version). This adheres to
+[the advice provided by
+psycopg2](https://www.psycopg.org/docs/install.html#psycopg-vs-psycopg-binary).
+Building psycopg from source [requires a few prerequisites to be
+installed](https://www.psycopg.org/docs/install.html#build-prerequisites).
+Make sure these are installed before trying to
+`pip install timescale_vector`.
+
 ## Basic usage
 
 First, import all the necessary libraries:
 
 ``` python
 from dotenv import load_dotenv, find_dotenv
 import os
@@ -128,20 +145,20 @@
 
 Now, you can query for similar items:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('73d05d6e-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('45ecb350-0f15-11ef-8d89-e666703872d0'),
       {'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 There are many search options which we will cover below in the
 `Advanced search` section.
@@ -149,15 +166,15 @@
 As one example, we will return one item using a similarity search
 constrained by a metadata filter.
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 ```
 
-    [[UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
       {'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The returned records contain 5 fields:
 
@@ -173,15 +190,15 @@
 keyed on the field name:
 
 ``` python
 records = vec.search([1.0, 9.0], limit=1, filter={"action": "jump"})
 (records[0]["id"],records[0]["metadata"], records[0]["contents"], records[0]["embedding"], records[0]["distance"])
 ```
 
-    (UUID('73d05df0-84c1-11ee-98da-6ee10b77fd08'),
+    (UUID('45ecb666-0f15-11ef-8d89-e666703872d0'),
      {'action': 'jump', 'animal': 'fox'},
      'jumped over the',
      array([ 1. , 10.8], dtype=float32),
      0.00016793422934946456)
 
 You can delete by ID:
 
@@ -236,32 +253,32 @@
 
 The basic query looks like:
 
 ``` python
 vec.search([1.0, 9.0])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You could provide a limit for the number of items returned:
 
 ``` python
 vec.search([1.0, 9.0], limit=1)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Narrowing your search by metadata
 
@@ -278,48 +295,48 @@
 have to match the provided values (keys not in the filter are
 unconstrained):
 
 ``` python
 vec.search([1.0, 9.0], limit=1, filter={"action": "sit"})
 ```
 
-    [[UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You can also specify a list of filter dictionaries, where an item is
 returned if it matches any dict:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, filter=[{"action": "jump"}, {"animal": "fox"}])
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('7487af14-84c1-11ee-98da-6ee10b77fd08'),
+     [UUID('4d629a50-0f15-11ef-8d89-e666703872d0'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ##### Predicates
 
 Predicates allow for more complex search conditions. For example, you
 could use greater than and less than conditions on numeric values.
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates)
 objects are defined by the name of the metadata key, an operator, and a
@@ -335,29 +352,29 @@
 use the right type. Supported Python types are: `str`, `int`, and
 `float`. One more example with a string comparison:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump"))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 The real power of predicates is that they can also be combined using the
 `&` operator (for combining predicates with AND semantics) and `|`(for
 combining using OR semantic). So you can do:
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates("action", "==", "jump") & client.Predicates("times", ">", 1))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Just for sanity, let’s show a case where no results are returned because
 or predicates:
@@ -372,29 +389,29 @@
 use grouping with parenthesis:
 
 ``` python
 my_predicates = client.Predicates("action", "==", "jump") & (client.Predicates("times", "==", 1) | client.Predicates("times", ">", 1))
 vec.search([1.0, 9.0], limit=2, predicates=my_predicates)
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 We also have some semantic sugar for combining many predicates with AND
 semantics. You can pass in multiple 3-tuples to
 [`Predicates`](https://timescale.github.io/python-vector/vector.html#predicates):
 
 ``` python
 vec.search([1.0, 9.0], limit=2, predicates=client.Predicates(("action", "==", "jump"), ("times", ">", 10)))
 ```
 
-    [[UUID('7487af96-84c1-11ee-98da-6ee10b77fd08'),
+    [[UUID('4d629b54-0f15-11ef-8d89-e666703872d0'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 #### Filter your search by time
 
@@ -418,15 +435,15 @@
 Then, you can filter using the timestamps by specifing a
 `uuid_time_filter`:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(specific_datetime, specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 A
 [`UUIDTimeRange`](https://timescale.github.io/python-vector/vector.html#uuidtimerange)
@@ -434,20 +451,20 @@
 Specifying only the start_date or end_date leaves the other end
 unconstrained.
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456],
-     [UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+     [UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 You have the option to define the inclusivity of the start and end dates
 with the `start_inclusive` and `end_inclusive` parameters. Setting
@@ -456,15 +473,15 @@
 default, the start date is inclusive, while the end date is exclusive.
 One example:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, uuid_time_filter=client.UUIDTimeRange(start_date=specific_datetime, start_inclusive=False))
 ```
 
-    [[UUID('ac8be800-0de6-11e9-889a-5eec84ba8a7b'),
+    [[UUID('0e505000-0def-11e9-8732-a154fea6fb50'),
       {'times': 100, 'action': 'jump', 'animal': 'fox'},
       'jumped over the',
       array([ 1. , 10.8], dtype=float32),
       0.00016793422934946456]]
 
 Notice how the results are different when we use the
 `start_inclusive=False` option because the first row has the exact
@@ -478,26 +495,26 @@
 systems). The reserved key names are `__start_date` and `__end_date` for
 filters and `__uuid_timestamp` for predicates. Some examples below:
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, filter={ "__start_date": specific_datetime, "__end_date": specific_datetime+timedelta(days=1)})
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ``` python
 tpvec.search([1.0, 9.0], limit=4, 
              predicates=client.Predicates("__uuid_timestamp", ">", specific_datetime) & client.Predicates("__uuid_timestamp", "<", specific_datetime+timedelta(days=1)))
 ```
 
-    [[UUID('33c52800-ef15-11e7-be03-4f1f9a1bde5a'),
+    [[UUID('95899000-ef1d-11e7-990e-7d2f7e013038'),
       {'times': 1, 'action': 'sit', 'animal': 'fox'},
       'the brown fox',
       array([1. , 1.3], dtype=float32),
       0.14489260377438218]]
 
 ### Indexing
 
@@ -858,15 +875,15 @@
 blog table defined in the following way:
 
 ``` python
 import psycopg2
 from langchain.docstore.document import Document
 from langchain.text_splitter import CharacterTextSplitter
 from timescale_vector import client, pgvectorizer
-from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain_openai import OpenAIEmbeddings
 from langchain.vectorstores.timescalevector import TimescaleVector
 from datetime import timedelta
 ```
 
 ``` python
 with psycopg2.connect(service_url) as conn:
     with conn.cursor() as cursor:
@@ -971,14 +988,14 @@
     time_partition_interval=timedelta(days=30),
 )
 
 res = vector_store.similarity_search_with_score("Blogs about cats")
 res
 ```
 
-    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-855a-06302dbc8ce7', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
-      0.12595687795193833)]
+    [(Document(page_content='Author Matvey Arye, title: First Post, contents:some super interesting content about cats.', metadata={'id': '4a784000-4bc4-11eb-979c-e8748f6439f2', 'author': 'Matvey Arye', 'blog_id': 1, 'category': 'AI', 'published_time': '2021-01-01T00:00:00+00:00'}),
+      0.12657619616729976)]
 
 ## Development
 
 This project is developed with [nbdev](https://nbdev.fast.ai/). Please
 see that website for the development process.
```

