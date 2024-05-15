# Comparing `tmp/mass_composition-0.4.9.tar.gz` & `tmp/mass_composition-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.4.9.tar", max compression
+gzip compressed data, was "mass_composition-0.5.0.tar", max compression
```

## Comparing `mass_composition-0.4.9.tar` & `mass_composition-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1069 2024-05-12 12:05:07.614922 mass_composition-0.4.9/LICENSE
--rw-r--r--   0        0        0     3449 2024-05-12 12:05:07.614922 mass_composition-0.4.9/README.md
--rw-r--r--   0        0        0      300 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9833 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0     9284 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6569 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0     2080 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52590 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      638 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0    41220 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/network.py
--rw-r--r--   0        0        0     5752 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0       42 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     3556 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      730 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8510 2024-05-12 12:05:08.018925 mass_composition-0.4.9/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2014 2024-05-12 12:05:08.022925 mass_composition-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 mass_composition-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-15 01:02:16.309356 mass_composition-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3449 2024-05-15 01:02:16.309356 mass_composition-0.5.0/README.md
+-rw-r--r--   0        0        0      360 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0     9238 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6565 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41758 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    52834 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19410 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0      960 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2014 2024-05-15 01:02:16.717358 mass_composition-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 mass_composition-0.5.0/PKG-INFO
```

### Comparing `mass_composition-0.4.9/LICENSE` & `mass_composition-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/README.md` & `mass_composition-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/balance.py` & `mass_composition-0.5.0/elphick/mass_composition/balance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 For managing the mass balance across a mc-network.
 
 DESIGN NOTE: Use a balance config file for the standard deviation definition rather than
-appending more properties to the MCNetwork object (at least for now), since mass balancing
+appending more properties to the Flowsheet object (at least for now), since mass balancing
 may be more for advanced users - keeps those properties in the scope of this class.
 
 DESIGN NOTE: Early attempts to optimise error/cost in absolute space (mass/grade differences) while
 constraining the mass balance (in metal units failed), due to needing a matric of constraints in the same space
 as the input.  Instead, we'll apply a cost to the metal balance by each component.
 
 Initially we will develop for dry balancing only.
@@ -15,21 +15,21 @@
 from functools import partial
 from typing import Optional, List, Callable, Dict
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import minimize, LinearConstraint
 
-from elphick.mass_composition.network import MCNetwork
+from elphick.mass_composition.flowsheet import Flowsheet
 from elphick.mass_composition.mc_node import NodeType
 
 
 class MCBalance:
-    def __init__(self, mcn: MCNetwork):
-        self.mcn: MCNetwork = mcn
+    def __init__(self, fs: Flowsheet):
+        self.fs: Flowsheet = fs
         self.sd: pd.DataFrame = self.create_balance_config(best_measurements='input')
 
     def _create_cost_functions(self) -> Dict[str, Callable]:
         """Cost Functions to be minimised
 
         We penalise the following:
         1) differences between mass and absolute grades for each stream versus measured.
@@ -38,24 +38,24 @@
         If each record is minimised with the appropriate cost function individually we expect
         to balance each record as well as the aggregate.
 
         Returns:
             float which is the cost to be minimised
         """
 
-        xm: pd.DataFrame = self.mcn.to_dataframe().drop(columns=['mass_wet'])
+        xm: pd.DataFrame = self.fs.to_dataframe().drop(columns=['mass_wet'])
 
         # xi: pd.DataFrame = df_x[[col for col in df_x.columns if col != 'mass_wet']]
         # sd: pd.DataFrame = self.sd
 
-        stream_map: Dict = {n: i for i, n in enumerate(self.mcn.get_stream_names())}
-        nodes = [n for n in self.mcn.graph.nodes.data() if n[1]['mc'].node_type == NodeType.BALANCE]
+        stream_map: Dict = {n: i for i, n in enumerate(self.fs.get_stream_names())}
+        nodes = [n for n in self.fs.graph.nodes.data() if n[1]['mc'].node_type == NodeType.BALANCE]
         node_ins_outs: List = []
         for n in nodes:
-            inputs, outputs = self.mcn.get_node_input_outputs(n[0])
+            inputs, outputs = self.fs.get_node_input_outputs(n[0])
             node_ins_outs.append(([stream_map[i.name] for i in inputs], [stream_map[o.name] for o in outputs]))
 
         def cost_fn(x: np.ndarray, xm: np.ndarray, sd: np.ndarray, node_relationships: List) -> float:
             """The numpy compliant cost function
 
             The columns of xm and sd are mass_dry, h2o, followed by any chemical analytes
 
@@ -83,17 +83,17 @@
                 cost_component_balance.append(x_mass_node.sum())
 
             costs = cost_mass_grades.sum() + sum(cost_component_balance)
             return costs
 
         # create one cost function per record
         d_fns: Dict = {}
-        df_network: pd.DataFrame = self.mcn.to_dataframe()
+        df_network: pd.DataFrame = self.fs.to_dataframe()
         cols = [col for col in df_network.columns if col != 'mass_wet']
-        for i in self.mcn.get_input_streams()[0].data.to_dataframe().index:
+        for i in self.fs.get_input_streams()[0].data.to_dataframe().index:
             df_x: pd.DataFrame = df_network.loc[i, :][cols]
             d_fns[i] = partial(cost_fn, xm=df_x.values, sd=self.sd.values, node_relationships=node_ins_outs)
 
         return d_fns
 
     def _create_constraints(self) -> List[LinearConstraint]:
         """Prepare the optimisation constraints
@@ -101,17 +101,17 @@
         The constraints ensure that the optimised component values stay within range post optimisation.
 
         The values are extracted from the MassComposition objects on the network.
 
         Returns:
 
         """
-        xm: pd.DataFrame = self.mcn.to_dataframe().drop(columns=['mass_wet'])
+        xm: pd.DataFrame = self.fs.to_dataframe().drop(columns=['mass_wet'])
 
-        streams = self.mcn.streams_to_dict()
+        streams = self.fs.streams_to_dict()
         linear_constraints: List[LinearConstraint] = []
         for i, (s, mc) in enumerate(streams.items()):
             cons = mc.constraints
             for col in xm.columns:
                 cons_matrix = np.zeros([len(streams.keys()), xm.shape[1]])
                 cons_matrix[i, :] = (xm.columns == col) * 1
                 linear_constraints.append(LinearConstraint([cons_matrix.ravel()], [cons[col][0]], [cons[col][1]]))
@@ -129,21 +129,21 @@
         2) iterate the ins/outs tuples and store the names
         3) prepare the function from the reshaped x array (using num_components) and the stream index number.
 
         Returns:
 
         """
         pass
-        # stream_map: Dict = {n: i for i, n in enumerate(self.mcn.get_edge_names())}
-        # nodes = [n for n in self.mcn.graph.nodes.data() if n[1]['mc'].node_type == NodeType.BALANCE]
+        # stream_map: Dict = {n: i for i, n in enumerate(self.fs.get_edge_names())}
+        # nodes = [n for n in self.fs.graph.nodes.data() if n[1]['mc'].node_type == NodeType.BALANCE]
         # node_ins_outs: List = []
         # for n in nodes:
-        #     inputs, outputs = self.mcn.get_node_input_outputs(n[0])
+        #     inputs, outputs = self.fs.get_node_input_outputs(n[0])
         #     node_ins_outs.append(([stream_map[i.name] for i in inputs], [stream_map[o.name] for o in outputs]))
-        # num_components: int = len(self.mcn.get_input_edges()[0].variables.chemistry.get_var_names()) + 2
+        # num_components: int = len(self.fs.get_input_edges()[0].variables.chemistry.get_var_names()) + 2
         #
         # def constraint_fn(x: np.ndarray, node_relationships: List, num_comp: int) -> Callable:
         #     x_2d = x.reshape(len(x) // num_comp, num_comp)
         #     # convert to mass units - first column is dry mass
         #     # ignore moisture (wet basis) for now...
         #     x_mass = np.hstack([x_2d[:, 0].reshape(-1, 1), x_2d[:, 1:] * x_2d[:, 0].reshape(-1, 1) / 100.0])
         #     pass
@@ -163,23 +163,23 @@
             tighter than the nominal, but still able to flex when balanced (though less than other streams).
 
         Returns:
             A DataFrame containing one row per stream, and one column per component.  The values will be
             the SDs used to normalise the residuals in the cost function that is minimised during balancing.
         """
 
-        df_sd: pd.DataFrame = self.mcn.report().drop(columns=['mass_wet'])
+        df_sd: pd.DataFrame = self.fs.report().drop(columns=['mass_wet'])
         df_sd.loc[:, :] = 1.0
         if best_measurements:
             tight_sd: float = 0.001 if best_locked else 0.1
             if best_measurements == 'input':
-                for strm in [e.name for e in self.mcn.get_input_streams()]:
+                for strm in [e.name for e in self.fs.get_input_streams()]:
                     df_sd.loc[strm, :] = tight_sd
             elif best_measurements == 'output':
-                for strm in [e.name for e in self.mcn.get_output_streams()]:
+                for strm in [e.name for e in self.fs.get_output_streams()]:
                     df_sd.loc[strm, :] = tight_sd
             else:
                 raise KeyError("best_measurements argument must be 'input'|'output'")
         return df_sd
 
     def optimise(self) -> pd.DataFrame:
         """Optimise to deliver balanced mass and component masses
@@ -189,15 +189,15 @@
 
         Returns:
 
         """
 
         d_cost_fns: Dict[str, Callable] = self._create_cost_functions()
         constraints: List[LinearConstraint] = self._create_constraints()
-        df_measured: pd.DataFrame = self.mcn.to_dataframe().fillna(0)
+        df_measured: pd.DataFrame = self.fs.to_dataframe().fillna(0)
         cols: List[str] = [col for col in df_measured.columns if col != 'mass_wet']
 
         chunks: List = []
         for k, fn in d_cost_fns.items():
             df_x0: pd.DataFrame = df_measured.loc[k, cols]
             res = minimize(fn, df_x0.values.ravel(), method='powell',  #method='nelder-mead',
                            options={'xatol': 1e-5, 'disp': True, 'maxfev': 100000},
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/config/config_read.py` & `mass_composition-0.5.0/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.5.0/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/dag.py` & `mass_composition-0.5.0/elphick/mass_composition/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
-from copy import deepcopy
 from typing import List, Callable, Union, Optional, Tuple
 
 import matplotlib.pyplot as plt
 import networkx as nx
-import pandas as pd
 from joblib import Parallel, delayed
 
 from elphick.mass_composition import MassComposition
 
 
 class Node:
     def __init__(self, operation: Callable[..., Union[MassComposition, Tuple[MassComposition, MassComposition]]],
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.5.0/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.5.0/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.5.0/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.5.0/elphick/mass_composition/datasets/sample_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Optional, Iterable, List
 
 import numpy as np
 import pandas as pd
 
 from elphick.mass_composition import MassComposition
-from elphick.mass_composition.network import MCNetwork
+from elphick.mass_composition.flowsheet import Flowsheet
 from elphick.mass_composition.utils.components import is_compositional
 from elphick.mass_composition.datasets import load_size_by_assay, load_iron_ore_sample_a072391, load_size_distribution, \
     load_a072391_met
 from elphick.mass_composition.utils.partition import napier_munn, perfect
 
 
 def sample_data(include_wet_mass: bool = True, include_dry_mass: bool = True,
@@ -112,30 +112,30 @@
 
 def size_by_assay_2() -> pd.DataFrame:
     """ 3 x Sample Size x Assay dataset (balanced)
     """
     mc_size: MassComposition = MassComposition(size_by_assay(), name='feed')
     partition = partial(napier_munn, d50=0.150, ep=0.1, dim='size')
     mc_coarse, mc_fine = mc_size.apply_partition(definition=partition, name_1='coarse', name_2='fine')
-    mcn: MCNetwork = MCNetwork().from_streams([mc_size, mc_coarse, mc_fine])
-    return mcn.to_dataframe()
+    fs: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse, mc_fine])
+    return fs.to_dataframe()
 
 
 def size_by_assay_3() -> pd.DataFrame:
     """ 3 x Sample Size x Assay dataset (unbalanced)
     """
     mc_size: MassComposition = MassComposition(size_by_assay(), name='feed')
     partition = partial(napier_munn, d50=0.150, ep=0.1, dim='size')
     mc_coarse, mc_fine = mc_size.apply_partition(definition=partition, name_1='coarse', name_2='fine')
     # add error to the coarse stream to create an imbalance
     df_coarse_2 = mc_coarse.data.to_dataframe().apply(lambda x: np.random.normal(loc=x, scale=np.std(x)))
     mc_coarse_2: MassComposition = MassComposition(data=df_coarse_2, name='coarse')
     mc_coarse_2 = mc_coarse_2.set_parent_node(mc_size)
-    mcn_ub: MCNetwork = MCNetwork().from_streams([mc_size, mc_coarse_2, mc_fine])
-    return mcn_ub.to_dataframe()
+    fs_ub: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse_2, mc_fine])
+    return fs_ub.to_dataframe()
 
 
 def size_distribution() -> pd.DataFrame:
     return load_size_distribution()
 
 
 def iron_ore_sample_data() -> pd.DataFrame:
@@ -149,22 +149,22 @@
         'float64')
     df_met['Fe'] = df_met['Fe'].replace('MISSING', np.nan).astype('float64')
     df_met.dropna(subset=['Fe', 'Bulk_Hole_No', 'Dry Weight Fines (kg)'], inplace=True)
     df_met.columns = [col.replace('LOITotal', 'LOI') for col in df_met.columns]
     return df_met
 
 
-def demo_size_network() -> MCNetwork:
+def demo_size_network() -> Flowsheet:
     mc_size: MassComposition = MassComposition(size_by_assay(), name='size sample')
     partition = partial(perfect, d50=0.150, dim='size')
     mc_coarse, mc_fine = mc_size.apply_partition(definition=partition)
     mc_coarse.name = 'coarse'
     mc_fine.name = 'fine'
-    mcn: MCNetwork = MCNetwork().from_streams([mc_size, mc_coarse, mc_fine])
-    return mcn
+    fs: Flowsheet = Flowsheet().from_streams([mc_size, mc_coarse, mc_fine])
+    return fs
 
 
 if __name__ == '__main__':
     df1: pd.DataFrame = size_by_assay()
     df2: pd.DataFrame = size_by_assay_2()
     df3: pd.DataFrame = size_by_assay_3()
     print('done')
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/layout.py` & `mass_composition-0.5.0/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/mass_composition.py` & `mass_composition-0.5.0/elphick/mass_composition/mass_composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 
         self._logger = logging.getLogger(name=self.__class__.__name__)
 
         if config_file is None:
             config_file = Path(__file__).parent / './config/mc_config.yml'
         self.config = read_yaml(config_file)
 
-        # nodes become useful when multiple objects exist
-        self.nodes: List[int] = [random_int(), random_int()]
+        # _nodes can preserve relationships from math operations, and can be used to build a network.
+        self._nodes: List[Union[str, int]] = [random_int(), random_int()]
 
         self._name: str = name
         self._mass_units = self.config['units']['mass'] if not mass_units else None
         self._composition_units = self.config['units']['composition_rel'] if not composition_units else None
 
         self._specified_columns: Dict = {'mass_wet_var': mass_wet_var,
                                          'mass_dry_var': mass_dry_var,
@@ -173,23 +173,23 @@
         if isinstance(values, xr.Dataset) or isinstance(values, xr.DataArray):
             values = values.to_dataframe()
         for v in values.columns:
             self._data[v].values = values[v].values
         self.status = Status(self._check_constraints())
 
     def set_parent_node(self, parent: 'MassComposition') -> 'MassComposition':
-        self.nodes = [parent.nodes[1], self.nodes[1]]
+        self._nodes = [parent._nodes[1], self._nodes[1]]
         return self
 
     def set_child_node(self, child: 'MassComposition') -> 'MassComposition':
-        self.nodes = [self.nodes[0], child.nodes[0]]
+        self._nodes = [self._nodes[0], child._nodes[0]]
         return self
 
     def set_stream_nodes(self, nodes: Tuple[int, int]) -> 'MassComposition':
-        self.nodes = nodes
+        self._nodes = nodes
         return self
 
     def to_xarray(self) -> xr.Dataset:
         """Returns the mc compliant xr.Dataset
 
         Returns:
 
@@ -574,15 +574,15 @@
         # TODO: add support for supplementary variables
 
         df_upsampled: pd.DataFrame = mass_preserving_interp(self.data.to_dataframe(),
                                                             interval_edges=interval_edges, precision=precision,
                                                             include_original_edges=include_original_edges)
 
         obj: MassComposition = MassComposition(df_upsampled, name=self.name)
-        obj.nodes = self.nodes
+        obj.nodes = self._nodes
         obj.constraints = self.constraints
         return obj
 
     def add(self, other: 'MassComposition', name: Optional[str] = None) -> 'MassComposition':
         """Add two objects
 
         Adds other to self, with optional name of the returned object
@@ -966,16 +966,16 @@
 
         """
         xr_sum: xr.Dataset = self._data.mc.add(other._data)
 
         res: MassComposition = MassComposition(name=xr_sum.mc.name, constraints=self.constraints)
         res.set_data(data=xr_sum, constraints=self.constraints)
 
-        other.nodes = [other.nodes[0], self.nodes[1]]
-        res.nodes = [self.nodes[1], random_int()]
+        other._nodes = [other._nodes[0], self._nodes[1]]
+        res._nodes = [self._nodes[1], random_int()]
 
         return res
 
     def __sub__(self, other: 'MassComposition') -> 'MassComposition':
         """Subtract the supplied object from self
 
         Perform the subtraction with the mass-composition variables only and then append any attribute variables.
@@ -987,15 +987,15 @@
         """
 
         xr_sub: xr.Dataset = self._data.mc.sub(other._data)
 
         res: MassComposition = MassComposition(name=xr_sub.mc.name, constraints=self.constraints)
         res.set_data(data=xr_sub, constraints=self.constraints)
 
-        res.nodes = [self.nodes[1], random_int()]
+        res.nodes = [self._nodes[1], random_int()]
         return res
 
     def __truediv__(self, other: 'MassComposition') -> 'MassComposition':
         """Divide self by the supplied object
 
         Perform the division with the mass-composition variables only and then append any attribute variables.
         Args:
@@ -1008,20 +1008,25 @@
         xr_div: xr.Dataset = self._data.mc.div(other._data)
 
         res: MassComposition = MassComposition(name=xr_div.mc.name, constraints=self.constraints)
         res.set_data(data=xr_div, constraints=self.constraints)
 
         return res
 
+    def __eq__(self, other):
+        if isinstance(other, MassComposition):
+            return self.__dict__ == other.__dict__
+        return False
+
     @staticmethod
     def _check_cols_in_data_cols(cols: List[str], cols_data: List[str]):
         for col in cols:
             if (col is not None) and (col not in cols_data):
                 msg: str = f"{col} not in the data columns: {cols_data}"
-                logging.error(msg)
+                logging.getLogger(__name__).error(msg)
                 raise IndexError(msg)
 
     @staticmethod
     def _copy_all_attrs(xr_to: xr.Dataset, xr_from: xr.Dataset) -> xr.Dataset:
         xr_to.attrs.update(xr_from.attrs)
         da: xr.DataArray
         for new_da, da in zip(xr_to.values(), xr_from.values()):
@@ -1037,16 +1042,16 @@
         return xr_ds
 
     def _post_process_split(self, obj_1, obj_2, name_1, name_2):
         if name_1:
             obj_1._data.mc.rename(name_1)
         if name_2:
             obj_2._data.mc.rename(name_2)
-        obj_1.nodes = [self.nodes[1], random_int()]
-        obj_2.nodes = [self.nodes[1], random_int()]
+        obj_1._nodes = [self._nodes[1], random_int()]
+        obj_2._nodes = [self._nodes[1], random_int()]
         obj_1._name = name_1
         obj_2._name = name_2
         return obj_1, obj_2
 
     def _intervals_to_columns(self, interval_index: pd.IntervalIndex) -> pd.DataFrame:
         """Reconstruct columns from an interval index
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/mc_node.py` & `mass_composition-0.5.0/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/mc_status.py` & `mass_composition-0.5.0/elphick/mass_composition/mc_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 from typing import List
 
 import pandas as pd
 
 
 class Status:
     def __init__(self, df_oor: pd.DataFrame):
+        self._logger = logging.getLogger(__name__)
         self.oor: pd.DataFrame = df_oor
         self.num_oor: int = len(df_oor)
         self.failing_components: List[str] = list(df_oor.dropna(axis=1).columns) if self.num_oor > 0 else None
 
     @property
     def ok(self) -> bool:
         if self.num_oor > 0:
-            logging.warning(f'{self.num_oor} OOR records exist.')
+            self._logger.warning(f'{self.num_oor} out of range records exist.')
         return True if self.num_oor == 0 else False
 
     def __str__(self) -> str:
         res: str = f'status.ok: {self.ok}\n'
         res += f'num_oor: {self.num_oor}'
         return res
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, Status):
+            # Compare the instances based on their attributes
+            return self.oor.equals(other.oor)
+        return False
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.5.0/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/network.py` & `mass_composition-0.5.0/elphick/mass_composition/flowsheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,43 +19,44 @@
 
 from elphick.mass_composition import MassComposition
 from elphick.mass_composition.config.config_read import read_flowsheet_yaml
 from elphick.mass_composition.dag import DAG
 from elphick.mass_composition.layout import digraph_linear_layout
 from elphick.mass_composition.mc_node import MCNode, NodeType
 from elphick.mass_composition.plot import parallel_plot, comparison_plot
+from elphick.mass_composition.stream import Stream
 from elphick.mass_composition.utils.geometry import midpoint
 from elphick.mass_composition.utils.loader import streams_from_dataframe
 from elphick.mass_composition.utils.sampling import random_int
 
 
-class MCNetwork:
+class Flowsheet:
     def __init__(self, name: str = 'Flowsheet'):
         self.name: str = name
         self.graph: nx.DiGraph = nx.DiGraph()
         self._logger: logging.Logger = logging.getLogger(__class__.__name__)
 
     @classmethod
-    def from_streams(cls, streams: List[MassComposition], name: Optional[str] = 'Flowsheet') -> 'MCNetwork':
+    def from_streams(cls, streams: List[Union[Stream, MassComposition]], name: Optional[str] = 'Flowsheet') -> 'Flowsheet':
         """Instantiate from a list of objects
 
         Args:
             streams: List of MassComposition objects
             name: name of the network
 
         Returns:
 
         """
 
-        streams: List[MassComposition] = cls._check_indexes(streams)
+        streams: List[Union[Stream, MassComposition]] = cls._check_indexes(streams)
         bunch_of_edges: List = []
         for stream in streams:
-            if stream.nodes is None:
+            if stream._nodes is None:
                 raise KeyError(f'Stream {stream.name} does not have the node property set')
-            nodes = stream.nodes
+            nodes = stream._nodes
 
             # add the objects to the edges
             bunch_of_edges.append((nodes[0], nodes[1], {'mc': stream}))
 
         graph = nx.DiGraph(name=name)
         graph.add_edges_from(bunch_of_edges)
         d_node_objects: Dict = {}
@@ -74,31 +75,35 @@
         obj = cls()
         obj.graph = graph
         return obj
 
     @classmethod
     def from_dataframe(cls, df: pd.DataFrame,
                        name: Optional[str] = 'Flowsheet',
-                       mc_name_col: Optional[str] = None) -> 'MCNetwork':
+                       mc_name_col: Optional[str] = None,
+                       n_jobs: int = 1) -> 'Flowsheet':
         """Instantiate from a DataFrame
 
         Args:
             df: The DataFrame
             name: name of the network
             mc_name_col: The column specified contains the names of objects to create.
               If None the DataFrame is assumed to be wide and the mc objects will be extracted from column prefixes.
+            n_jobs: The number of parallel jobs to run.  If -1, will use all available cores.
 
         Returns:
+            Flowsheet: An instance of the Flowsheet class initialized from the provided DataFrame.
 
         """
-        streams: Dict = streams_from_dataframe(df=df, mc_name_col=mc_name_col)
+        streams: Dict[Union[int, str], MassComposition] = streams_from_dataframe(df=df, mc_name_col=mc_name_col,
+                                                                                 n_jobs=n_jobs)
         return cls().from_streams(streams=list(streams.values()), name=name)
 
     @classmethod
-    def from_yaml(cls, flowsheet_file: Path) -> 'MCNetwork':
+    def from_yaml(cls, flowsheet_file: Path) -> 'Flowsheet':
         """Construct a flowsheet defined in a yaml file
 
         Args:
             flowsheet_file: The yaml file following the prescribed format
 
         Returns:
 
@@ -122,45 +127,45 @@
                                           node_subset=config['nodes'][node]['subset'])
         nx.set_node_attributes(graph, d_node_objects, 'mc')
 
         obj.graph = graph
         return obj
 
     @classmethod
-    def from_dag(cls, dag: DAG) -> 'MCNetwork':
+    def from_dag(cls, dag: DAG) -> 'Flowsheet':
         """Construct a flowsheet from a dag object
 
         Args:
             dag: The dag object that has been run previously.
 
         Returns:
 
         """
 
-        # Create a new instance of MCNetwork
-        mcn = cls(name=dag.name)
+        # Create a new instance of Flowsheet
+        fs = cls(name=dag.name)
 
-        # Copy the nodes from the dag to the MCNetwork
+        # Copy the nodes from the dag to the Flowsheet
         for nid, (node, data) in enumerate(dag.graph.nodes(data=True)):
-            mcn.graph.add_node(data['name'], mc=MCNode(node_id=nid, node_name=data['name']))
+            fs.graph.add_node(data['name'], mc=MCNode(node_id=nid, node_name=data['name']))
 
-        # Copy the edges from the dag to the MCNetwork
+        # Copy the edges from the dag to the Flowsheet
         for edge in dag.graph.edges:
             # Retrieve the MassComposition object from the edge
             mc = dag.graph.edges[edge]['mc']
             # Use the name of the MassComposition object as the name of the edge
-            mcn.graph.add_edge(*edge, name=mc.name, **dag.graph.edges[edge])
+            fs.graph.add_edge(*edge, name=mc.name, **dag.graph.edges[edge])
 
         # Populate the inputs and outputs properties of the MCNode objects
-        for node in mcn.graph.nodes:
-            mc_node = mcn.graph.nodes[node]['mc']
-            mc_node.inputs = [mcn.graph.edges[edge]['mc'] for edge in mcn.graph.in_edges(node)]
-            mc_node.outputs = [mcn.graph.edges[edge]['mc'] for edge in mcn.graph.out_edges(node)]
+        for node in fs.graph.nodes:
+            mc_node = fs.graph.nodes[node]['mc']
+            mc_node.inputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.in_edges(node)]
+            mc_node.outputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.out_edges(node)]
 
-        return mcn
+        return fs
 
     @property
     def balanced(self) -> bool:
         bal_vals: List = [self.graph.nodes[n]['mc'].balanced for n in self.graph.nodes]
         bal_vals = [bv for bv in bal_vals if bv is not None]
         return all(bal_vals)
 
@@ -184,15 +189,15 @@
         Args:
             name: The string name of the MassComposition object stored on an edge in the network.
 
         Returns:
 
         """
 
-        res: Optional[MassComposition] = None
+        res: Optional[Union[Stream, MassComposition]] = None
         for u, v, a in self.graph.edges(data=True):
             if a['mc'].name == name:
                 res = a['mc']
 
         if not res:
             raise ValueError(f"The specified name: {name} is not found on the network.")
 
@@ -206,38 +211,38 @@
         """
 
         res: List = []
         for u, v, a in self.graph.edges(data=True):
             res.append(a['mc'].name)
         return res
 
-    def get_input_streams(self) -> List[MassComposition]:
+    def get_input_streams(self) -> List[Union[Stream, MassComposition]]:
         """Get the input (feed) streams (edge objects)
 
         Returns:
             List of MassComposition objects
         """
 
         # Create a dictionary that maps node names to their degrees
         degrees = {n: d for n, d in self.graph.degree()}
 
-        res: List[MassComposition] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[u] == 1]
+        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[u] == 1]
         return res
 
-    def get_output_streams(self) -> List[MassComposition]:
+    def get_output_streams(self) -> List[Union[Stream, MassComposition]]:
         """Get the output (product) streams (edge objects)
 
         Returns:
             List of MassComposition objects
         """
 
         # Create a dictionary that maps node names to their degrees
         degrees = {n: d for n, d in self.graph.degree()}
 
-        res: List[MassComposition] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[v] == 1]
+        res: List[Union[Stream, MassComposition]] = [d['mc'] for u, v, d in self.graph.edges(data=True) if degrees[v] == 1]
         return res
 
     def get_column_formats(self, columns: List[str], strip_percent: bool = False) -> Dict[str, str]:
         """
 
         Args:
             columns: The columns to lookup format strings for
@@ -278,15 +283,15 @@
         return rpt
 
     def imbalance_report(self, node: int):
         mc_node: MCNode = self.graph.nodes[node]['mc']
         rpt: Path = mc_node.imbalance_report()
         webbrowser.open(str(rpt))
 
-    def query(self, mc_name: str, queries: Dict) -> 'MCNetwork':
+    def query(self, mc_name: str, queries: Dict) -> 'Flowsheet':
         """Query/filter across the network
 
         The queries provided will be applied to the MassComposition object in the network with the mc_name.
         The indexes for that result are then used to filter the other edges of the network.
 
         Args:
             mc_name: The name of the MassComposition object in the network to which the first filter to be applied.
@@ -298,24 +303,24 @@
 
         mc_obj_ref: MassComposition = self.get_edge_by_name(mc_name).query(queries=queries)
         # TODO: This construct limits us to filtering along a single dimension only
         coord: str = list(queries.keys())[0]
         index = mc_obj_ref.data[coord]
 
         # iterate through all other objects on the edges and filter them to the same indexes
-        mc_objects: List[MassComposition] = []
+        mc_objects: List[Union[Stream, MassComposition]] = []
         for u, v, a in self.graph.edges(data=True):
             if a['mc'].name == mc_name:
                 mc_objects.append(mc_obj_ref)
             else:
                 mc_obj: MassComposition = deepcopy(self.get_edge_by_name(a['mc'].name))
                 mc_obj._data = mc_obj._data.sel({coord: index.values})
                 mc_objects.append(mc_obj)
 
-        res: MCNetwork = MCNetwork.from_streams(mc_objects)
+        res: Flowsheet = Flowsheet.from_streams(mc_objects)
 
         return res
 
     def get_node_input_outputs(self, node) -> Tuple:
         in_edges = self.graph.in_edges(node)
         in_mc = [self.graph.get_edge_data(oe[0], oe[1])['mc'] for oe in in_edges]
         out_edges = self.graph.out_edges(node)
@@ -643,15 +648,15 @@
         Returns:
 
         """
         if stream is None:
             streams: Dict[str, MassComposition] = self.streams_to_dict()
             for k, v in streams.items():
                 streams[k] = v.set_stream_nodes((random_int(), random_int()))
-            self.graph = MCNetwork(name=self.name).from_streams(streams=list(streams.values())).graph
+            self.graph = Flowsheet(name=self.name).from_streams(streams=list(streams.values())).graph
         else:
             mc: MassComposition = self.get_edge_by_name(stream)
             mc.set_stream_nodes((random_int(), random_int()))
             self._update_graph(mc)
 
     def _update_graph(self, mc: MassComposition):
         """Update the graph with an existing stream object
@@ -659,21 +664,21 @@
         Args:
             mc: The stream object
 
         Returns:
 
         """
         # brutal approach - rebuild from streams
-        strms: List[MassComposition] = []
+        strms: List[Union[Stream, MassComposition]] = []
         for u, v, a in self.graph.edges(data=True):
             if a['mc'].name == mc.name:
                 strms.append(mc)
             else:
                 strms.append(a['mc'])
-        self.graph = MCNetwork(name=self.name).from_streams(streams=strms).graph
+        self.graph = Flowsheet(name=self.name).from_streams(streams=strms).graph
 
     def set_node_names(self, node_names: Dict[int, str]):
         """Set the names of network nodes with a Dict
         """
         for node in node_names.keys():
             if ('mc' in self.graph.nodes[node].keys()) and (node in node_names.keys()):
                 self.graph.nodes[node]['mc'].node_name = node_names[node]
@@ -970,20 +975,20 @@
                 df_streams_full.sort_index(ascending=False, inplace=True)
                 stream_nans: pd.DataFrame = df_streams_full.isna().stack(level=-1)
 
                 for stream in streams:
                     s: str = stream.name
                     tmp_nans: pd.Series = stream_nans.query('stream==@s').sum(axis=1)
                     if tmp_nans.iloc[0] > 0:
-                        logging.debug(f'The {s} stream has missing coarse sizes')
+                        logger.debug(f'The {s} stream has missing coarse sizes')
                         first_zero_index = tmp_nans.loc[tmp_nans == 0].index[0]
                         if tmp_nans[tmp_nans.index <= first_zero_index].sum() > 0:
-                            logging.debug(f'The {s} stream has missing sizes requiring interpolation')
+                            logger.debug(f'The {s} stream has missing sizes requiring interpolation')
                             raise NotImplementedError('Coming soon - we need interpolation!')
                         else:
-                            logging.debug(f'The {s} stream has missing coarse sizes only')
+                            logger.debug(f'The {s} stream has missing coarse sizes only')
                             stream_df = df_streams_full.loc[:, (slice(None), s)].droplevel(-1, axis=1).fillna(0)
                             # recreate the stream from the dataframe
                             stream.set_data(stream_df)
             else:
                 raise KeyError("stream index shapes are not consistent")
         return streams
```

### Comparing `mass_composition-0.4.9/elphick/mass_composition/plot.py` & `mass_composition-0.5.0/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/components.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/interp.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/partition.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/size.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/utils/viz.py` & `mass_composition-0.5.0/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.4.9/elphick/mass_composition/variables.py` & `mass_composition-0.5.0/elphick/mass_composition/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,21 @@
                                           name_match=str(match.group()) if match else None,
                                           name_force=self._specified_map[
                                               f"{v}_var"] if f"{v}_var" in self._specified_map.keys() else None,
                                           group=VariableGroups.MASS)
             res.append(variable)
         return res
 
+    def __eq__(self, other) -> bool:
+        if isinstance(other, Variables):
+            # Compare the instances based on their attributes
+            return (self._variables == other._variables and self._config == other._config and
+                    self._supplied == other._supplied and self._specified_map == other._specified_map)
+        return False
+
     def _detect_moisture_var(self) -> Variable:
         v = 'moisture'
         match = re.search(self._config[v]['search_regex'], '\n'.join(self._supplied),
                           flags=re.IGNORECASE | re.MULTILINE)
         variable: Variable = Variable(name=self._config[v]['standard_name'],
                                       name_property=v,
                                       format=self._config[v]['format'],
@@ -162,11 +169,7 @@
         for v in sup_vars:
             variable: Variable = Variable(name=v,
                                           name_property=v,
                                           name_match=v,
                                           group=VariableGroups.SUPPLEMENTARY)
             res.append(variable)
         return res
-
-
-
-
```

### Comparing `mass_composition-0.4.9/pyproject.toml` & `mass_composition-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.4.9"
+version = "0.5.0"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
```

### Comparing `mass_composition-0.4.9/PKG-INFO` & `mass_composition-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.4.9
+Version: 0.5.0
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

