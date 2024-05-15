# Comparing `tmp/faim_ipa-0.3.3.tar.gz` & `tmp/faim_ipa-0.3.4.tar.gz`

## Comparing `faim_ipa-0.3.3.tar` & `faim_ipa-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/MetaSeriesUtils_dask.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/UIntHistogram.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/Zarr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/dask_utils.py
--rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/mobie.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/alignment/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/alignment/alignment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/__init__.py
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/acquisition.py
--rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/converter.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/plate.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackedTile.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/__init__.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/ChannelMetadata.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/MetaSeriesTiff.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/io/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/BoundingBox5D.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/DaskTileStitcher.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/Tile.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/__init__.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/stitching/stitching_utils.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/RegionAcquisition.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/StackedTile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/src/faim_ipa/visiview/ome_companion_utils.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/LICENSE
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/README.md
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 faim_ipa-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/MetaSeriesUtils_dask.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/UIntHistogram.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/Zarr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/__init__.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/dask_utils.py
+-rw-r--r--   0        0        0    11203 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/mobie.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/alignment/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/alignment/alignment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/__init__.py
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/acquisition.py
+-rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/converter.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/plate.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/StackedTile.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/StackAcquisition.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/io/ChannelMetadata.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/io/MetaSeriesTiff.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/io/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/stitching/BoundingBox5D.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/stitching/DaskTileStitcher.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/stitching/Tile.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/stitching/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/stitching/stitching_utils.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/visiview/RegionAcquisition.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/visiview/StackedTile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/visiview/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/src/faim_ipa/visiview/ome_companion_utils.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/LICENSE
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/README.md
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 faim_ipa-0.3.4/PKG-INFO
```

### Comparing `faim_ipa-0.3.3/src/faim_ipa/MetaSeriesUtils_dask.py` & `faim_ipa-0.3.4/src/faim_ipa/MetaSeriesUtils_dask.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/UIntHistogram.py` & `faim_ipa-0.3.4/src/faim_ipa/UIntHistogram.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/Zarr.py` & `faim_ipa-0.3.4/src/faim_ipa/Zarr.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/dask_utils.py` & `faim_ipa-0.3.4/src/faim_ipa/dask_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/mobie.py` & `faim_ipa-0.3.4/src/faim_ipa/mobie.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/utils.py` & `faim_ipa-0.3.4/src/faim_ipa/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 from datetime import datetime
+import os.path
+from pathlib import Path
 
 
 def wavelength_to_rgb(wavelength, gamma=0.8):
     """This converts a given wavelength of light to an
     approximate RGB color value. The wavelength must be given
     in nanometers in the range from 380 nm through 750 nm
     (789 THz through 400 THz).
@@ -71,7 +73,64 @@
     handler.setLevel(logging.INFO)
     formatter = logging.Formatter(
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     return logger
+
+
+def get_git_root() -> Path:
+    """
+    Recursively search for the directory containing the .git folder.
+
+    Returns
+    -------
+    Path
+        Path to the root of the git repository.
+    """
+    parent_dir = Path(__file__).parent
+    while not (parent_dir / ".git").exists():
+        parent_dir = parent_dir.parent
+
+    return parent_dir
+
+
+def resolve_with_git_root(relative_path: Path) -> Path:
+    """
+    Takes a relative path and resolves it relative to the git_root directory.
+
+    Parameters
+    ----------
+    relative_path
+        Path relative to the git root.
+
+    Returns
+    -------
+    Path
+        Absolute path to the file.
+    """
+    git_root = get_git_root()
+    return (git_root / relative_path).resolve()
+
+
+def make_relative_to_git_root(path: Path) -> Path:
+    """
+    Convert an absolute path to a path relative to the git_root directory.
+
+    Parameters
+    ----------
+    path
+        Absolute path to a file.
+
+    Returns
+    -------
+    Path
+        Path relative to the git root.
+    """
+    git_root = get_git_root()
+    try:
+        # requires Python >= 3.12
+        return path.relative_to(git_root, walk_up=True)
+    except (ValueError, TypeError):
+        # fallback for Python < 3.12
+        return Path(os.path.relpath(path, git_root))
```

### Comparing `faim_ipa-0.3.3/src/faim_ipa/alignment/alignment.py` & `faim_ipa-0.3.4/src/faim_ipa/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/acquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/acquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/converter.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/converter.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/plate.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/plate.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/CellVoyagerWellAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/StackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/StackedTile.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/cellvoyager/ZAdjustedStackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/ImageXpressPlateAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/ImageXpressWellAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/MixedAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/SinglePlaneAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/hcs/imagexpress/StackAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/hcs/imagexpress/StackAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/io/MetaSeriesTiff.py` & `faim_ipa-0.3.4/src/faim_ipa/io/MetaSeriesTiff.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/stitching/BoundingBox5D.py` & `faim_ipa-0.3.4/src/faim_ipa/stitching/BoundingBox5D.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/stitching/DaskTileStitcher.py` & `faim_ipa-0.3.4/src/faim_ipa/stitching/DaskTileStitcher.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/stitching/Tile.py` & `faim_ipa-0.3.4/src/faim_ipa/stitching/Tile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/stitching/stitching_utils.py` & `faim_ipa-0.3.4/src/faim_ipa/stitching/stitching_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/visiview/RegionAcquisition.py` & `faim_ipa-0.3.4/src/faim_ipa/visiview/RegionAcquisition.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/visiview/StackedTile.py` & `faim_ipa-0.3.4/src/faim_ipa/visiview/StackedTile.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/src/faim_ipa/visiview/ome_companion_utils.py` & `faim_ipa-0.3.4/src/faim_ipa/visiview/ome_companion_utils.py`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/.gitignore` & `faim_ipa-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/LICENSE` & `faim_ipa-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/pyproject.toml` & `faim_ipa-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faim_ipa-0.3.3/PKG-INFO` & `faim_ipa-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faim-ipa
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools used at FMI-FAIM for Image Processing and Analysis.
 Project-URL: Bug Tracker, https://github.com/fmi-faim/faim-ipa/issues
 Project-URL: Documentation, https://github.com/fmi-faim/faim-ipa#README.md
 Project-URL: Homepage, https://github.com/fmi-faim/faim-ipa.git
 Project-URL: Source Code, https://github.com/fmi-faim/faim-ipa
 Project-URL: User Support, https://github.com/fmi-faim/faim-ipa/issues
 Author-email: Tim-Oliver Buchholz <tim-oliver.buchholz@fmi.ch>, Jan Eglinger <jan.eglinger@fmi.ch>
```

