# Comparing `tmp/maze_dataset-0.5.2.tar.gz` & `tmp/maze_dataset-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maze_dataset-0.5.2.tar", max compression
+gzip compressed data, was "maze_dataset-0.5.3.tar", max compression
```

## Comparing `maze_dataset-0.5.2.tar` & `maze_dataset-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      807 2024-02-23 23:31:07.694247 maze_dataset-0.5.2/maze_dataset/__init__.py
--rw-r--r--   0        0        0     3184 2023-08-30 17:18:26.899296 maze_dataset-0.5.2/maze_dataset/constants.py
--rw-r--r--   0        0        0      315 2023-06-14 21:33:25.457634 maze_dataset-0.5.2/maze_dataset/dataset/__init__.py
--rw-r--r--   0        0        0     7125 2023-08-05 17:49:14.165405 maze_dataset-0.5.2/maze_dataset/dataset/collected_dataset.py
--rw-r--r--   0        0        0      733 2023-06-14 21:33:25.459637 maze_dataset-0.5.2/maze_dataset/dataset/configs.py
--rw-r--r--   0        0        0    17940 2024-02-23 23:31:07.694247 maze_dataset-0.5.2/maze_dataset/dataset/dataset.py
--rw-r--r--   0        0        0    28928 2024-02-23 23:31:07.694247 maze_dataset-0.5.2/maze_dataset/dataset/maze_dataset.py
--rw-r--r--   0        0        0     9330 2023-09-19 02:43:45.435702 maze_dataset-0.5.2/maze_dataset/dataset/rasterized.py
--rw-r--r--   0        0        0      222 2023-06-14 21:33:25.462641 maze_dataset-0.5.2/maze_dataset/generation/__init__.py
--rw-r--r--   0        0        0      785 2023-09-04 07:04:48.392819 maze_dataset-0.5.2/maze_dataset/generation/default_generators.py
--rw-r--r--   0        0        0    16135 2023-09-22 00:15:11.541314 maze_dataset-0.5.2/maze_dataset/generation/generators.py
--rw-r--r--   0        0        0      354 2023-08-05 17:49:14.169411 maze_dataset-0.5.2/maze_dataset/maze/__init__.py
--rw-r--r--   0        0        0    40417 2024-03-19 21:12:46.325821 maze_dataset-0.5.2/maze_dataset/maze/lattice_maze.py
--rw-r--r--   0        0        0      294 2023-06-14 21:33:25.466639 maze_dataset-0.5.2/maze_dataset/plotting/__init__.py
--rw-r--r--   0        0        0     1425 2023-09-02 08:46:57.984811 maze_dataset-0.5.2/maze_dataset/plotting/plot_dataset.py
--rw-r--r--   0        0        0    18639 2024-02-23 23:21:43.983510 maze_dataset-0.5.2/maze_dataset/plotting/plot_maze.py
--rw-r--r--   0        0        0     2359 2023-09-06 08:38:01.808112 maze_dataset-0.5.2/maze_dataset/plotting/plot_tokens.py
--rw-r--r--   0        0        0     4820 2023-09-19 06:42:47.505724 maze_dataset-0.5.2/maze_dataset/plotting/print_tokens.py
--rw-r--r--   0        0        0        0 2023-02-27 15:19:24.914942 maze_dataset-0.5.2/maze_dataset/py.typed
--rw-r--r--   0        0        0      639 2024-03-19 22:11:10.517178 maze_dataset-0.5.2/maze_dataset/tokenization/__init__.py
--rw-r--r--   0        0        0    13101 2024-03-19 22:11:10.518179 maze_dataset-0.5.2/maze_dataset/tokenization/maze_tokenizer.py
--rw-r--r--   0        0        0     4293 2024-03-19 22:11:10.519189 maze_dataset-0.5.2/maze_dataset/tokenization/token_utils.py
--rw-r--r--   0        0        0     5107 2024-03-19 22:11:10.520183 maze_dataset-0.5.2/maze_dataset/tokenization/util.py
--rw-r--r--   0        0        0     7784 2024-02-23 23:31:07.694247 maze_dataset-0.5.2/maze_dataset/utils.py
--rw-r--r--   0        0        0     1972 2024-03-19 22:11:34.920286 maze_dataset-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     5691 2023-09-20 22:27:14.177464 maze_dataset-0.5.2/README.md
--rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 maze_dataset-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      807 2024-05-14 01:33:10.842133 maze_dataset-0.5.3/maze_dataset/__init__.py
+-rw-r--r--   0        0        0     3184 2024-05-14 01:33:10.843133 maze_dataset-0.5.3/maze_dataset/constants.py
+-rw-r--r--   0        0        0      315 2023-06-14 21:33:25.457634 maze_dataset-0.5.3/maze_dataset/dataset/__init__.py
+-rw-r--r--   0        0        0     7125 2023-08-05 17:49:14.165405 maze_dataset-0.5.3/maze_dataset/dataset/collected_dataset.py
+-rw-r--r--   0        0        0      733 2023-06-14 21:33:25.459637 maze_dataset-0.5.3/maze_dataset/dataset/configs.py
+-rw-r--r--   0        0        0    17940 2024-02-23 23:31:07.694247 maze_dataset-0.5.3/maze_dataset/dataset/dataset.py
+-rw-r--r--   0        0        0    29245 2024-05-14 23:02:49.631765 maze_dataset-0.5.3/maze_dataset/dataset/maze_dataset.py
+-rw-r--r--   0        0        0     9330 2023-09-19 02:43:45.435702 maze_dataset-0.5.3/maze_dataset/dataset/rasterized.py
+-rw-r--r--   0        0        0      222 2023-06-14 21:33:25.462641 maze_dataset-0.5.3/maze_dataset/generation/__init__.py
+-rw-r--r--   0        0        0      785 2023-09-04 07:04:48.392819 maze_dataset-0.5.3/maze_dataset/generation/default_generators.py
+-rw-r--r--   0        0        0    16135 2023-09-22 00:15:11.541314 maze_dataset-0.5.3/maze_dataset/generation/generators.py
+-rw-r--r--   0        0        0      354 2023-08-05 17:49:14.169411 maze_dataset-0.5.3/maze_dataset/maze/__init__.py
+-rw-r--r--   0        0        0    40417 2024-05-14 21:21:20.934839 maze_dataset-0.5.3/maze_dataset/maze/lattice_maze.py
+-rw-r--r--   0        0        0      294 2023-06-14 21:33:25.466639 maze_dataset-0.5.3/maze_dataset/plotting/__init__.py
+-rw-r--r--   0        0        0     1425 2023-09-02 08:46:57.984811 maze_dataset-0.5.3/maze_dataset/plotting/plot_dataset.py
+-rw-r--r--   0        0        0    19007 2024-05-14 23:03:04.312655 maze_dataset-0.5.3/maze_dataset/plotting/plot_maze.py
+-rw-r--r--   0        0        0     2359 2023-09-06 08:38:01.808112 maze_dataset-0.5.3/maze_dataset/plotting/plot_tokens.py
+-rw-r--r--   0        0        0     4820 2023-09-19 06:42:47.505724 maze_dataset-0.5.3/maze_dataset/plotting/print_tokens.py
+-rw-r--r--   0        0        0        0 2023-02-27 15:19:24.914942 maze_dataset-0.5.3/maze_dataset/py.typed
+-rw-r--r--   0        0        0      639 2024-05-14 01:33:10.847135 maze_dataset-0.5.3/maze_dataset/tokenization/__init__.py
+-rw-r--r--   0        0        0    13101 2024-05-14 01:33:10.848133 maze_dataset-0.5.3/maze_dataset/tokenization/maze_tokenizer.py
+-rw-r--r--   0        0        0     4293 2024-05-14 01:33:10.849133 maze_dataset-0.5.3/maze_dataset/tokenization/token_utils.py
+-rw-r--r--   0        0        0     5107 2024-05-14 01:33:10.850134 maze_dataset-0.5.3/maze_dataset/tokenization/util.py
+-rw-r--r--   0        0        0     7784 2024-05-14 01:33:10.851135 maze_dataset-0.5.3/maze_dataset/utils.py
+-rw-r--r--   0        0        0     1972 2024-05-14 23:06:26.632810 maze_dataset-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5691 2023-09-20 22:27:14.177464 maze_dataset-0.5.3/README.md
+-rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 maze_dataset-0.5.3/PKG-INFO
```

### Comparing `maze_dataset-0.5.2/maze_dataset/__init__.py` & `maze_dataset-0.5.3/maze_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/constants.py` & `maze_dataset-0.5.3/maze_dataset/constants.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/dataset/collected_dataset.py` & `maze_dataset-0.5.3/maze_dataset/dataset/collected_dataset.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/dataset/configs.py` & `maze_dataset-0.5.3/maze_dataset/dataset/configs.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/dataset/dataset.py` & `maze_dataset-0.5.3/maze_dataset/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/dataset/maze_dataset.py` & `maze_dataset-0.5.3/maze_dataset/dataset/maze_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,14 +650,15 @@
 
     @register_dataset_filter
     @staticmethod
     def collect_generation_meta(
         dataset: MazeDataset,
         clear_in_mazes: bool = True,
         inplace: bool = True,
+        allow_fail: bool = False,
     ) -> MazeDataset:
         if dataset.generation_metadata_collected is not None:
             return dataset
         # if the generation meta is already collected, don't collect it again, do nothing
 
         new_dataset: MazeDataset
         if inplace:
@@ -665,14 +666,21 @@
         else:
             new_dataset = copy.deepcopy(dataset)
 
         gen_meta_lists: dict[bool | int | float | str | CoordTup, Counter] = (
             defaultdict(Counter)
         )
         for maze in new_dataset:
+            if maze.generation_meta is None:
+                if allow_fail:
+                    break
+                else:
+                    raise ValueError(
+                        "generation meta is not present in a maze, cannot collect generation meta"
+                    )
             for key, value in maze.generation_meta.items():
                 if isinstance(value, (bool, int, float, str)):
                     gen_meta_lists[key][value] += 1
 
                 elif isinstance(value, set):
                     # special case for visited_cells
                     gen_meta_lists[key].update(value)
```

### Comparing `maze_dataset-0.5.2/maze_dataset/dataset/rasterized.py` & `maze_dataset-0.5.3/maze_dataset/dataset/rasterized.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/generation/default_generators.py` & `maze_dataset-0.5.3/maze_dataset/generation/default_generators.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/generation/generators.py` & `maze_dataset-0.5.3/maze_dataset/generation/generators.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/maze/lattice_maze.py` & `maze_dataset-0.5.3/maze_dataset/maze/lattice_maze.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/plotting/plot_dataset.py` & `maze_dataset-0.5.3/maze_dataset/plotting/plot_dataset.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/plotting/plot_maze.py` & `maze_dataset-0.5.3/maze_dataset/plotting/plot_maze.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations  # for type hinting self as return value
 
+import warnings
 from copy import deepcopy
 from dataclasses import dataclass
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from jaxtyping import Bool, Float
@@ -469,20 +470,28 @@
                         row * self.unit_length + 1 : (row + 1) * self.unit_length,
                         (col + 1) * self.unit_length,
                     ] = connection_values[row, col]
 
         return img
 
     def _plot_path(self, path_format: PathFormat) -> None:
+        if len(path_format.path) == 0:
+            warnings.warn(f"Empty path, skipping plotting\n{path_format = }")
+            return
         p_transformed = np.array(
             [self._rowcol_to_coord(coord) for coord in path_format.path]
         )
         if path_format.quiver_kwargs is not None:
-            x: np.ndarray = p_transformed[:, 0]
-            y: np.ndarray = p_transformed[:, 1]
+            try:
+                x: np.ndarray = p_transformed[:, 0]
+                y: np.ndarray = p_transformed[:, 1]
+            except Exception as e:
+                raise ValueError(
+                    f"Error in plotting quiver path:\n{path_format = }\n{p_transformed = }\n{e}"
+                ) from e
 
             # Generate colors from the colormap
             if path_format.cmap is not None:
                 n = len(x) - 1  # Number of arrows
                 cmap = plt.get_cmap(path_format.cmap)
                 colors = [cmap(i / n) for i in range(n)]
             else:
```

### Comparing `maze_dataset-0.5.2/maze_dataset/plotting/plot_tokens.py` & `maze_dataset-0.5.3/maze_dataset/plotting/plot_tokens.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/plotting/print_tokens.py` & `maze_dataset-0.5.3/maze_dataset/plotting/print_tokens.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/tokenization/__init__.py` & `maze_dataset-0.5.3/maze_dataset/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/tokenization/maze_tokenizer.py` & `maze_dataset-0.5.3/maze_dataset/tokenization/maze_tokenizer.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/tokenization/token_utils.py` & `maze_dataset-0.5.3/maze_dataset/tokenization/token_utils.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/tokenization/util.py` & `maze_dataset-0.5.3/maze_dataset/tokenization/util.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/maze_dataset/utils.py` & `maze_dataset-0.5.3/maze_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/pyproject.toml` & `maze_dataset-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maze-dataset"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Michael Ivanitskiy <miv@knc.ai>", "Dan Valentine <danvalentine256@gmail.com>", "Rusheb Shah <rusheb.shah@gmail.com>", "Lucia Quirke <luciaq@canva.com>", "Can Rager <can.rager@posteo.de>", "Alex Spies <alexfspies@gmail.com>", "Chris Mathwin <cwmathwin@gmail.com>", "Tilman Rauker <traeuker@googlemail.com>", "Guillaume Corlouer <guillaume.corlouer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "maze_dataset"}]
 repository = "https://github.com/understanding-search/maze-dataset"
 
 [tool.poetry.dependencies]
```

### Comparing `maze_dataset-0.5.2/README.md` & `maze_dataset-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `maze_dataset-0.5.2/PKG-INFO` & `maze_dataset-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maze-dataset
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Home-page: https://github.com/understanding-search/maze-dataset
 Author: Michael Ivanitskiy
 Author-email: miv@knc.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

