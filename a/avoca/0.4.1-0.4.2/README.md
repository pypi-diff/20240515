# Comparing `tmp/avoca-0.4.1.tar.gz` & `tmp/avoca-0.4.2.tar.gz`

## Comparing `avoca-0.4.1.tar` & `avoca-0.4.2.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.4.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/export_nas.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/flags.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/io.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/logging.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/manager.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/requirements.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/__init__.py
--rw-r--r--   0        0        0    16458 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/ebas.py
--rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/bindings/gcwerks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/__init__.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/abstract.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/concs.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/generate_classes_doc.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/rt.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/test.py
--rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/qa_class/zscore.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/testing/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/testing/df.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.4.1/avoca/utils/torch_models.py
--rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.4.1/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
--rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.4.1/data/voc_jan2jun_2023.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.4.1/data/.avoca/config.yaml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 avoca-0.4.1/data/tests/missing_area_cols.csv
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/make.bat
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/conf.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/index.rst
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/quickstart.ipynb
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/ebas.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/gcwerks.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.4.1/docs/source/bindings/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/config.yaml
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/data_qa.ipynb
--rw-r--r--   0        0        0   199025 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/data_qa_gcwerks.ipynb
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/export_gc_werks.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/export_gc_werks_secondary_peaks.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.4.1/examples/read_nas.ipynb
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/test_io.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/bindings/gcwerks.dat
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 avoca-0.4.1/tests/bindings/test_gcwerks.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 avoca-0.4.1/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.4.1/LICENCE.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.4.1/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.4.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 avoca-0.4.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/export_nas.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/flags.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/io.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/logging.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/manager.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/requirements.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/bindings/__init__.py
+-rw-r--r--   0        0        0    16450 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/bindings/ebas.py
+-rw-r--r--   0        0        0    12398 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/bindings/gcwerks.py
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/bindings/gcwerks_gui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/__init__.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/abstract.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/concs.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/generate_classes_doc.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/rt.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/test.py
+-rw-r--r--   0        0        0    15855 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/qa_class/zscore.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/testing/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/testing/df.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.4.2/avoca/utils/torch_models.py
+-rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.4.2/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
+-rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.4.2/data/voc_jan2jun_2023.csv
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.4.2/data/.avoca/config.yaml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 avoca-0.4.2/data/tests/missing_area_cols.csv
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/make.bat
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/conf.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/index.rst
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/quickstart.ipynb
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/bindings/ebas.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/bindings/gcwerks.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.4.2/docs/source/bindings/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/config.yaml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/data_qa.ipynb
+-rw-r--r--   0        0        0   199025 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/data_qa_gcwerks.ipynb
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/export_gc_werks.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/export_gc_werks_secondary_peaks.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.4.2/examples/read_nas.ipynb
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 avoca-0.4.2/tests/test_io.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 avoca-0.4.2/tests/bindings/gcwerks.dat
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 avoca-0.4.2/tests/bindings/test_gcwerks.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 avoca-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.4.2/LICENCE.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.4.2/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.4.2/PKG-INFO
```

### Comparing `avoca-0.4.1/.gitlab-ci.yml` & `avoca-0.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/.readthedocs.yaml` & `avoca-0.4.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/flags.py` & `avoca-0.4.2/avoca/flags.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/io.py` & `avoca-0.4.2/avoca/io.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/manager.py` & `avoca-0.4.2/avoca/manager.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/requirements.py` & `avoca-0.4.2/avoca/requirements.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/settings.py` & `avoca-0.4.2/avoca/settings.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/bindings/ebas.py` & `avoca-0.4.2/avoca/bindings/ebas.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,26 +135,25 @@
         "rt": "retention_time",
         "w": "peak_width",
         "area": "peak_area",
     }
 
     metadatas = {}
 
-        
     # Export calibration status if given by the user
     status_col = ("-", "status")
     if status_col in df_export.columns:
         metadata = DataObject()
         metadata.comp_name = "status"
-        metadata.title = "cal"
+        metadata.title = "status"
         metadata.unit = "no unit"
         values = [val for val in df_export[status_col]]
         flags = [[] for _ in df_export[status_col]]
         nas.variables.append(
-            DataObject(values_=values,flags=flags, flagcol=True, metadata=metadata)
+            DataObject(values_=values, flags=flags, flagcol=True, metadata=metadata)
         )
 
     for sub in compounds:
         flags = [
             sorted(flag_all + [flags_to_ebas[f] for f in QA_Flag if f in QA_Flag(flag)])
             for flag in df_export[(sub, "flag")]
         ]
@@ -263,28 +262,28 @@
     compounds = []
 
     for var in nas.variables:
         if "metadata" not in var:
             continue
 
         metadata = var["metadata"]
-        if "comp_name" not in metadata:
-            continue
 
         values = var["values_"]
 
         title = metadata["title"]
 
         # Special variable used for calibration
         if title == "cal":
             calib_ids = np.array(values, dtype=float)
             mask_nan = np.isnan(calib_ids)
             calib_ids[mask_nan] = 0
-            clean_for_df[("-", "calib_id")] = calib_ids.astype(int)
+            clean_for_df[("-", "status")] = calib_ids.astype(int)
 
+        if "comp_name" not in metadata:
+            continue
         # Split the title on the _
         title = title.split("_")
 
         if len(title) != 2:
 
             print("passing", title)
             continue
```

### Comparing `avoca-0.4.1/avoca/bindings/gcwerks.py` & `avoca-0.4.2/avoca/bindings/gcwerks.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,31 @@
     "ht",
     "w",
 ]
 cols_float = cols_have_flags + ["q1_area", "q2_area"]
 cols_zero_is_nan = ["rt"]
 
 
+# allowed variables
+allowed_vars = [
+    "area",
+    "q1_area",
+    "q2_area",
+    "rt",
+    "C",
+    "ht",
+    "w",
+    "norm_ht",
+    "norm_a",
+    "C_ht",
+    "C_a",
+    "C.report",
+]
+
+
 def read_gcwerks(
     file_path: PathLike,
     datetime_format: str = "%y%m%d%H%M",
     runtypes: list[str] = [],
     keep_ordering_from_file: bool = False,
     return_flags: bool = True,
 ) -> pd.DataFrame:
@@ -226,14 +243,15 @@
 
 def export(
     workdir: PathLike,
     gcdir: PathLike,
     compounds: list[str],
     out_file: PathLike,
     date_start: datetime,
+    date_end: datetime | None = None,
     variables: list[str] = ["area", "rt", "C"],
     update: bool = False,
     require_import: bool = False,
     verbose: bool = True,
     use_reported_conc: bool = True,
     gc_bin_dir: str = "/agage/gcwerks-3/bin",
 ):
@@ -242,27 +260,29 @@
     workdir = Path(workdir)
     gcdir = Path(gcdir)
     out_file = Path(out_file)
 
     # The file is in the same directory as this py file
     report_conf = __file__.replace("export_gcwerks.py", "gcwerks-report.conf")
 
-    # allowed variables
-    allowed_vars = [
-        "area",
-        "rt",
-        "C",
-        "ht",
-        "w",
-        "norm_ht",
-        "norm_a",
-        "C_ht",
-        "C_a",
-        "C.report",
-    ]
+    logger.debug(f"Exporting data to {out_file}")
+    logger.debug(f"{variables=}")
+    logger.debug(f"{compounds=}")
+
+    if not variables:
+        raise ValueError("No variables selected")
+    if not compounds:
+        raise ValueError("No compounds selected")
+
+    if date_end is not None:
+        if not date_end > date_start:
+            raise ValueError(
+                f"End date ({date_end}) must be after start date ({date_start})"
+            )
+
     for var in variables:
         if var not in allowed_vars:
             raise ValueError(
                 f"Variable {var} not allowed. Allowed variables are: {allowed_vars}"
             )
 
     if use_reported_conc and "C" in variables:
@@ -284,43 +304,79 @@
         subprocess.run(command_update, shell=True, check=True)
         command_calc = f"{gc_bin_dir}/gccalc -gcdir {gcdir} -1"
         print("Running: ", command_calc)
         subprocess.run(command_calc, shell=True, check=True)
 
     variables_str = " ".join([f"{sub}.{var}" for sub in compounds for var in variables])
 
-    command = (
-        f"{gc_bin_dir}/gcexport "
-        f"-gcdir {gcdir} "
-        # f"-format {report_conf} "
-        f"-mindate {date_start.strftime('%y%m%d')} "
-        f"time type sample {variables_str} "
-        f"> {out_file}"
+    command = " ".join(
+        (
+            f"{gc_bin_dir}/gcexport",
+            f"-gcdir {gcdir}",
+            # f"-format {report_conf}",
+            f"-mindate {date_start.strftime('%y%m%d')}",
+            (f"-maxdate {date_end.strftime('%y%m%d')}" if date_end else ""),
+            "time",
+            "type",
+            "sample",
+            f"{variables_str}",
+            f"> {out_file}",
+        )
     )
     # command = f"gcnetcdf-export -gcdir {gcdir}  -mindate {date_start.strftime('%y%m%d')} time type {variables_str} -exportdir {out_file.parent}"
 
     # Run the command
     print("Running: ", command)
     subprocess.run(command, shell=True, check=True)
 
 
+def get_gcwerks_folders(gcwerks_folders: PathLike = "/agage/") -> list[Path]:
+    """Get the folders in the directory contiaining all gcwerks intruments."""
+
+    gcwerks_folders = Path(gcwerks_folders)
+    if not gcwerks_folders.is_dir():
+        logger = logging.getLogger(__name__)
+        logger.error(f"{gcwerks_folders} is not a directory. Cannot get the folders.")
+        return []
+    return [f for f in gcwerks_folders.iterdir() if f.is_dir()]
+
 
 def read_quats_log(gcdir: PathLike) -> pd.DataFrame:
     """Read the quat.log file from gcwerks."""
 
     # Find where the quat log file is located
-    quat_log_filepath = Path(gcdir) /"results" / "log" / "quat.log"
+    quat_log_filepath = Path(gcdir) / "results" / "log" / "quat.log"
 
     if not quat_log_filepath.exists():
         raise FileNotFoundError(f"File {quat_log_filepath} not found.")
 
-    df = pd.read_csv(quat_log_filepath, sep="\s+", skiprows=1, header=None, names=["dt1", "dt2", "gas", "mean", "mean_s", "blank", "blank_s", "fit_n", "fit_a", "fit_b", "fit_c", "#", "tanks"])
+    df = pd.read_csv(
+        quat_log_filepath,
+        sep="\s+",
+        skiprows=1,
+        header=None,
+        names=[
+            "dt1",
+            "dt2",
+            "gas",
+            "mean",
+            "mean_s",
+            "blank",
+            "blank_s",
+            "fit_n",
+            "fit_a",
+            "fit_b",
+            "fit_c",
+            "#",
+            "tanks",
+        ],
+    )
     # Convert datetime from unix timestamp to datetime
     for col in ["dt1", "dt2"]:
         df[col] = pd.to_datetime(df[col], unit="s")
 
-    # Split the tank column inot the two tanks they contain 
+    # Split the tank column inot the two tanks they contain
     splitted = df["tanks"].str.split("/", expand=True)
     df["sampleQuaternary"] = splitted[0]
     df["sampleTertiary"] = splitted[1]
 
-    return df
+    return df
```

### Comparing `avoca-0.4.1/avoca/qa_class/abstract.py` & `avoca-0.4.2/avoca/qa_class/abstract.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/qa_class/concs.py` & `avoca-0.4.2/avoca/qa_class/concs.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/qa_class/generate_classes_doc.py` & `avoca-0.4.2/avoca/qa_class/generate_classes_doc.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/qa_class/rt.py` & `avoca-0.4.2/avoca/qa_class/rt.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/qa_class/test.py` & `avoca-0.4.2/avoca/qa_class/test.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/qa_class/zscore.py` & `avoca-0.4.2/avoca/qa_class/zscore.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/utils/__init__.py` & `avoca-0.4.2/avoca/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/avoca/utils/torch_models.py` & `avoca-0.4.2/avoca/utils/torch_models.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas` & `avoca-0.4.2/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/data/voc_jan2jun_2023.csv` & `avoca-0.4.2/data/voc_jan2jun_2023.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/data/tests/missing_area_cols.csv` & `avoca-0.4.2/data/tests/missing_area_cols.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/Makefile` & `avoca-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/make.bat` & `avoca-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/source/conf.py` & `avoca-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/source/index.rst` & `avoca-0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/source/quickstart.ipynb` & `avoca-0.4.2/docs/source/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/docs/source/bindings/ebas.md` & `avoca-0.4.2/docs/source/bindings/ebas.md`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/examples/data_qa.ipynb` & `avoca-0.4.2/examples/data_qa.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/examples/data_qa_gcwerks.ipynb` & `avoca-0.4.2/examples/data_qa_gcwerks.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/examples/export_gc_werks.py` & `avoca-0.4.2/examples/export_gc_werks.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/examples/export_gc_werks_secondary_peaks.py` & `avoca-0.4.2/examples/export_gc_werks_secondary_peaks.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/examples/read_nas.ipynb` & `avoca-0.4.2/examples/read_nas.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/tests/test_io.py` & `avoca-0.4.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/LICENCE.txt` & `avoca-0.4.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `avoca-0.4.1/pyproject.toml` & `avoca-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "avoca"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Lionel Constantin", email="lionel.constantin@empa.ch" },
 ]
 description = "@voc@: Quality assessement of measurement data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avoca-0.4.1/PKG-INFO` & `avoca-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avoca
-Version: 0.4.1
+Version: 0.4.2
 Summary: @voc@: Quality assessement of measurement data
 Project-URL: Homepage, https://gitlab.com/empa503/atmospheric-measurements/avoca
 Project-URL: Bug Tracker, https://gitlab.com/empa503/atmospheric-measurements/avoca/-/issues
 Project-URL: Documentation, http://avoca.readthedocs.io/
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>
 License-File: LICENCE.txt
 Classifier: License :: OSI Approved :: MIT License
```

