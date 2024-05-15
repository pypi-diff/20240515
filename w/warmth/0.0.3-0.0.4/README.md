# Comparing `tmp/warmth-0.0.3.tar.gz` & `tmp/warmth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warmth-0.0.3.tar", max compression
+gzip compressed data, was "warmth-0.0.4.tar", max compression
```

## Comparing `warmth-0.0.3.tar` & `warmth-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7652 2024-05-08 06:50:19.427116 warmth-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1286 2024-05-08 06:50:19.427116 warmth-0.0.3/README.md
--rw-r--r--   0        0        0      854 2024-05-08 06:50:47.571419 warmth-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       87 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/__init__.py
--rw-r--r--   0        0        0    33895 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/build.py
--rw-r--r--   0        0        0    44794 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/data/haq87.json
--rw-r--r--   0        0        0    39680 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/data.py
--rw-r--r--   0        0        0    78689 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/forward_modelling.py
--rw-r--r--   0        0        0      284 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/logging.py
--rw-r--r--   0        0        0    80196 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/mesh_model.py
--rw-r--r--   0        0        0     8296 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/mesh_utils.py
--rw-r--r--   0        0        0     1991 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/model.py
--rw-r--r--   0        0        0    10952 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/parameters.py
--rw-r--r--   0        0        0    19686 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/postprocessing.py
--rw-r--r--   0        0        0    30098 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/resqpy_helpers.py
--rw-r--r--   0        0        0    10027 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/simulator.py
--rw-r--r--   0        0        0     4255 2024-05-08 06:50:19.563118 warmth-0.0.3/warmth/utils.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 warmth-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-15 13:34:48.629138 warmth-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1409 2024-05-15 13:34:48.629138 warmth-0.0.4/README.md
+-rw-r--r--   0        0        0      854 2024-05-15 13:35:18.109297 warmth-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-15 13:34:48.785139 warmth-0.0.4/warmth/__init__.py
+-rw-r--r--   0        0        0    33895 2024-05-15 13:34:48.785139 warmth-0.0.4/warmth/build.py
+-rw-r--r--   0        0        0    44794 2024-05-15 13:34:48.785139 warmth-0.0.4/warmth/data/haq87.json
+-rw-r--r--   0        0        0    39680 2024-05-15 13:34:48.785139 warmth-0.0.4/warmth/data.py
+-rw-r--r--   0        0        0    78689 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/forward_modelling.py
+-rw-r--r--   0        0        0      284 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/logging.py
+-rw-r--r--   0        0        0    80278 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/mesh_model.py
+-rw-r--r--   0        0        0     8296 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/mesh_utils.py
+-rw-r--r--   0        0        0     1991 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/model.py
+-rw-r--r--   0        0        0    11012 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/parameters.py
+-rw-r--r--   0        0        0    19686 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/postprocessing.py
+-rw-r--r--   0        0        0    30098 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/resqpy_helpers.py
+-rw-r--r--   0        0        0    10265 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/simulator.py
+-rw-r--r--   0        0        0     4307 2024-05-15 13:34:48.789139 warmth-0.0.4/warmth/utils.py
+-rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 warmth-0.0.4/PKG-INFO
```

### Comparing `warmth-0.0.3/LICENSE.md` & `warmth-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/README.md` & `warmth-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Warmth
 ## Forward modeling of thermal evolution through geological time
 
 ![Build Status](https://github.com/equinor/warmth/actions/workflows/python-test.yml/badge.svg?branch=main)
 ![Build Status](https://github.com/equinor/warmth/actions/workflows/docs.yml/badge.svg?branch=main)
+[![codecov](https://codecov.io/gh/equinor/warmth/graph/badge.svg?token=A9LWISA7OI)](https://codecov.io/gh/equinor/warmth)
 
 [Documentation](https://equinor.github.io/warmth/)
 
 warmth is a python package used for modeling thermal evolution based on McKenzie's type basin extension. It can be use for:
 
 - Finding beta factor
 - Calculating subsidence and thermal history
```

### Comparing `warmth-0.0.3/pyproject.toml` & `warmth-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warmth"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 xtgeo = "^3.4.0"
```

### Comparing `warmth-0.0.3/warmth/build.py` & `warmth-0.0.4/warmth/build.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/data/haq87.json` & `warmth-0.0.4/warmth/data/haq87.json`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/data.py` & `warmth-0.0.4/warmth/data.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/forward_modelling.py` & `warmth-0.0.4/warmth/forward_modelling.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/mesh_model.py` & `warmth-0.0.4/warmth/mesh_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Tuple
+from pathlib import Path
 import numpy as np
 from mpi4py import MPI
 import meshio
 import dolfinx  
 from petsc4py import PETSc
 import ufl
 import sys
@@ -1587,15 +1588,15 @@
     nums = 4
     dt = parameters.myr2s / nums # time step is 1/4 of 1Ma
     mms2 = []
     mms_tti = []
     tti = 0
     # base_flux = 0.0033
     writeout_final = True
-    time_solve = 0.0    
+    time_solve = 0.0
     with Bar('Processing...',check_tty=False, max=(start_time-end_time)) as bar:
         for tti in range(start_time, end_time-1,-1): #start from oldest
             rebuild_mesh = (tti==start_time)
             if rebuild_mesh:
                 logger.info(f"Rebuild/reload mesh at {tti}")          
                 mm2 = UniformNodeGridFixedSizeMeshModel(builder, parameters,sedimentsOnly, padding_num_nodes=pad_num_nodes)
                 mm2.buildMesh(tti)
@@ -1638,13 +1639,14 @@
             comm.send(mm2.mesh.topology.index_map(0).local_to_global(list(range(mm2.mesh.geometry.x.shape[0]))) , dest=0, tag=((comm.rank-1)*10)+21)
             comm.send(mm2.mesh_reindex, dest=0, tag=((comm.rank-1)*10)+23)
             comm.send(mm2.mesh_vertices_age, dest=0, tag=((comm.rank-1)*10)+25)
             comm.send(mm2.posarr, dest=0, tag=((comm.rank-1)*10)+20)
             comm.send(mm2.Tarr, dest=0, tag=((comm.rank-1)*10)+24)
         if comm.rank==0:
             mm2.receive_mpi_messages()
+            Path(out_dir).mkdir(parents=True, exist_ok=True)
             # EPCfilename = mm2.write_hexa_mesh_resqml("temp/", end_time)
             # logger.info(f"RESQML model written to: {EPCfilename}")
-            EPCfilename_ts = mm2.write_hexa_mesh_timeseries("temp/")
+            EPCfilename_ts = mm2.write_hexa_mesh_timeseries(out_dir)
             logger.info(f"RESQML partial model with timeseries written to: {EPCfilename_ts}")
             read_mesh_resqml_hexa(EPCfilename_ts)  # test reading of the .epc file
     return mm2
```

### Comparing `warmth-0.0.3/warmth/mesh_utils.py` & `warmth-0.0.4/warmth/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/model.py` & `warmth-0.0.4/warmth/model.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/parameters.py` & `warmth-0.0.4/warmth/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,13 +377,14 @@
         if val == -1:
             self._time_step_Ma = val
         else:
             logger.warning("Accept -1 only")
         return
 
     def dump(self,filepath:Path):
+        filepath.parent.mkdir(exist_ok=True, parents=True)
         with open(filepath, "wb") as f:
             pickle.dump(self, f, protocol=pickle.HIGHEST_PROTOCOL)
         return
```

### Comparing `warmth-0.0.3/warmth/postprocessing.py` & `warmth-0.0.4/warmth/postprocessing.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/resqpy_helpers.py` & `warmth-0.0.4/warmth/resqpy_helpers.py`

 * *Files identical despite different names*

### Comparing `warmth-0.0.3/warmth/simulator.py` & `warmth-0.0.4/warmth/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,34 +110,36 @@
 
         node._dump(p)
         return p
 
     def dump_input_data(self, use_mpi=False):
         p = []
         parameter_data_path = self._parameters_path
-
-        from mpi4py import MPI
-        comm = MPI.COMM_WORLD        
-        if (comm.rank==0):
-            self._builder.parameters.dump(self._parameters_path)
-            if isinstance(self._builder.grid,type(None)) is False:
-                self._builder.grid.dump(self._grid_path)                
-            if use_mpi:
+        if use_mpi:
+            from mpi4py import MPI
+            comm = MPI.COMM_WORLD        
+            if (comm.rank==0):
+                self._builder.parameters.dump(self._parameters_path)
+                if isinstance(self._builder.grid,type(None)) is False:
+                    self._builder.grid.dump(self._grid_path)                
                 from mpi4py.futures import MPIPoolExecutor
                 with MPIPoolExecutor(max_workers=10) as th:
                     futures = [th.submit(self.dump_input_nodes,  i)
                             for i in self._builder.iter_node() if i is not False]
                     for future in concurrent.futures.as_completed(futures):
                         p.append([parameter_data_path, future.result()])
-            else:
-                with concurrent.futures.ThreadPoolExecutor(max_workers=10) as th:
-                    futures = [th.submit(self.dump_input_nodes,  i)
-                            for i in self._builder.iter_node() if i is not False]
-                    for future in concurrent.futures.as_completed(futures):
-                        p.append([parameter_data_path, future.result()])
+        else:
+            self._builder.parameters.dump(self._parameters_path)
+            if isinstance(self._builder.grid,type(None)) is False:
+                self._builder.grid.dump(self._grid_path)
+            with concurrent.futures.ThreadPoolExecutor(max_workers=10) as th:
+                futures = [th.submit(self.dump_input_nodes,  i)
+                        for i in self._builder.iter_node() if i is not False]
+                for future in concurrent.futures.as_completed(futures):
+                    p.append([parameter_data_path, future.result()])
         return p
 
     def setup_directory(self, purge=False):
         if self._builder.parameters.output_path.exists():
             if purge:
                 from shutil import rmtree
                 rmtree(self._builder.parameters.output_path)
@@ -189,65 +191,66 @@
         if count >0:
             logger.info(f"Setting {count} nodes to partial simulation")
         return count
 
 
     def _parellel_run(self, save, purge, use_mpi=False):
         filtered = self._filter_full_sim()
-        from mpi4py import MPI
-        comm = MPI.COMM_WORLD        
-        if (comm.rank==0):
-            self.setup_directory(purge)
-        p = self.dump_input_data(use_mpi=use_mpi)
-
         if use_mpi:
             from mpi4py.futures import MPIPoolExecutor
+            from mpi4py import MPI
+            comm = MPI.COMM_WORLD        
+            if (comm.rank==0):
+                self.setup_directory(purge)
+            p = self.dump_input_data(use_mpi=use_mpi)
             with MPIPoolExecutor(max_workers=20) as executor:
                 results = [executor.submit(runWorker, i) for i in p]
                 with Bar('Processing...',check_tty=False, max=len(p)) as bar:
                     for future in concurrent.futures.as_completed(results):
                         bar.next()
                         try:
                             path_result = future.result()
                             n= load_node(path_result) # numerical model error should still resovle
                             if save==False:
                                 path_result.unlink()
                             self.put_node_to_grid(n)
                         except Exception as e:
                             logger.error(e)
         else:
+            self.setup_directory(purge)
+            p = self.dump_input_data(use_mpi=use_mpi)
             with concurrent.futures.ProcessPoolExecutor(mp_context=get_context('spawn')) as executor:
                 results = [executor.submit(runWorker, i) for i in p]
                 with Bar('Processing...',check_tty=False, max=len(p)) as bar:
                     for future in concurrent.futures.as_completed(results):
                         bar.next()
                         try:
                             path_result = future.result()
                             n= load_node(path_result) # numerical model error should still resovle
                             if save==False:
                                 path_result.unlink()
                             self.put_node_to_grid(n)
                         except Exception as e:
                             logger.error(e)
         # pick up node with no results (failed)
-        if comm.rank==0:                            
-            for node_path in self._nodes_path.iterdir():
-                str_f = str(node_path)
-                if str_f.endswith(".pickle"):
-                    n=load_node(node_path)
-                    if save==False:
-                        node_path.unlink()
-                    self.put_node_to_grid(n)
-                    logger.warning(f"No result file for node X:{n.X}, Y:{n.Y}")
-            if save==False:
-                from shutil import rmtree
-                rmtree(self._builder.parameters.output_path)
-            if filtered >0:
-                logger.info(f"Interpolating results back to {filtered} partial simulated nodes")
-                interp_res= Results_interpolator(self._builder,len(p)-filtered)
-                interp_res.run()
+        #if comm.rank==0:                            
+        for node_path in self._nodes_path.iterdir():
+            str_f = str(node_path)
+            if str_f.endswith(".pickle"):
+                n=load_node(node_path)
+                if save==False:
+                    node_path.unlink()
+                self.put_node_to_grid(n)
+                logger.warning(f"No result file for node X:{n.X}, Y:{n.Y}")
+        if save==False:
+            from shutil import rmtree
+            rmtree(self._builder.parameters.output_path)
+        if filtered >0:
+            logger.info(f"Interpolating results back to {filtered} partial simulated nodes")
+            interp_res= Results_interpolator(self._builder,len(p)-filtered)
+            interp_res.run()
         return
     def put_node_to_grid(self,node:single_node):
         self._builder.nodes[node.indexer[0]][node.indexer[1]]=node
         return
```

### Comparing `warmth-0.0.3/warmth/utils.py` & `warmth-0.0.4/warmth/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 #             x0, x1 = x1, x0
 
 #         steps_taken += 1
 
 #     return x1, steps_taken
 
 def compressed_pickle_save(data, path: Path):
+    path.parent.mkdir(exist_ok=True, parents=True)
     with open(path, "wb") as f:
         pickle.dump(data, f, protocol=pickle.HIGHEST_PROTOCOL)
 
 
 def compressed_pickle_open(path: Path):
     with open(path, "rb") as f:
         data = pickle.load(f)
```

### Comparing `warmth-0.0.3/PKG-INFO` & `warmth-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warmth
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,14 +21,15 @@
 Description-Content-Type: text/markdown
 
 # Warmth
 ## Forward modeling of thermal evolution through geological time
 
 ![Build Status](https://github.com/equinor/warmth/actions/workflows/python-test.yml/badge.svg?branch=main)
 ![Build Status](https://github.com/equinor/warmth/actions/workflows/docs.yml/badge.svg?branch=main)
+[![codecov](https://codecov.io/gh/equinor/warmth/graph/badge.svg?token=A9LWISA7OI)](https://codecov.io/gh/equinor/warmth)
 
 [Documentation](https://equinor.github.io/warmth/)
 
 warmth is a python package used for modeling thermal evolution based on McKenzie's type basin extension. It can be use for:
 
 - Finding beta factor
 - Calculating subsidence and thermal history
```

