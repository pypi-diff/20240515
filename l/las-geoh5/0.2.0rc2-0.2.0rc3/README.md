# Comparing `tmp/las_geoh5-0.2.0rc2.tar.gz` & `tmp/las_geoh5-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las_geoh5-0.2.0rc2.tar", max compression
+gzip compressed data, was "las_geoh5-0.2.0rc3.tar", max compression
```

## Comparing `las_geoh5-0.2.0rc2.tar` & `las_geoh5-0.2.0rc3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0      702 2024-05-02 20:02:14.201504 las_geoh5-0.2.0rc2/las_geoh5/__init__.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc2/las_geoh5/export_files/__init__.py
--rw-r--r--   0        0        0     1734 2024-04-23 21:10:39.082255 las_geoh5-0.2.0rc2/las_geoh5/export_files/driver.py
--rw-r--r--   0        0        0     1264 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc2/las_geoh5/export_files/uijson.py
--rw-r--r--   0        0        0     6748 2024-04-23 21:11:17.349111 las_geoh5-0.2.0rc2/las_geoh5/export_las.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc2/las_geoh5/import_directories/__init__.py
--rw-r--r--   0        0        0     2104 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc2/las_geoh5/import_directories/driver.py
--rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc2/las_geoh5/import_directories/uijson.py
--rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc2/las_geoh5/import_files/__init__.py
--rw-r--r--   0        0        0     4632 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/driver.py
--rw-r--r--   0        0        0     1468 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/params.py
--rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc2/las_geoh5/import_files/uijson.py
--rw-r--r--   0        0        0    13319 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/import_las.py
--rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/uijson/__init__.py
--rw-r--r--   0        0        0     2119 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc2/las_geoh5/uijson/write_uijson.py
--rw-r--r--   0        0        0      122 2024-04-23 21:10:39.087480 las_geoh5-0.2.0rc2/las_geoh5-assets/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-02 03:50:51.043275 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/export_las_files.ui.json
--rw-r--r--   0        0        0      976 2024-05-02 03:50:51.044307 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_directories.ui.json
--rw-r--r--   0        0        0     2656 2024-05-02 03:50:51.045439 las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_files.ui.json
--rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 las_geoh5-0.2.0rc2/LICENSE
--rw-r--r--   0        0        0     2742 2024-05-02 20:02:14.185918 las_geoh5-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4992 2024-04-26 06:14:29.001844 las_geoh5-0.2.0rc2/README.rst
--rw-r--r--   0        0        0     6327 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      702 2024-05-13 19:27:23.598067 las_geoh5-0.2.0rc3/las_geoh5/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.081155 las_geoh5-0.2.0rc3/las_geoh5/export_files/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-14 20:25:48.897070 las_geoh5-0.2.0rc3/las_geoh5/export_files/driver.py
+-rw-r--r--   0        0        0     1264 2024-05-14 18:03:54.730380 las_geoh5-0.2.0rc3/las_geoh5/export_files/uijson.py
+-rw-r--r--   0        0        0     6748 2024-05-14 18:18:52.463471 las_geoh5-0.2.0rc3/las_geoh5/export_las.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.083315 las_geoh5-0.2.0rc3/las_geoh5/import_directories/__init__.py
+-rw-r--r--   0        0        0     2300 2024-05-14 20:25:48.898069 las_geoh5-0.2.0rc3/las_geoh5/import_directories/driver.py
+-rw-r--r--   0        0        0     1057 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc3/las_geoh5/import_directories/uijson.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:10:39.084314 las_geoh5-0.2.0rc3/las_geoh5/import_files/__init__.py
+-rw-r--r--   0        0        0     5797 2024-05-14 20:56:13.468616 las_geoh5-0.2.0rc3/las_geoh5/import_files/driver.py
+-rw-r--r--   0        0        0     1468 2024-05-14 18:03:54.747566 las_geoh5-0.2.0rc3/las_geoh5/import_files/params.py
+-rw-r--r--   0        0        0     3080 2024-04-23 21:10:39.085372 las_geoh5-0.2.0rc3/las_geoh5/import_files/uijson.py
+-rw-r--r--   0        0        0    13319 2024-05-14 18:03:54.762581 las_geoh5-0.2.0rc3/las_geoh5/import_las.py
+-rw-r--r--   0        0        0      237 2024-05-13 17:12:35.795341 las_geoh5-0.2.0rc3/las_geoh5/scripts/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-14 16:07:37.620031 las_geoh5-0.2.0rc3/las_geoh5/scripts/geoh5_to_las.py
+-rw-r--r--   0        0        0     1826 2024-05-14 16:07:37.539510 las_geoh5-0.2.0rc3/las_geoh5/scripts/las_to_geoh5.py
+-rw-r--r--   0        0        0      122 2024-04-23 21:10:39.086374 las_geoh5-0.2.0rc3/las_geoh5/uijson/__init__.py
+-rw-r--r--   0        0        0     2119 2024-05-14 18:03:54.739474 las_geoh5-0.2.0rc3/las_geoh5/uijson/write_uijson.py
+-rw-r--r--   0        0        0      122 2024-05-14 04:22:36.345473 las_geoh5-0.2.0rc3/las_geoh5-assets/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-02 03:50:51.043275 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/export_las_files.ui.json
+-rw-r--r--   0        0        0      976 2024-05-02 03:50:51.044307 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_directories.ui.json
+-rw-r--r--   0        0        0     2656 2024-05-02 03:50:51.045439 las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_files.ui.json
+-rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 las_geoh5-0.2.0rc3/LICENSE
+-rw-r--r--   0        0        0     2875 2024-05-13 19:29:43.964478 las_geoh5-0.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5588 2024-05-14 04:13:37.741819 las_geoh5-0.2.0rc3/README.rst
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 las_geoh5-0.2.0rc3/PKG-INFO
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/__init__.py` & `las_geoh5-0.2.0rc3/las_geoh5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # flake8: noqa
 
 from __future__ import annotations
 
 from pathlib import Path
 
-__version__ = "0.2.0-rc.2"
+__version__ = "0.2.0-rc.3"
 
 
 def assets_path() -> Path:
     """Return the path to the assets folder."""
 
     parent = Path(__file__).parent
     folder_name = f"{parent.name}-assets"
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/export_files/driver.py` & `las_geoh5-0.2.0rc3/las_geoh5/export_files/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,39 +16,50 @@
 from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import InputFile
 from tqdm import tqdm
 
 from las_geoh5.export_las import drillhole_to_las
 
 
-def run(file: str | Path):
-    ifile = InputFile.read_ui_json(file)
+def run(params_json: str | Path, output_dir: str | Path | None = None):
+    """
+    Export drillhole data from GEOH5 to LAS.
+
+    :param params_json: The JSON file with export parameters, with references to the input
+        GEOH5 file, and an output directory for LAS.
+    :param output_dir: if specified, use this path as the directory to write out the resulting
+        LAS files, instead of the ``rootpath`` location defined by the parameter file.
+    """
+    ifile = InputFile.read_ui_json(params_json)
     dh_group = ifile.data["drillhole_group"]
-    rootpath = Path(ifile.data["rootpath"])
+    if output_dir is not None:
+        rootpath = output_dir
+    else:
+        rootpath = Path(ifile.data["rootpath"])
     use_directories = ifile.data["use_directories"]
     with fetch_active_workspace(ifile.data["geoh5"]):
         export_las_files(dh_group, rootpath, use_directories)
 
 
 def export_las_files(
     group: DrillholeGroup, basepath: str | Path, use_directories: bool = True
 ):
     """
-    Export contents of drillhole group to las files organized by directories.
+    Export contents of drillhole group to LAS files organized by directories.
 
     :param group: Drillhole group container.
     :param basepath: Base path where directories/files will be created.
-    :param use_directories: Use directories to organize las files by property group.
+    :param use_directories: Use directories to organize LAS files by property group.
     """
 
     if isinstance(basepath, str):
         basepath = Path(basepath)
 
     drillholes = [k for k in group.children if isinstance(k, Drillhole)]
 
-    print(f"Exporting drillhole surveys and property group data to {str(basepath)}")
+    print(f"Exporting drillhole surveys and property group data to '{str(basepath)}'")
     for drillhole in tqdm(drillholes):
         drillhole_to_las(drillhole, basepath, use_directories=use_directories)
 
 
 if __name__ == "__main__":
     run(sys.argv[1])
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/export_files/uijson.py` & `las_geoh5-0.2.0rc3/las_geoh5/export_files/uijson.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,12 +31,12 @@
             "fileType": ["directory"],
             "value": None,
             "directoryOnly": True,
         },
         "use_directories": {
             "main": True,
             "label": "Use directories",
-            "tooltip": "Organize las files by property group directories",
+            "tooltip": "Organize LAS files by property group directories",
             "value": True,
         },
     },
 )
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/export_las.py` & `las_geoh5-0.2.0rc3/las_geoh5/export_las.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def add_well_data(
     file: LASFile,
     drillhole: Drillhole,
 ) -> LASFile:
     """
-    Populate las file well data from drillhole.
+    Populate LAS file well data from drillhole.
 
     :param file: lasio file object.
     :param drillhole: geoh5py drillhole object.
 
     :returns: Updated lasio file object.
     """
 
@@ -48,15 +48,15 @@
     file.well.append(HeaderItem(mnemonic="ELEV", value=float(drillhole.collar["z"])))
 
     return file
 
 
 def add_curve_data(file: LASFile, drillhole: Drillhole, group):
     """
-    Populate las file with curve data from each property in group.
+    Populate LAS file with curve data from each property in group.
 
     :param file: lasio file object.
     :param drillhole: geoh5py.drillhole object containing property
         groups for collocated data.
     :param group: Property group containing collocated float data
         objects of 'drillhole'.
     """
@@ -90,18 +90,18 @@
     return file
 
 
 def add_survey_data(file: LASFile, drillhole: Drillhole) -> LASFile:
     """
     Add drillhole survey data to LASFile object.
 
-    :param file: las file object.
+    :param file: LAS file object.
     :param drillhole: drillhole containing survey data.
 
-    :return: Updated las file object.
+    :return: Updated LAS file object.
     """
 
     # Add survey data
     file.append_curve("DEPTH", drillhole.surveys[:, 0], unit="m")
     file.append_curve(
         "DIP",
         drillhole.surveys[:, 1],
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_directories/driver.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_directories/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,46 +20,50 @@
 from las_geoh5.import_las import las_to_drillhole
 
 
 def run(file: str):
     ifile = InputFile.read_ui_json(file)
     dh_group = ifile.data["drillhole_group"]
     parent_folder = ifile.data["parent_folder"]
+    if not parent_folder:
+        raise ValueError("No folder specified to read LAS files from.")
     with fetch_active_workspace(ifile.data["geoh5"], mode="a"):
         import_las_directory(dh_group, parent_folder)
 
 
 def import_las_directory(dh_group: DrillholeGroup, basepath: str | Path):
     """
     Import directory/files from previous export.
 
     :param workspace: Project workspace.
-    :param basepath: Root directory for las data.
+    :param basepath: Root directory for LAS data.
 
     :return: New drillhole group containing imported items.
     """
 
     if isinstance(basepath, str):
         basepath = Path(basepath)
 
     if not basepath.exists():
-        raise OSError(f"Path {str(basepath)} does not exist.")
+        raise OSError(f"Directory does not exist: {basepath}")
+    if not basepath.is_dir():
+        raise OSError(f"Path is not a directory: {basepath}")
 
     surveys_path = basepath / "Surveys"
     surveys = list(surveys_path.iterdir()) if surveys_path.exists() else None
 
     property_group_folders = [
         p for p in basepath.iterdir() if p.is_dir() and p.name != "Surveys"
     ]
 
     for prop in property_group_folders:
         lasfiles = []
         for file in [k for k in prop.iterdir() if k.suffix == ".las"]:
             lasfiles.append(lasio.read(file, mnemonic_case="preserve"))
-        print(f"Importing property group data from to {prop.name}")
+        print(f"Importing property group data from to '{prop.name}'")
         las_to_drillhole(
             lasfiles,
             dh_group,
             prop.name,
             surveys,
             options=ImportOptions(),
         )
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_directories/uijson.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_directories/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_files/driver.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_files/driver.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,148 +6,160 @@
 #  (see LICENSE file at the root of this source code package).
 #
 
 from __future__ import annotations
 
 import logging
 import sys
+from collections.abc import Iterator
+from contextlib import contextmanager
+from datetime import datetime
 from multiprocessing import Pool
 from pathlib import Path
 from shutil import move
-from time import time
 
 import lasio
 from geoh5py import Workspace
 from geoh5py.shared.utils import fetch_active_workspace
 from geoh5py.ui_json import InputFile
 from tqdm import tqdm
 
 from las_geoh5.import_files.params import ImportOptions, NameOptions
 from las_geoh5.import_las import las_to_drillhole
 
+_logger = logging.getLogger(__name__)
+_logger.name = "Import Files"
 
-def get_logger(
-    name: str, level: int = logging.INFO, path: str | Path | None = None
-) -> logging.Logger:
-    """
-    Create a looger with stream and optional file handlers.
 
-    :param name: Logger name.
-    :param level: logging level.
-    :param path: Creates a file handler at the specified path if not None.
-    :return: Logger object.
+@contextmanager
+def log_to_file(
+    logger: logging.Logger, log_dir: Path, log_level: int = logging.INFO
+) -> Iterator[Path]:
     """
-    if isinstance(path, str):
-        path = Path(path)
-
-    logger = logging.getLogger(name)
-    logger.setLevel(level)
-    formatter = logging.Formatter(
-        "%(asctime)s : %(name)s : %(levelname)s : %(message)s"
-    )
+    Configure the given logger with file handler at the given path.
 
-    stream_handler = logging.StreamHandler()
-    stream_handler.setFormatter(formatter)
-    stream_handler.setLevel(level)
-    logger.addHandler(stream_handler)
-
-    if path is not None:
-        filename = f"{'_'.join([k.lower() for k in name.split(' ')])}.log"
-        file_handler = logging.FileHandler(path / filename)
-        file_handler.setFormatter(formatter)
-        file_handler.setLevel(level)
-        logger.addHandler(file_handler)
+    :param logger: The logger object.
+    :param log_dir: The directory where to create the log file.
+    :param log_level: The log level to set for the file handler.
+    """
 
-    return logger
+    log_file = log_dir / (_logger.name.lower().replace(" ", "_") + ".log")
 
+    original_level = logger.level
+    logger.setLevel(
+        log_level if original_level == 0 else min(original_level, log_level)
+    )
+    file_handler = logging.FileHandler(log_file, encoding="utf-8")
+    file_handler.setLevel(log_level)
+    logger.addHandler(file_handler)
+    try:
+        yield log_file
+    finally:
+        file_handler.close()
+        logger.removeHandler(file_handler)
+        logger.setLevel(original_level)
+
+
+@contextmanager
+def log_execution_time(message: str, log_level: int = logging.INFO) -> Iterator[None]:
+    start = datetime.now()
+
+    # no exception handling: only display message if no exception happened
+    yield
+
+    elapsed = (datetime.now() - start).total_seconds()
+    minutes = int(elapsed / 60)
+    seconds = elapsed - 60 * minutes
 
-def elapsed_time_logger(start, end, message):
-    if message[-1] != ".":
+    message = message.strip()
+    if message and message[-1] != ".":
         message += "."
 
-    elapsed = end - start
-    minutes = elapsed // 60
-    seconds = elapsed % 60
-
+    prefix_msg = f"{message} Time elapsed:"
     if minutes >= 1:
-        out = f"{message} Time elapsed: {minutes}m {seconds}s."
+        out = f"{prefix_msg} {minutes}m {seconds:.0f}s."
     else:
-        out = f"{message} Time elapsed: {seconds:.2f}s."
+        out = f"{prefix_msg} {seconds:.2f}s."
 
-    return out
+    _logger.log(log_level, out)
 
 
-def run(filepath: Path):  # pylint: disable=too-many-locals
-    start = time()
-    ifile = InputFile.read_ui_json(filepath)
-
-    logger = get_logger("Import Files", path=filepath.parent)
-    logger.info(
-        "Importing las file data to workspace %s.geoh5.",
-        ifile.data["geoh5"].h5file.stem,
-    )
+def run(params_json: Path, output_geoh5: Path | None = None):
+    """
+    Import LAS files into a geoh5 file.
 
-    workspace = Workspace()
-    begin_reading = time()
+    :param params_json: The JSON file with import parameters, with references to the input
+        LAS files, and an input GEOH5 file (``geoh5`` in parameters) that contains the
+        destination drill hole group.
+        For output, will either write the created GEOH5 with a timestamped name to
+        ``monitoring_directory``, if defined, or overwrite the input GEOH5 file.
+    :param output_geoh5: if specified, use this path to write out the resulting GEOH5 file,
+        instead of the GEOH5 output location defined by the parameter file.
+    """
 
-    with Pool() as pool:
-        futures = []
-        for file in tqdm(ifile.data["files"].split(";"), desc="Reading las files"):
-            futures.append(
-                pool.apply_async(lasio.read, (file,), {"mnemonic_case": "preserve"})
+    with log_to_file(_logger, params_json.parent) as log_file:
+        with log_execution_time("All done"):
+            ifile = InputFile.read_ui_json(params_json)
+
+            _logger.info(
+                "Importing LAS file data to workspace '%s.geoh5'.",
+                ifile.data["geoh5"].h5file.stem,
             )
 
-        lasfiles = [future.get() for future in futures]
-
-    end_reading = time()
-    logger.info(
-        elapsed_time_logger(begin_reading, end_reading, "Finished reading las files")
-    )
-
-    with fetch_active_workspace(ifile.data["geoh5"]) as geoh5:
-        dh_group = geoh5.get_entity(ifile.data["drillhole_group"].uid)[0]
-        dh_group = dh_group.copy(parent=workspace)
-
-    logger.info(
-        "Saving drillhole data into drillhole group %s under property group %s",
-        dh_group.name,
-        ifile.data["name"],
-    )
-    begin_saving = time()
-
-    name_options = NameOptions(**ifile.data)
-    import_options = ImportOptions(names=name_options, **ifile.data)
-    las_to_drillhole(
-        lasfiles,
-        dh_group,
-        ifile.data["name"],
-        options=import_options,
-    )
-    end_saving = time()
-    logger.info(
-        elapsed_time_logger(begin_saving, end_saving, "Finished saving drillhole data")
-    )
-    end = time()
-    logger.info(elapsed_time_logger(start, end, "All done."))
-    logpath = Path(logger.handlers[1].baseFilename)  # type: ignore
-    dh_group.add_file(logpath)
-    logger.handlers[1].close()
-    logpath.unlink()
+            workspace = Workspace()
+            with log_execution_time("Finished reading LAS files"):
+                with Pool() as pool:
+                    futures = []
+                    for file in tqdm(
+                        ifile.data["files"].split(";"), desc="Reading LAS files"
+                    ):
+                        futures.append(
+                            pool.apply_async(
+                                lasio.read, (file,), {"mnemonic_case": "preserve"}
+                            )
+                        )
+
+                    lasfiles = [future.get() for future in futures]
+
+            with fetch_active_workspace(ifile.data["geoh5"]) as geoh5:
+                dh_group = geoh5.get_entity(ifile.data["drillhole_group"].uid)[0]
+                dh_group = dh_group.copy(parent=workspace)
+
+            _logger.info(
+                "Saving drillhole data into drillhole group '%s' under property group '%s'",
+                dh_group.name,
+                ifile.data["name"],
+            )
 
-    if ifile.data["monitoring_directory"]:
+            with log_execution_time("Finished saving drillhole data"):
+                name_options = NameOptions(**ifile.data)
+                las_to_drillhole(
+                    lasfiles,
+                    dh_group,
+                    ifile.data["name"],
+                    options=ImportOptions(names=name_options, **ifile.data),
+                )
+
+    if log_file.exists() and log_file.stat().st_size > 0:
+        dh_group.add_file(log_file)
+    log_file.unlink(missing_ok=True)
+
+    if output_geoh5 is not None:
+        output_geoh5.unlink(missing_ok=True)
+        workspace.save_as(output_geoh5)
+    elif ifile.data["monitoring_directory"]:
         working_path = Path(ifile.data["monitoring_directory"]) / ".working"
         working_path.mkdir(exist_ok=True)
-        temp_geoh5 = f"temp{time():.3f}.geoh5"
+        temp_geoh5 = f"temp{datetime.now().timestamp():.3f}.geoh5"
         workspace.save_as(working_path / temp_geoh5)
         workspace.close()
         move(
             working_path / temp_geoh5,
             Path(ifile.data["monitoring_directory"]) / temp_geoh5,
         )
-
     else:
         geoh5_path = geoh5.h5file
         geoh5.h5file.unlink()
         workspace.save_as(geoh5_path)
 
     workspace.close()
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_files/params.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_files/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "collar_y_name": "Y",
     "collar_z_name": "ELEV",
 }
 
 
 class NameOptions(BaseModel):
     """
-    Stores options for naming of dillhole parameters in las files.
+    Stores options for naming of dillhole parameters in LAS files.
 
     :param collar_x_name: Name of the collar x field.
     :param collar_y_name: Name of the collar y field.
     :param collar_z_name: Name of the collar z field.
     """
 
     well_name: str = "WELL"
@@ -34,15 +34,15 @@
         return {k: v for k, v in data.items() if v is not None}
 
 
 class ImportOptions(BaseModel):
     """
     Stores options for the drillhole import.
 
-    :param names: Options for naming of dillhole parameters in las files.
+    :param names: Options for naming of dillhole parameters in LAS files.
     :param collocation_tolerance: Tolerance for collocation of collar and depth data.
     :param warnings: Whether to show warnings.
     :param skip_empty_header: Whether to skip empty headers.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_files/uijson.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_files/uijson.py`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/import_las.py` & `las_geoh5-0.2.0rc3/las_geoh5/import_las.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,46 +32,46 @@
 
     def translate(self, field: str):
         """
         Return translated field name or rais KeyError if field not recognized.
 
         :param field: Standardized field name.
 
-        :return: Name of corresponding field in las file.
+        :return: Name of corresponding field in LAS file.
         """
         if field not in dict(self.names):
             raise KeyError(f"'{field}' is not a recognized field.")
 
         return getattr(self.names, field)
 
     def retrieve(self, field: str, lasfile: lasio.LASFile):
         """
-        Access las data using translation.
+        Access LAS data using translation.
 
         :param field: Name of field to retrieve.
         :param lasfile: lasio file object.
 
-        :return: data stored in las file under translated field name.
+        :return: data stored in LAS file under translated field name.
         """
         if getattr(self.names, field) in lasfile.well:
             out = lasfile.well[getattr(self.names, field)].value
         elif getattr(self.names, field) in lasfile.curves:
             out = lasfile.curves[getattr(self.names, field)].data
         elif getattr(self.names, field) in lasfile.params:
             out = lasfile.params[getattr(self.names, field)].value
         else:
-            msg = f"'{field}' field: '{getattr(self.names, field)}' not found in las file."
+            msg = f"'{field}' field: '{getattr(self.names, field)}' not found in LAS file."
             raise KeyError(msg)
 
         return out
 
 
 def get_depths(lasfile: lasio.LASFile) -> dict[str, np.ndarray]:
     """
-    Get depth data from las file.
+    Get depth data from LAS file.
 
     :param lasfile: Las file object.
 
     :return: Depth data as 'from-to' interval or 'depth' locations.
     """
 
     depths = None
@@ -98,18 +98,18 @@
 
 def get_collar(
     lasfile: lasio.LASFile,
     translator: LASTranslator | None = None,
     logger: logging.Logger | None = None,
 ) -> list:
     """
-    Returns collar data from las file or None if data missing.
+    Returns collar data from LAS file or None if data missing.
 
     :param lasfile: Las file object.
-    :param translator: Translator for las file.
+    :param translator: Translator for LAS file.
     :param logger: Logger object if warnings are enabled.
 
     :return: Collar data.
     """
 
     if translator is None:
         translator = LASTranslator(names=NameOptions())
@@ -125,15 +125,15 @@
                 k.mnemonic
                 for k in lasfile.well
                 if k.value and k.mnemonic not in exclusions
             ]
             if logger is not None:
                 logger.warning(
                     f"{field.replace('_', ' ').capitalize()} field "
-                    f"'{getattr(translator.names, field)}' not found in las file."
+                    f"'{getattr(translator.names, field)}' not found in LAS file."
                     f" Setting coordinate to 0.0. Non-null header fields include: "
                     f"{options}."
                 )
 
             collar_coord = 0.0
 
         try:
@@ -165,15 +165,15 @@
 
 def add_survey(
     survey: str | Path,
     drillhole: ConcatenatedDrillhole,
     logger: logging.Logger | None = None,
 ) -> ConcatenatedDrillhole:
     """
-    Import survey data from csv or las format and add to drillhole.
+    Import survey data from CSV or LAS format and add to drillhole.
 
     :param survey: Path to a survey file stored as .csv or .las format.
     :param drillhole: Drillhole object to append data to.
     :param logger: logger object if warning are enabled.
 
     :return: Updated drillhole object.
     """
@@ -212,15 +212,15 @@
 def add_data(
     drillhole: ConcatenatedDrillhole,
     lasfile: lasio.LASFile,
     group_name: str,
     collocation_tolerance: float = 0.01,
 ) -> ConcatenatedDrillhole:
     """
-    Add data from las file curves to drillhole.
+    Add data from LAS file curves to drillhole.
 
     :param drillhole: Drillhole object to append data to.
     :param lasfile: Las file object.
     :param group_name: Property group name.
     :param collocation_tolerance: Tolerance for determining collocation of data.
 
     :return: Updated drillhole object.
@@ -294,28 +294,28 @@
 ) -> ConcatenatedDrillhole:
     """
     Create a drillhole or append data to drillhole if it exists in workspace.
 
     :param lasfile: Las file object.
     :param drillhole_group: Drillhole group container.
     :param group_name: Property group name.
-    :param translator: Translator for las file.
+    :param translator: Translator for LAS file.
     :param collocation_tolerance: Tolerance for determining collocation of data.
     :param logger: Logger object if warnings are enabled.
 
     :return: Created or augmented drillhole.
     """
 
     if translator is None:
         translator = LASTranslator(NameOptions())
 
     name = translator.retrieve("well_name", lasfile)
     if not name and logger is not None:
         logger.warning(
-            "No well name provided for las file. "
+            "No well name provided for LAS file. "
             "Saving drillhole with name 'Unknown'."
         )
 
     collar = get_collar(lasfile, translator, logger)
     drillhole = drillhole_group.get_entity(name)[0]  # type: ignore
 
     if not isinstance(drillhole, Drillhole) or (
@@ -349,15 +349,15 @@
     drillhole_group: DrillholeGroup,
     property_group: str,
     survey: Path | list[Path] | None = None,
     logger: logging.Logger | None = None,
     options: ImportOptions | None = None,
 ):
     """
-    Import a las file containing collocated datasets for a single drillhole.
+    Import a LAS file containing collocated datasets for a single drillhole.
 
     :param data: Las file(s) containing drillhole data.
     :param drillhole_group: Drillhole group container.
     :param property_group: Property group name.
     :param survey: Path to a survey file stored as .csv or .las format.
     :param logger: Logger object if warnings are enabled.
     :param options: Import options covering name translations, collocation
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5/uijson/write_uijson.py` & `las_geoh5-0.2.0rc3/las_geoh5/uijson/write_uijson.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from pathlib import Path
 
 from geoh5py.ui_json import InputFile
 
 
 def write_uijson(basepath: str | Path, mode: str = "import_files"):
     """
-    Write a ui.json file for either import or export or las files.
+    Write a ui.json file for either import or export or LAS Files.
 
-    :param basepath: Root directory for las data.
+    :param basepath: Root directory for LAS Data.
     :param mode: Switch for 'import' or 'export' behaviour.
 
     :return: Input file for the written data.
     """
 
     if mode not in ["import_files", "import_directories", "export_files"]:
         msg = "Mode argument must be 'import_files', 'import_directories', or 'export_files'."
```

### Comparing `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/export_las_files.ui.json` & `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/export_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_directories.ui.json` & `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_directories.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/las_geoh5-assets/uijson/import_las_files.ui.json` & `las_geoh5-0.2.0rc3/las_geoh5-assets/uijson/import_las_files.ui.json`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/LICENSE` & `las_geoh5-0.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `las_geoh5-0.2.0rc2/pyproject.toml` & `las_geoh5-0.2.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 [tool.poetry]
 name = "las-geoh5"
-version = "0.2.0-rc.2"
+version = "0.2.0-rc.3"
 description = "Las/Geoh5 conversion"
 license = "MIT"
 readme = "README.rst"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Benjamin Kary <benjamink@mirageoscience.com>"]
 keywords = ["geology", "geophysics", "earth sciences", "io", "data", "interoperability"]
 repository = "https://github.com/MiraGeoscience/las-geoh5"
 documentation  = "https://mirageoscience-las-geoh5.readthedocs-hosted.com/"
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 
-packages = [
-    { include = "las_geoh5" },
-    { include = "las_geoh5-assets" },
-]
-
-include = [
-    "COPYING",
-    "COPYING.LESSER",
-    "LICENSE",
-    "README.rst",
-    "THIRD_PARTY_SOFTWARE.rst",
-]
-
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Natural Language :: English",
 ]
 
+packages = [
+    { include = "las_geoh5" },
+    { include = "las_geoh5-assets" },
+]
+
+include = [
+    "COPYING",
+    "COPYING.LESSER",
+    "LICENSE",
+    "README.rst",
+    "THIRD_PARTY_SOFTWARE.rst",
+]
+
+[tool.poetry.scripts]
+geoh5_to_las = 'las_geoh5.scripts.geoh5_to_las:main'
+las_to_geoh5 = 'las_geoh5.scripts.las_to_geoh5:main'
+
 [tool.poetry.dependencies]
 python = "^3.10, <3.11"
 
 lasio = "~0.31"
 numpy = "~1.23.5"  # also in geoh5py
 pydantic = "~2.5.2"
 tqdm = "^4.66.1"
```

### Comparing `las_geoh5-0.2.0rc2/README.rst` & `las_geoh5-0.2.0rc3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -49,49 +49,64 @@
    :depth: 3
 
 Documentation
 -------------
 `Online documentation <https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/>`_
 
 
-Install with PyPI
------------------
+Installation
+------------
 
-Since las-geoh5 is a small package with only a few dependencies, we recommend installing
-with the Python package index (PyPI) using pip.
+Install **las-geoh5** with ``pip`` from PyPI::
 
-From PyPI
-~~~~~~~~~
+    $ pip install las-geoh5
 
-To install the **las-geoh5** package published on PyPI:
 
-.. code-block:: bash
+Or from a branch on `github <https://github.com/MiraGeoscience/las-geoh5>`_::
+
+    $ pip install --upgrade --force-reinstall https://github.com/MiraGeoscience/las-geoh5/archive/refs/heads/BRANCH_NAME.zip
+
+(to use a tag rather than a branch, replace ``heads\BRANCH_NAME.zip`` by ``tags\TAG_NAME.zip``)
+
+
+Or from a local sources, after you have cloned the repository::
+
+    $ git clone https://github.com/MiraGeoscience/las-geoh5 [-b BRANCH_NAME]
+    $ pip install -e las-geoh5
 
-    pip install las-geoh5 geoh5py lasio tqdm
 
 Basic Usage
 -----------
+
+From Geoscience Analyst
+~~~~~~~~~~~~~~~~~~~~~~~
 .. _Geoscience ANALYST Pro: https://mirageoscience.com/mining-industry-software/geoscience-analyst-pro/
 
 The most convenient way to use this package is through `Geoscience ANALYST Pro`_
 where the import files driver may be run from the **file -> import**
 menu.
 
 All drivers may also be run from a ui.json file in `Geoscience ANALYST Pro`_
 by either adding to the Python Scripts directory or drag and drop into
 the viewport. Defaulted ui.json files can be found in the uijson folder
 of the las-geoh5 project.
 
-Finally, the drivers can be run from CLI using the following
+From command line
+~~~~~~~~~~~~~~~~~
+To run from command line, prepare first a JSON file with the parameters required for conversion.
+
+Then execute with::
 
-.. code:: bash
+    $ las_to_geoh5 parameters.json [-o output_geoh5]
+    $ geoh5_to_las parameters.json [-o output_dir]
 
-   python -m las_geoh5.module.driver some_file.ui.json
+where ``parameters.json`` is the path on disk to a JSON file with required input parameters.
 
-Where module is one of ``import_files``, ``export_files``, or ``import_las``.
+If optional ``-o`` (or ``--out``) value is not provided, the program will write out to the location
+specified by the JSON file.
 
 License
 -------
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a
```

### Comparing `las_geoh5-0.2.0rc2/PKG-INFO` & `las_geoh5-0.2.0rc3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: las-geoh5
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Las/Geoh5 conversion
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Keywords: geology,geophysics,earth sciences,io,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
@@ -84,49 +84,64 @@
    :depth: 3
 
 Documentation
 -------------
 `Online documentation <https://mirageoscience-las-geoh5.readthedocs-hosted.com/en/latest/>`_
 
 
-Install with PyPI
------------------
+Installation
+------------
 
-Since las-geoh5 is a small package with only a few dependencies, we recommend installing
-with the Python package index (PyPI) using pip.
+Install **las-geoh5** with ``pip`` from PyPI::
 
-From PyPI
-~~~~~~~~~
+    $ pip install las-geoh5
 
-To install the **las-geoh5** package published on PyPI:
 
-.. code-block:: bash
+Or from a branch on `github <https://github.com/MiraGeoscience/las-geoh5>`_::
+
+    $ pip install --upgrade --force-reinstall https://github.com/MiraGeoscience/las-geoh5/archive/refs/heads/BRANCH_NAME.zip
+
+(to use a tag rather than a branch, replace ``heads\BRANCH_NAME.zip`` by ``tags\TAG_NAME.zip``)
+
+
+Or from a local sources, after you have cloned the repository::
+
+    $ git clone https://github.com/MiraGeoscience/las-geoh5 [-b BRANCH_NAME]
+    $ pip install -e las-geoh5
 
-    pip install las-geoh5 geoh5py lasio tqdm
 
 Basic Usage
 -----------
+
+From Geoscience Analyst
+~~~~~~~~~~~~~~~~~~~~~~~
 .. _Geoscience ANALYST Pro: https://mirageoscience.com/mining-industry-software/geoscience-analyst-pro/
 
 The most convenient way to use this package is through `Geoscience ANALYST Pro`_
 where the import files driver may be run from the **file -> import**
 menu.
 
 All drivers may also be run from a ui.json file in `Geoscience ANALYST Pro`_
 by either adding to the Python Scripts directory or drag and drop into
 the viewport. Defaulted ui.json files can be found in the uijson folder
 of the las-geoh5 project.
 
-Finally, the drivers can be run from CLI using the following
+From command line
+~~~~~~~~~~~~~~~~~
+To run from command line, prepare first a JSON file with the parameters required for conversion.
+
+Then execute with::
 
-.. code:: bash
+    $ las_to_geoh5 parameters.json [-o output_geoh5]
+    $ geoh5_to_las parameters.json [-o output_dir]
 
-   python -m las_geoh5.module.driver some_file.ui.json
+where ``parameters.json`` is the path on disk to a JSON file with required input parameters.
 
-Where module is one of ``import_files``, ``export_files``, or ``import_las``.
+If optional ``-o`` (or ``--out``) value is not provided, the program will write out to the location
+specified by the JSON file.
 
 License
 -------
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a
```

