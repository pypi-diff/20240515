# Comparing `tmp/tgqSim-0.1.8.tar.gz` & `tmp/tgqSim-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.8.tar", last modified: Tue May 14 05:41:47 2024, max compression
+gzip compressed data, was "tgqSim-0.1.9.tar", last modified: Wed May 15 00:53:48 2024, max compression
```

## Comparing `tgqSim-0.1.8.tar` & `tgqSim-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.874247 tgqSim-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-14 05:41:46.000000 tgqSim-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-14 05:41:46.000000 tgqSim-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 05:41:47.873247 tgqSim-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 05:41:46.000000 tgqSim-0.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 05:41:47.874247 tgqSim-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-14 05:41:46.000000 tgqSim-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.872247 tgqSim-0.1.8/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.873247 tgqSim-0.1.8/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.873247 tgqSim-0.1.8/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    61952 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-14 05:41:46.000000 tgqSim-0.1.8/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 05:41:47.872247 tgqSim-0.1.8/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 05:41:47.000000 tgqSim-0.1.8/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-15 00:53:46.000000 tgqSim-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-15 00:53:46.000000 tgqSim-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-15 00:53:48.654812 tgqSim-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-15 00:53:46.000000 tgqSim-0.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 00:53:48.654812 tgqSim-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-15 00:53:47.000000 tgqSim-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.653812 tgqSim-0.1.9/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-15 00:53:47.000000 tgqSim-0.1.9/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    61952 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.653812 tgqSim-0.1.9/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.8/LICENSE` & `tgqSim-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/PKG-INFO` & `tgqSim-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.8
+Version: 0.1.9
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.8/setup.py` & `tgqSim-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.8',
+    version='0.1.9',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
     packages=["tgqSim", "tgqSim.GateSimulation"],
     install_requires=[
-        'numpy>=1.21.3',
-        'numba>=0.56.4',
+        'numpy>=1.19.0',
+        'numba>=0.53.0',
         'matplotlib>=3.5.3',
         'GPUtil>=1.4.0'
     ],
     classifiers=[
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
```

### Comparing `tgqSim-0.1.8/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.9/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.9/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.9/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.9/tgqSim/QuantumCircuit.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.9/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.1.9/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.1.9/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.8/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.9/tgqSim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.8
+Version: 0.1.9
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

