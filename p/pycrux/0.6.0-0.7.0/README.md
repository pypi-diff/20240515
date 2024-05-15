# Comparing `tmp/pycrux-0.6.0.tar.gz` & `tmp/pycrux-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrux-0.6.0.tar", max compression
+gzip compressed data, was "pycrux-0.7.0.tar", max compression
```

## Comparing `pycrux-0.6.0.tar` & `pycrux-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.6.0/LICENSE
--rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.6.0/pycrux/__init__.py
--rw-r--r--   0        0        0     6507 2023-05-31 12:31:40.113940 pycrux-0.6.0/pycrux/crux.py
--rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.6.0/pycrux/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.6.0/pycrux/utils/config.py
--rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.6.0/pycrux/utils/logger.py
--rw-r--r--   0        0        0      959 2023-05-31 12:32:26.591794 pycrux-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pycrux-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-13 07:38:17.256480 pycrux-0.7.0/LICENSE
+-rw-r--r--   0        0        0       85 2024-01-13 07:38:18.051617 pycrux-0.7.0/pycrux/__init__.py
+-rw-r--r--   0        0        0     8486 2024-05-15 08:38:42.631594 pycrux-0.7.0/pycrux/crux.py
+-rw-r--r--   0        0        0      148 2024-05-15 08:35:59.116044 pycrux-0.7.0/pycrux/pipes.py
+-rw-r--r--   0        0        0        0 2024-01-13 07:38:18.052337 pycrux-0.7.0/pycrux/utils/__init__.py
+-rw-r--r--   0        0        0      600 2024-01-13 07:38:18.052193 pycrux-0.7.0/pycrux/utils/config.py
+-rw-r--r--   0        0        0      731 2024-01-13 07:38:18.053865 pycrux-0.7.0/pycrux/utils/logger.py
+-rw-r--r--   0        0        0      923 2024-05-15 08:42:02.481882 pycrux-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 pycrux-0.7.0/PKG-INFO
```

### Comparing `pycrux-0.6.0/LICENSE` & `pycrux-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrux-0.6.0/pycrux/crux.py` & `pycrux-0.7.0/pycrux/crux.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,147 @@
 import glob
 import os
 import subprocess
 from pathlib import Path
 from subprocess import CompletedProcess
 
-import pandas as pd
+import polars as pl
 
+from pycrux.pipes import drop_row_that_is_all_null
 from pycrux.utils.logger import logger
 
 
 class Crux:
     def __init__(self, crux_common_root_folder: str):
         root = Path(os.path.expanduser(crux_common_root_folder))
         self._raise_if_folder_does_not_exist(root)
         self.root: Path = root
-        self._bin_crFitTool: Path = self.root / """tools/crFitTool/bin/crFitTool"""
+        self._bin_crFitTool: Path = (
+            self.root / """tools/crFitTool/bin/crFitTool"""
+        )
 
     def read_fit(
-        self, fit_file: str, to_log: bool = False, ending: str = ".records.csv"
-    ) -> pd.DataFrame:
+        self,
+        fit_file: str,
+        to_log: bool = False,
+        ending: str = ".records.csv",
+        clean: bool = False,
+        move_to_folder: bool = False,
+        folder_suffix: str = "_csv",
+    ) -> pl.DataFrame:
         """Return the records for a given .fit file.
 
         Parameters
         ----------
         fit_file : str
             Path to a .fit file.
         to_log : bool, optional
             Whether or not to log information, by default False
         ending : str, optional
             Suffix that `crux` appends to the .fit files, by default ".records.csv"
+        cleanup: bool, optional
+            Whether or not to remove the .csv file after reading it, by default False
 
         Returns
         -------
-        pd.DataFrame
-            A `pandas` data frame containing the records data.
+        pl.DataFrame
+            A `polars` data frame containing the records data.
         """
         self.crfittool(fit_file=fit_file, to_log=to_log)
-        return pd.read_csv(fit_file + ending)
+        df = pl.read_csv(fit_file + ending).pipe(drop_row_that_is_all_null)
+        if clean:
+            self.cleanup(fit_file)
+        else:
+            if move_to_folder:
+                self.move_to_folder(fit_file, folder_suffix)
+        return df
+
+    def move_to_folder(self, fit_file: str, folder_suffix: str) -> None:
+        """Moves the created .csv files to a folder.
+
+        Parameters
+        ----------
+        fit_file : str
+            The name of the .fit file.
+        folder_suffix : str
+            The suffix to append to the folder name.
+        """
+        file = Path(os.path.expanduser(fit_file))
+        # remove the .fit and add the suffix
+        folder = file.with_suffix("").as_posix() + folder_suffix
+
+        # try to create the folder if it does not exist
+        try:
+            os.makedirs(folder)
+        except FileExistsError:
+            pass
+
+        for created_file in glob.glob(f"{file}.*.csv"):
+            # Move file
+            try:
+                os.rename(
+                    created_file,
+                    os.path.join(folder, os.path.basename(created_file)),
+                )
+            except Exception as e:
+                logger.error(f"Could not move {created_file}: {e}")
+
+    def cleanup(self, fit_file: str) -> None:
+        """Remove the .csv file created by `crFitTool`.
+
+        Parameters
+        ----------
+        fit_file : str
+            The name of the .fit file.
+        """
+        file = Path(os.path.expanduser(fit_file))
+
+        # Get all files of the format `fit_file.*.csv`.
+        for created_file in glob.glob(f"{file}.*.csv"):
+            # Try to safely remove the file.
+            try:
+                os.remove(created_file)
+            except Exception as e:
+                logger.error(f"Could not remove {created_file}: {e}")
 
     def read_fit_recursively(
         self, root: str, to_log: bool = True, ending: str = ".records.csv"
-    ) -> dict[str, pd.DataFrame]:
+    ) -> dict[str, pl.DataFrame]:
         """Runs read_fit on all .fit files found recursively inside the root folder.
 
         Parameters
         ----------
         root : str
             Root folder in which to look for .fit files.
         to_log : bool, optional
             Whether or not to log information, by default True
         ending : str, optional
             Suffix that `crux` appends to the .fit files, by default ".records.csv"
 
         Returns
         -------
-        dict[str, pd.DataFrame]
+        dict[str, pl.DataFrame]
             A dictionary where the keys are the location of the .fit files, and
             the items are the data frames containing the records.
         """
         fit_files = self.get_all_files_in_folder(root)
-        dict_of_dataframes: dict[str, pd.DataFrame] = {}
+        dict_of_dataframes: dict[str, pl.DataFrame] = {}
         for fit_file in fit_files:
             try:
-                df = self.read_fit(fit_file=fit_file, to_log=to_log, ending=ending)
+                df = self.read_fit(
+                    fit_file=fit_file, to_log=to_log, ending=ending
+                )
                 dict_of_dataframes[fit_file] = df
             except Exception as e:
                 logger.error(f"Could not parse {fit_file}: {e}")
         return dict_of_dataframes
 
-    def crfittool(self, fit_file: str, to_log: bool = False) -> CompletedProcess[str]:
+    def crfittool(
+        self, fit_file: str, to_log: bool = False
+    ) -> CompletedProcess[str]:
         """Run crFitTool.
 
         Parameters
         ----------
         fit_file : str
             The .fit file to parse.
         to_log : bool, optional
@@ -85,28 +154,27 @@
             and the stderr.
 
         Raises
         ------
         Exception
             Raises an exception if `fit_file` is not a .fit file.
         """
-        # TODO: Add cleanup flag that removes the created .csv files.
-        # TODO: Add a `safe` flag that when true does not run crux if the corresponding
-        #       records exist already.
         if not fit_file.endswith("fit"):
-            raise Exception(f"Can only parse .fit files, got {fit_file}")
+            raise ValueError(f"Can only parse .fit files, got {fit_file}")
 
         file = Path(os.path.expanduser(fit_file))
         self._raise_if_file_does_not_exist(file)
 
         f = file.as_posix()
         command = f"""{self._bin_crFitTool} --in "{f}" --csv "{f}" """
         if to_log:
             logger.info(f"Running: {command}")
-        result = subprocess.run([command], shell=True, capture_output=True, text=True)
+        result = subprocess.run(
+            [command], shell=True, capture_output=True, text=True
+        )
         if to_log:
             logger.info(result)
         return result
 
     def crfittool_recursively(
         self, root: str, to_log: bool = True
     ) -> list[CompletedProcess[str]]:
```

### Comparing `pycrux-0.6.0/pycrux/utils/config.py` & `pycrux-0.7.0/pycrux/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.6.0/pycrux/utils/logger.py` & `pycrux-0.7.0/pycrux/utils/logger.py`

 * *Files identical despite different names*

