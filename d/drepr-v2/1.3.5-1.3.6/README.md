# Comparing `tmp/drepr_v2-1.3.5.tar.gz` & `tmp/drepr_v2-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.3.5.tar", max compression
+gzip compressed data, was "drepr_v2-1.3.6.tar", max compression
```

## Comparing `drepr_v2-1.3.5.tar` & `drepr_v2-1.3.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1064 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/LICENSE
--rw-r--r--   0        0        0       53 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/README.md
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/__init__.py
--rw-r--r--   0        0        0     3754 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/__main__.py
--rw-r--r--   0        0        0     2063 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/main.py
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/__init__.py
--rw-r--r--   0        0        0     4710 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/attr.py
--rw-r--r--   0        0        0    12298 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4520 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11569 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     9359 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/prelude.py
--rw-r--r--   0        0        0     3917 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     2200 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/resource.py
--rw-r--r--   0        0        0     9252 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/planning/__init__.py
--rw-r--r--   0        0        0    19809 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    17577 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4783 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    17908 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    23969 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    16794 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1458 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/readers/__init__.py
--rw-r--r--   0        0        0      361 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/readers/csv.py
--rw-r--r--   0        0        0      365 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/readers/prelude.py
--rw-r--r--   0        0        0      382 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/readers/spreadsheet.py
--rw-r--r--   0        0        0       61 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/__init__.py
--rw-r--r--   0        0        0     6400 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/attr_data.py
--rw-r--r--   0        0        0     2960 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/misc.py
--rw-r--r--   0        0        0      828 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/safe.py
--rw-r--r--   0        0        0     5729 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/writers/base.py
--rw-r--r--   0        0        0     3986 2024-05-14 19:08:05.285577 drepr_v2-1.3.5/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      605 2024-05-14 19:08:05.289577 drepr_v2-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 drepr_v2-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/LICENSE
+-rw-r--r--   0        0        0       53 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/__init__.py
+-rw-r--r--   0        0        0     3752 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/__main__.py
+-rw-r--r--   0        0        0     2063 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/main.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/attr.py
+-rw-r--r--   0        0        0    12298 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4520 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2200 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.691719 drepr_v2-1.3.6/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19809 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/csv.py
+-rw-r--r--   0        0        0      365 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/safe.py
+-rw-r--r--   0        0        0     5729 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/base.py
+-rw-r--r--   0        0        0     3986 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      605 2024-05-15 00:22:48.695719 drepr_v2-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 drepr_v2-1.3.6/PKG-INFO
```

### Comparing `drepr_v2-1.3.5/LICENSE` & `drepr_v2-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/__main__.py` & `drepr_v2-1.3.6/drepr/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
         return ResourceInput(id, file)
 
 
 @app.command()
 def main(
     repr: Annotated[
         Path,
-        typer.Option(
+        typer.Argument(
             help="A path to a file containing representation (support 2 formats: JSON & YML)",
             exists=True,
             dir_okay=False,
         ),
     ],
     resource: Annotated[
         list[str],
-        typer.Option(
+        typer.Argument(
             help="file paths of resources in this format: <resource_id>=<file_path>",
         ),
     ],
     progfile: Annotated[
         Optional[Path],
         typer.Option(
             help="A path to a file to save the generated program", exists=False
@@ -69,15 +69,15 @@
             help="The output format",
         ),
     ] = OutputFormat.TTL,
     tmpdir: Annotated[
         Path,
         typer.Option(
             help="A directory to save temporary files",
-            default=Path("/tmp/drepr"),
+            default="/tmp/drepr",
         ),
     ] = Path("/tmp/drepr"),
     debuginfo: Annotated[
         bool, typer.Option(help="Whether to add debug information to the program")
     ] = False,
 ):
     parsed_resources = {
```

### Comparing `drepr_v2-1.3.5/drepr/main.py` & `drepr_v2-1.3.6/drepr/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/align.py` & `drepr_v2-1.3.6/drepr/models/align.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/attr.py` & `drepr_v2-1.3.6/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/drepr.py` & `drepr_v2-1.3.6/drepr/models/drepr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/drepr_builder.py` & `drepr_v2-1.3.6/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/attr_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.3.6/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v2/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.3.6/drepr/models/parse_v2/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/path.py` & `drepr_v2-1.3.6/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/preprocessing.py` & `drepr_v2-1.3.6/drepr/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/resource.py` & `drepr_v2-1.3.6/drepr/models/resource.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/models/sm.py` & `drepr_v2-1.3.6/drepr/models/sm.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/planning/class_map_plan.py` & `drepr_v2-1.3.6/drepr/planning/class_map_plan.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.3.6/drepr/planning/drepr_model_alignments.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/planning/topological_sorting.py` & `drepr_v2-1.3.6/drepr/planning/topological_sorting.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.3.6/drepr/program_generation/alignment_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/main.py` & `drepr_v2-1.3.6/drepr/program_generation/main.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.3.6/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/preprocessing.py` & `drepr_v2-1.3.6/drepr/program_generation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/program_space.py` & `drepr_v2-1.3.6/drepr/program_generation/program_space.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/program_generation/writers.py` & `drepr_v2-1.3.6/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/utils/attr_data.py` & `drepr_v2-1.3.6/drepr/utils/attr_data.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/utils/misc.py` & `drepr_v2-1.3.6/drepr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/utils/namespace_mixin.py` & `drepr_v2-1.3.6/drepr/utils/namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/utils/udf.py` & `drepr_v2-1.3.6/drepr/utils/udf.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/utils/validator.py` & `drepr_v2-1.3.6/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/writers/base.py` & `drepr_v2-1.3.6/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/drepr/writers/rdfgraph_writer.py` & `drepr_v2-1.3.6/drepr/writers/rdfgraph_writer.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.3.5/pyproject.toml` & `drepr_v2-1.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.3.5"
+version = "1.3.6"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 orjson = "^3.9.13"
 ruamel-yaml = "^0.17.21"
 graph-wrapper = "^1.7.1"
 serde2 = "^1.7.3"
-typer = { extras = ["all"], version = "==0.9.0" }
+typer = { extras = ["all"], version = "^0.12.3" }
 codegen-2 = "^2.1.3"
 rdflib = "^7.0.0"
 openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
 autoflake = "^2.2.1"
```

### Comparing `drepr_v2-1.3.5/PKG-INFO` & `drepr_v2-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.3.5
+Version: 1.3.6
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: codegen-2 (>=2.1.3,<3.0.0)
 Requires-Dist: graph-wrapper (>=1.7.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: orjson (>=3.9.13,<4.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: serde2 (>=1.7.3,<2.0.0)
-Requires-Dist: typer[all] (==0.9.0)
+Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # drepr-v2
 DRepr with code generation implementation
```

