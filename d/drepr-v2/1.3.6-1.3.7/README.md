# Comparing `tmp/drepr_v2-1.3.6.tar.gz` & `tmp/drepr_v2-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.3.6.tar", max compression
+gzip compressed data, was "drepr_v2-1.3.7.tar", max compression
```

## Comparing `drepr_v2-1.3.6.tar` & `drepr_v2-1.3.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1064 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/LICENSE
--rw-r--r--   0        0        0       53 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/README.md
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/__init__.py
--rw-r--r--   0        0        0     3752 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/__main__.py
--rw-r--r--   0        0        0     2063 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/main.py
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/__init__.py
--rw-r--r--   0        0        0     4710 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/attr.py
--rw-r--r--   0        0        0    12298 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4520 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11569 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     9359 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/prelude.py
--rw-r--r--   0        0        0     3917 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     2200 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/resource.py
--rw-r--r--   0        0        0     9252 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/planning/__init__.py
--rw-r--r--   0        0        0    19809 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    17577 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4783 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    17908 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    23969 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    16794 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1458 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/__init__.py
--rw-r--r--   0        0        0      361 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/csv.py
--rw-r--r--   0        0        0      365 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/prelude.py
--rw-r--r--   0        0        0      382 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/spreadsheet.py
--rw-r--r--   0        0        0       61 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/__init__.py
--rw-r--r--   0        0        0     6400 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/attr_data.py
--rw-r--r--   0        0        0     2960 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/misc.py
--rw-r--r--   0        0        0      828 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/safe.py
--rw-r--r--   0        0        0     5729 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/base.py
--rw-r--r--   0        0        0     3986 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      605 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/LICENSE
+-rw-r--r--   0        0        0       53 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/__init__.py
+-rw-r--r--   0        0        0     3810 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/__main__.py
+-rw-r--r--   0        0        0     2063 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/main.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/attr.py
+-rw-r--r--   0        0        0    12298 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4520 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2200 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.717357 drepr_v2-1.3.7/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19809 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/readers/csv.py
+-rw-r--r--   0        0        0      365 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/safe.py
+-rw-r--r--   0        0        0     5729 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/writers/base.py
+-rw-r--r--   0        0        0     3986 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      605 2024-05-15 01:21:12.721356 drepr_v2-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.7/PKG-INFO
```

### Comparing `drepr_v2-1.3.6/LICENSE` & `drepr_v2-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/__main__.py` & `drepr_v2-1.3.7/drepr/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,19 @@
         typer.Argument(
             help="A path to a file containing representation (support 2 formats: JSON & YML)",
             exists=True,
             dir_okay=False,
         ),
     ],
     resource: Annotated[
-        list[str],
+        Optional[list[str]],
         typer.Argument(
             help="file paths of resources in this format: <resource_id>=<file_path>",
         ),
-    ],
+    ] = None,
     progfile: Annotated[
         Optional[Path],
         typer.Option(
             help="A path to a file to save the generated program", exists=False
         ),
     ] = None,
     outfile: Annotated[
@@ -76,17 +76,14 @@
             default="/tmp/drepr",
         ),
     ] = Path("/tmp/drepr"),
     debuginfo: Annotated[
         bool, typer.Option(help="Whether to add debug information to the program")
     ] = False,
 ):
-    parsed_resources = {
-        (x := ResourceInput.from_string(r)).id: x.file for r in resource
-    }
     parsed_repr = DRepr.parse_from_file(repr)
     exec_plan = ClassesMapExecutionPlan.create(parsed_repr)
 
     if outfile is not None:
         output = FileOutput(outfile, format)
     else:
         output = MemoryOutput(format)
@@ -98,14 +95,20 @@
             f.write(prog)
     else:
         tmpdir.mkdir(parents=True, exist_ok=True)
         unique_id = str(uuid4()).replace("-", "_")
         progfile = tmpdir / f"main_{unique_id}.py"
         progfile.write_text(prog)
 
+    if resource is None:
+        return
+
+    parsed_resources = {
+        (x := ResourceInput.from_string(r)).id: x.file for r in resource
+    }
     spec = importlib.util.spec_from_file_location("drepr_prog", progfile)
     assert spec is not None and spec.loader is not None
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     if outfile is not None:
         module.main(
             *[
```

### Comparing `drepr_v2-1.3.6/drepr/main.py` & `drepr_v2-1.3.7/drepr/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/align.py` & `drepr_v2-1.3.7/drepr/models/align.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/attr.py` & `drepr_v2-1.3.7/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/drepr.py` & `drepr_v2-1.3.7/drepr/models/drepr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/drepr_builder.py` & `drepr_v2-1.3.7/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/attr_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.3.7/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v2/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.3.7/drepr/models/parse_v2/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/path.py` & `drepr_v2-1.3.7/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/preprocessing.py` & `drepr_v2-1.3.7/drepr/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/resource.py` & `drepr_v2-1.3.7/drepr/models/resource.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/models/sm.py` & `drepr_v2-1.3.7/drepr/models/sm.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/planning/class_map_plan.py` & `drepr_v2-1.3.7/drepr/planning/class_map_plan.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.3.7/drepr/planning/drepr_model_alignments.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/planning/topological_sorting.py` & `drepr_v2-1.3.7/drepr/planning/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.3.7/drepr/program_generation/alignment_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/main.py` & `drepr_v2-1.3.7/drepr/program_generation/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.3.7/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/preprocessing.py` & `drepr_v2-1.3.7/drepr/program_generation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/program_space.py` & `drepr_v2-1.3.7/drepr/program_generation/program_space.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/program_generation/writers.py` & `drepr_v2-1.3.7/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/utils/attr_data.py` & `drepr_v2-1.3.7/drepr/utils/attr_data.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/utils/misc.py` & `drepr_v2-1.3.7/drepr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/utils/namespace_mixin.py` & `drepr_v2-1.3.7/drepr/utils/namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/utils/udf.py` & `drepr_v2-1.3.7/drepr/utils/udf.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/utils/validator.py` & `drepr_v2-1.3.7/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/writers/base.py` & `drepr_v2-1.3.7/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/drepr/writers/rdfgraph_writer.py` & `drepr_v2-1.3.7/drepr/writers/rdfgraph_writer.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.6/pyproject.toml` & `drepr_v2-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.3.6"
+version = "1.3.7"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `drepr_v2-1.3.6/PKG-INFO` & `drepr_v2-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.3.6
+Version: 1.3.7
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

