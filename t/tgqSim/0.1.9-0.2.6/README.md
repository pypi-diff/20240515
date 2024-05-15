# Comparing `tmp/tgqSim-0.1.9.tar.gz` & `tmp/tgqSim-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.9.tar", last modified: Wed May 15 00:53:48 2024, max compression
+gzip compressed data, was "tgqSim-0.2.6.tar", last modified: Wed May 15 08:11:22 2024, max compression
```

## Comparing `tgqSim-0.1.9.tar` & `tgqSim-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-15 00:53:46.000000 tgqSim-0.1.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-15 00:53:46.000000 tgqSim-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-15 00:53:48.654812 tgqSim-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-15 00:53:46.000000 tgqSim-0.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 00:53:48.654812 tgqSim-0.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-15 00:53:47.000000 tgqSim-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.653812 tgqSim-0.1.9/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22122 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-15 00:53:47.000000 tgqSim-0.1.9/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.654812 tgqSim-0.1.9/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    61952 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/lib/cuda_11-8_tgq_simulator.so
--rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-15 00:53:46.000000 tgqSim-0.1.9/tgqSim/lib/cuda_12-4_tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 00:53:48.653812 tgqSim-0.1.9/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-15 00:53:48.000000 tgqSim-0.1.9/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.053230 tgqSim-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-15 08:11:20.000000 tgqSim-0.2.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-15 08:11:20.000000 tgqSim-0.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-15 08:11:22.053230 tgqSim-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-15 08:11:20.000000 tgqSim-0.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:11:22.053230 tgqSim-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2024-05-15 08:11:21.000000 tgqSim-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.051230 tgqSim-0.2.6/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.052230 tgqSim-0.2.6/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22160 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-15 08:11:21.000000 tgqSim-0.2.6/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.053230 tgqSim-0.2.6/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    61952 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/lib/cuda_11-8_tgq_simulator.so
+-rw-rw-rw-   0 root         (0) root         (0)    73456 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/lib/cuda_12-4_tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.053230 tgqSim-0.2.6/tgqSim/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-15 08:11:20.000000 tgqSim-0.2.6/tgqSim/utils/dev_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:11:22.052230 tgqSim-0.2.6/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-15 08:11:21.000000 tgqSim-0.2.6/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-15 08:11:22.000000 tgqSim-0.2.6/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:11:21.000000 tgqSim-0.2.6/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-15 08:11:21.000000 tgqSim-0.2.6/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-15 08:11:21.000000 tgqSim-0.2.6/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.9/LICENSE` & `tgqSim-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/PKG-INFO` & `tgqSim-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.9
+Version: 0.2.6
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
-Keywords: tgq,quantum,simulator
+Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `tgqSim-0.1.9/setup.py` & `tgqSim-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.9',
+    version='0.2.6',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
     packages=["tgqSim", "tgqSim.GateSimulation"],
     install_requires=[
         'numpy>=1.19.0',
         'numba>=0.53.0',
-        'matplotlib>=3.5.3',
+        'matplotlib>=3.3.0',
         'GPUtil>=1.4.0'
     ],
     classifiers=[
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     ],
-    keywords=["tgq", "quantum", "simulator"],
+    keywords=["tgq", "quantum", "simulator", "noise"],
 )
```

### Comparing `tgqSim-0.1.9/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.2.6/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.2.6/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.2.6/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim/QuantumCircuit.py` & `tgqSim-0.2.6/tgqSim/QuantumCircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 @Modifider: Zhiqiang Wang
 @contact: wangzhiqiang@tgqs.net
 @version: 0.1.1
 @file: QuantumCircuit.py
 @time: 2024/04/19 15:36
 """
 from tgqSim.GateSimulation import SingleGate, DoubleGate, TripleGate
+from tgqSim.utils import dev_tools
 from typing import Union
 import random, os, ctypes
 import numpy as np
 import tgqSim.draw_circuit_tools as tools
 import matplotlib.pyplot as plt
 import GPUtil
 # from numba import njit, prange
@@ -150,15 +151,15 @@
         for deviceid in deviceList:
             if deviceid not in gpuidList:
                 raise ValueError("设置设备ID不存在")
         self.isgpu = True
         self.deviceid = deviceList
     
     def _run_with_device(self):
-        cuda_version = GPUtil.get_cuda_version().replace(".", "-")
+        cuda_version = dev_tools.get_cuda_version().replace(".", "-")
         lib_name = f"cuda_{cuda_version}_tgq_simulator.so"
         current_file_path = os.path.abspath(__file__)
         current_directory = os.path.dirname(current_file_path)
         dll_path = os.path.abspath(current_directory + '/lib/' + lib_name)
         lib = ctypes.CDLL(dll_path)
         lib.execute_circuit.argtypes = [
             ctypes.POINTER(Float2),
```

### Comparing `tgqSim-0.1.9/tgqSim/draw_circuit_tools.py` & `tgqSim-0.2.6/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim/lib/cuda_11-8_tgq_simulator.so` & `tgqSim-0.2.6/tgqSim/lib/cuda_11-8_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim/lib/cuda_12-4_tgq_simulator.so` & `tgqSim-0.2.6/tgqSim/lib/cuda_12-4_tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.9/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.2.6/tgqSim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.9
+Version: 0.2.6
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
-Keywords: tgq,quantum,simulator
+Keywords: tgq,quantum,simulator,noise
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

