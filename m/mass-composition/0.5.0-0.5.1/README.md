# Comparing `tmp/mass_composition-0.5.0.tar.gz` & `tmp/mass_composition-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.5.0.tar", max compression
+gzip compressed data, was "mass_composition-0.5.1.tar", max compression
```

## Comparing `mass_composition-0.5.0.tar` & `mass_composition-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1069 2024-05-15 01:02:16.309356 mass_composition-0.5.0/LICENSE
--rw-r--r--   0        0        0     3449 2024-05-15 01:02:16.309356 mass_composition-0.5.0/README.md
--rw-r--r--   0        0        0      360 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0     9238 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6565 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41758 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52834 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0      960 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-15 01:02:16.713358 mass_composition-0.5.0/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-15 01:02:16.717358 mass_composition-0.5.0/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2014 2024-05-15 01:02:16.717358 mass_composition-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 mass_composition-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-15 12:38:27.334730 mass_composition-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-15 12:38:27.334730 mass_composition-0.5.1/README.md
+-rw-r--r--   0        0        0      360 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    13598 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6565 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41619 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    52834 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19410 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     3357 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2014 2024-05-15 12:38:27.742732 mass_composition-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.5.1/PKG-INFO
```

### Comparing `mass_composition-0.5.0/LICENSE` & `mass_composition-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/README.md` & `mass_composition-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MassComposition
 
-[![Run Tests](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml)
-[![Publish Docs](https://github.com/Elphick/mass-composition/actions/workflows/docs_to_gh_pages.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/docs_to_gh_pages.yml)
+[![Run Tests](https://github.com/Elphick/mass-composition/actions/workflows/poetry_build_and_test.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/poetry_build_and_test.yml)
+[![Publish Docs](https://github.com/Elphick/mass-composition/actions/workflows/poetry_sphinx_docs_to_gh_pages.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/poetry_sphinx_docs_to_gh_pages.yml)
 
 MassComposition is a python package that allows Geoscientists and Metallurgists to easily work with, and visualise
 mass-compositional data.
 
 Mass Composition in this context is just that - Mass *and* Composition.  It is not Compositional Data Analysis (CoDA), 
 since here we care more about mathematical operations like weight averaging and technically correct mathematical 
 operations.  Of course, we also need to manage moisture correctly - chemical composition is reported on a dry basis
```

### Comparing `mass_composition-0.5.0/elphick/mass_composition/balance.py` & `mass_composition-0.5.1/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/config/config_read.py` & `mass_composition-0.5.1/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.5.1/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.5.1/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.5.1/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.5.1/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.5.1/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/flowsheet.py` & `mass_composition-0.5.1/elphick/mass_composition/flowsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,22 +142,20 @@
         """
 
         # Create a new instance of Flowsheet
         fs = cls(name=dag.name)
 
         # Copy the nodes from the dag to the Flowsheet
         for nid, (node, data) in enumerate(dag.graph.nodes(data=True)):
-            fs.graph.add_node(data['name'], mc=MCNode(node_id=nid, node_name=data['name']))
+            fs.graph.add_node(node, mc=MCNode(node_id=nid, node_name=node))
 
         # Copy the edges from the dag to the Flowsheet
         for edge in dag.graph.edges:
-            # Retrieve the MassComposition object from the edge
-            mc = dag.graph.edges[edge]['mc']
             # Use the name of the MassComposition object as the name of the edge
-            fs.graph.add_edge(*edge, name=mc.name, **dag.graph.edges[edge])
+            fs.graph.add_edge(*edge, **dag.graph.edges[edge])
 
         # Populate the inputs and outputs properties of the MCNode objects
         for node in fs.graph.nodes:
             mc_node = fs.graph.nodes[node]['mc']
             mc_node.inputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.in_edges(node)]
             mc_node.outputs = [fs.graph.edges[edge]['mc'] for edge in fs.graph.out_edges(node)]
```

### Comparing `mass_composition-0.5.0/elphick/mass_composition/layout.py` & `mass_composition-0.5.1/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/mass_composition.py` & `mass_composition-0.5.1/elphick/mass_composition/mass_composition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/mc_node.py` & `mass_composition-0.5.1/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/mc_status.py` & `mass_composition-0.5.1/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.5.1/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/plot.py` & `mass_composition-0.5.1/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/components.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/interp.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/loader.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/partition.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/size.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/utils/viz.py` & `mass_composition-0.5.1/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/elphick/mass_composition/variables.py` & `mass_composition-0.5.1/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.0/pyproject.toml` & `mass_composition-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.5.0"
+version = "0.5.1"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
```

### Comparing `mass_composition-0.5.0/PKG-INFO` & `mass_composition-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.5.0
+Version: 0.5.1
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -28,16 +28,16 @@
 Requires-Dist: xarray (>=2022.6.0)
 Project-URL: Documentation, https://elphick.github.io/mass-composition
 Project-URL: Repository, https://github.com/elphick/mass-composition
 Description-Content-Type: text/markdown
 
 # MassComposition
 
-[![Run Tests](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/build_and_test.yml)
-[![Publish Docs](https://github.com/Elphick/mass-composition/actions/workflows/docs_to_gh_pages.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/docs_to_gh_pages.yml)
+[![Run Tests](https://github.com/Elphick/mass-composition/actions/workflows/poetry_build_and_test.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/poetry_build_and_test.yml)
+[![Publish Docs](https://github.com/Elphick/mass-composition/actions/workflows/poetry_sphinx_docs_to_gh_pages.yml/badge.svg?branch=main)](https://github.com/Elphick/mass-composition/actions/workflows/poetry_sphinx_docs_to_gh_pages.yml)
 
 MassComposition is a python package that allows Geoscientists and Metallurgists to easily work with, and visualise
 mass-compositional data.
 
 Mass Composition in this context is just that - Mass *and* Composition.  It is not Compositional Data Analysis (CoDA), 
 since here we care more about mathematical operations like weight averaging and technically correct mathematical 
 operations.  Of course, we also need to manage moisture correctly - chemical composition is reported on a dry basis
```

