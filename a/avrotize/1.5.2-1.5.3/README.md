# Comparing `tmp/avrotize-1.5.2.tar.gz` & `tmp/avrotize-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.5.2.tar` & `avrotize-1.5.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    30034 2024-05-14 18:14:27.070084 avrotize-1.5.2/README.md
--rw-r--r--   0        0        0     1673 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-14 18:14:31.266114 avrotize-1.5.2/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    16902 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotize.py
--rw-r--r--   0        0        0    48409 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58275 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     6433 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13758 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/constants.py
--rw-r--r--   0        0        0    19374 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-14 18:14:27.070084 avrotize-1.5.2/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    20738 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/kustotoavro.py
--rw-r--r--   0        0        0    19742 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-14 18:14:27.074084 avrotize-1.5.2/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1169 2024-05-14 18:14:27.074084 avrotize-1.5.2/pyproject.toml
--rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    30034 2024-05-14 18:52:03.138231 avrotize-1.5.3/README.md
+-rw-r--r--   0        0        0     1673 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-14 18:52:07.602216 avrotize-1.5.3/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    16902 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotize.py
+-rw-r--r--   0        0        0    48409 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58275 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     6501 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13758 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/common.py
+-rw-r--r--   0        0        0      112 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/constants.py
+-rw-r--r--   0        0        0    19374 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    20738 2024-05-14 18:52:03.138231 avrotize-1.5.3/avrotize/kustotoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-14 18:52:03.142231 avrotize-1.5.3/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1169 2024-05-14 18:52:03.142231 avrotize-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0    30740 1970-01-01 00:00:00.000000 avrotize-1.5.3/PKG-INFO
```

### Comparing `avrotize-1.5.2/README.md` & `avrotize-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/__init__.py` & `avrotize-1.5.3/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/asn1toavro.py` & `avrotize-1.5.3/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotize.py` & `avrotize-1.5.3/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotocsharp.py` & `avrotize-1.5.3/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotojava.py` & `avrotize-1.5.3/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotojs.py` & `avrotize-1.5.3/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotojsons.py` & `avrotize-1.5.3/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotokusto.py` & `avrotize-1.5.3/avrotize/avrotokusto.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,50 +10,52 @@
     fields = schema["fields"]
 
     # Create a StringBuilder to store the kusto statements
     kusto = []
 
     # Append the create table statement with the column names and types
     kusto.append(f".create table [{table_name}] (")
+    columns = []
     for field in fields:
         column_name = field["name"]
         column_type = convert_avro_type_to_kusto_type(field["type"])
-        kusto.append(f"    [{column_name}]: {column_type},")
+        columns.append(f"    [{column_name}]: {column_type}")
     if emit_cloud_events_columns:
-        kusto.append("    [__type]: string,")
-        kusto.append("    [__source]: string,")
-        kusto.append("    [__id]: string,")
-        kusto.append("    [__time]: datetime,")
-        kusto.append("    [__subject]: string")
+        columns.append("    [__type]: string")
+        columns.append("    [__source]: string")
+        columns.append("    [__id]: string")
+        columns.append("    [__time]: datetime")
+        columns.append("    [__subject]: string")
+    kusto.append(",\n".join(columns))
     kusto.append(");")
     kusto.append("")
 
     # Add the doc string as table metadata
     if "doc" in schema:
         doc_string = schema["doc"]
         kusto.append(f".alter table [{table_name}] docstring '{doc_string}';")
         kusto.append("")
 
     doc_string_statement = []
     for field in fields:
         column_name = field["name"]
         if "doc" in field:
             doc = field["doc"]
-            doc_string_statement.append(f"   [{column_name}]: '{doc}',")
+            doc_string_statement.append(f"   [{column_name}]: '{doc}'")
     if doc_string_statement and emit_cloud_events_columns:
         doc_string_statement.extend([
-            "  [__type] : 'Event type',",
-            "  [__source]: 'Context origin/source of the event',",
-            "  [__id]: 'Event identifier',",
-            "  [__time]: 'Event generation time',",
-            "  [__subject]: 'Context subject of the event',"
+            "  [__type] : 'Event type'",
+            "  [__source]: 'Context origin/source of the event'",
+            "  [__id]: 'Event identifier'",
+            "  [__time]: 'Event generation time'",
+            "  [__subject]: 'Context subject of the event'"
         ])
     if doc_string_statement:
         kusto.append(f".alter table [{table_name}] column-docstrings (")
-        kusto.extend(doc_string_statement)
+        kusto.append(",\n".join(doc_string_statement))
         kusto.append(");")
         kusto.append("")
 
     # add the JSON mapping for the table
     # .create-or-alter table dfl_data_events ingestion json mapping
     kusto.append(
         f".create-or-alter table [{table_name}] ingestion json mapping \"{table_name}_json_mapping\"")
```

### Comparing `avrotize-1.5.2/avrotize/avrotoparquet.py` & `avrotize-1.5.3/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotoproto.py` & `avrotize-1.5.3/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotopython.py` & `avrotize-1.5.3/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotots.py` & `avrotize-1.5.3/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrototsql.py` & `avrotize-1.5.3/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/avrotoxsd.py` & `avrotize-1.5.3/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/common.py` & `avrotize-1.5.3/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/dependency_resolver.py` & `avrotize-1.5.3/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/generic/generic.avsc` & `avrotize-1.5.3/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/jsonstoavro.py` & `avrotize-1.5.3/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/kconnect.json` & `avrotize-1.5.3/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/kstructtoavro.py` & `avrotize-1.5.3/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/kustotoavro.py` & `avrotize-1.5.3/avrotize/kustotoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/proto2parser.py` & `avrotize-1.5.3/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/proto3parser.py` & `avrotize-1.5.3/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototoavro.py` & `avrotize-1.5.3/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/any.avsc` & `avrotize-1.5.3/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/api.avsc` & `avrotize-1.5.3/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/duration.avsc` & `avrotize-1.5.3/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/field_mask.avsc` & `avrotize-1.5.3/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/struct.avsc` & `avrotize-1.5.3/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/timestamp.avsc` & `avrotize-1.5.3/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/type.avsc` & `avrotize-1.5.3/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/prototypes/wrappers.avsc` & `avrotize-1.5.3/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/avrotize/xsdtoavro.py` & `avrotize-1.5.3/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/pyproject.toml` & `avrotize-1.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.5.2/PKG-INFO` & `avrotize-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.5.2
+Version: 1.5.3
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

