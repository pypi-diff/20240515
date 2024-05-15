# Comparing `tmp/met_annot_unifier-0.0.4.tar.gz` & `tmp/met_annot_unifier-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met_annot_unifier-0.0.4.tar", max compression
+gzip compressed data, was "met_annot_unifier-0.0.5.tar", max compression
```

## Comparing `met_annot_unifier-0.0.4.tar` & `met_annot_unifier-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-04-26 13:45:30.393365 met_annot_unifier-0.0.4/LICENSE
--rw-r--r--   0        0        0     4691 2024-04-26 13:45:30.393365 met_annot_unifier-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/aligner/__init__.py
--rw-r--r--   0        0        0     7539 2024-04-26 13:45:30.421365 met_annot_unifier-0.0.4/met_annot_unifier/aligner/aligner.py
--rw-r--r--   0        0        0     9393 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/aligner/parser.py
--rw-r--r--   0        0        0     2644 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/aligner/utils.py
--rw-r--r--   0        0        0     4947 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/cli.py
--rw-r--r--   0        0        0    10938 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/config/column_config.json
--rw-r--r--   0        0        0      694 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/exceptions.py
--rw-r--r--   0        0        0      267 2024-04-26 13:45:30.425366 met_annot_unifier-0.0.4/met_annot_unifier/foo.py
--rw-r--r--   0        0        0     2409 2024-04-26 13:45:48.893399 met_annot_unifier-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-14 16:27:30.689922 met_annot_unifier-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4691 2024-05-14 16:27:30.689922 met_annot_unifier-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/aligner/__init__.py
+-rw-r--r--   0        0        0     7537 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/aligner/aligner.py
+-rw-r--r--   0        0        0     9393 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/aligner/parser.py
+-rw-r--r--   0        0        0     2644 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/aligner/utils.py
+-rw-r--r--   0        0        0     4947 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/cli.py
+-rw-r--r--   0        0        0    10938 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/config/column_config.json
+-rw-r--r--   0        0        0      694 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/exceptions.py
+-rw-r--r--   0        0        0      267 2024-05-14 16:27:30.717922 met_annot_unifier-0.0.5/met_annot_unifier/foo.py
+-rw-r--r--   0        0        0     2409 2024-05-14 16:27:49.477900 met_annot_unifier-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.5/PKG-INFO
```

### Comparing `met_annot_unifier-0.0.4/LICENSE` & `met_annot_unifier-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/README.md` & `met_annot_unifier-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/aligner/aligner.py` & `met_annot_unifier-0.0.5/met_annot_unifier/aligner/aligner.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     process_isdb_data,
     process_sirius_data,
     standardize_column_names,
 )
 from met_annot_unifier.aligner.utils import count_sources, determine_source
 from met_annot_unifier.exceptions import DataFileError
 
-gnps_file = "examples/data/in/gnps_output_example.tsv"
-sirius_file = "examples/data/in/sirius_output_example.tsv"
-isdb_file = "examples/data/in/isdb_output_example.tsv"
-
 
 def align_data_vertically(
     gnps_file: Optional[str] = None,
     isdb_file: Optional[str] = None,
     sirius_file: Optional[str] = None,
 ) -> pd.DataFrame:
     """
@@ -119,16 +115,18 @@
     pd.DataFrame: A DataFrame with aligned and merged data from the provided sources.
     """
 
     data_frames = []
 
     if canopus_file:
         canopus_data = pd.read_csv(canopus_file, sep="\t")
-        canopus_data = standardize_column_names(canopus_data, "feature_id", "feature_id")
+        canopus_data = standardize_column_names(canopus_data, "id", "feature_id")
         canopus_data = prefix_columns(canopus_data, "canopus_", exclude_columns=[])
+        canopus_data = extract_feature_id(canopus_data, "canopus_feature_id")
+        canopus_data = standardize_column_names(canopus_data, "canopus_feature_id", "feature_id")
         data_frames.append(canopus_data)
 
     if gnps_file:
         gnps_data = pd.read_csv(gnps_file, sep="\t")
         gnps_data = standardize_column_names(gnps_data, "InChIKey-Planar", "IK2D")
         gnps_data = standardize_column_names(gnps_data, "#Scan#", "feature_id")
         gnps_data = standardize_column_names(gnps_data, "Smiles", "SMILES")
```

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/aligner/parser.py` & `met_annot_unifier-0.0.5/met_annot_unifier/aligner/parser.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/aligner/utils.py` & `met_annot_unifier-0.0.5/met_annot_unifier/aligner/utils.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/cli.py` & `met_annot_unifier-0.0.5/met_annot_unifier/cli.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/config/column_config.json` & `met_annot_unifier-0.0.5/met_annot_unifier/config/column_config.json`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/met_annot_unifier/exceptions.py` & `met_annot_unifier-0.0.5/met_annot_unifier/exceptions.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.4/pyproject.toml` & `met_annot_unifier-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "met-annot-unifier"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Python project to combine tabular outputs from GNPS, Sirius and ISDB"
 authors = ["Pierre-Marie Allard <pierre-marie.allard@unifr.ch>"]
 repository = "https://github.com/mapp-metabolomics-unit/met-annot-unifier"
 documentation = "https://mapp-metabolomics-unit.github.io/met-annot-unifier/"
 readme = "README.md"
 packages = [
   {include = "met_annot_unifier"}
```

### Comparing `met_annot_unifier-0.0.4/PKG-INFO` & `met_annot_unifier-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: met-annot-unifier
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python project to combine tabular outputs from GNPS, Sirius and ISDB
 Home-page: https://github.com/mapp-metabolomics-unit/met-annot-unifier
 Author: Pierre-Marie Allard
 Author-email: pierre-marie.allard@unifr.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

