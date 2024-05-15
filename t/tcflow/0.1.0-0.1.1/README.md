# Comparing `tmp/tcflow-0.1.0.tar.gz` & `tmp/tcflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcflow-0.1.0.tar", last modified: Tue Jun  6 08:05:48 2023, max compression
+gzip compressed data, was "tcflow-0.1.1.tar", last modified: Wed May 15 17:35:08 2024, max compression
```

## Comparing `tcflow-0.1.0.tar` & `tcflow-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-05-28 09:19:52.000000 tcflow-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    16106 2023-06-06 08:05:48.509075 tcflow-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    15282 2023-05-29 20:07:24.000000 tcflow-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 08:05:48.509075 tcflow-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-06-06 08:04:43.000000 tcflow-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/tcflow/
--rw-rw-rw-   0        0        0     2784 2023-05-28 20:00:29.000000 tcflow-0.1.0/tcflow/EMD_MD_OPs.py
--rw-rw-rw-   0        0        0     3891 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/EMD_reprocess_OPs.py
--rw-rw-rw-   0        0        0     7074 2023-05-29 20:29:24.000000 tcflow-0.1.0/tcflow/EMD_run.py
--rw-rw-rw-   0        0        0     1973 2023-05-28 20:00:32.000000 tcflow-0.1.0/tcflow/NEMD_MD_OPs.py
--rw-rw-rw-   0        0        0     6240 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/NEMD_reprocess_OPs.py
--rw-rw-rw-   0        0        0     6638 2023-05-28 19:48:42.000000 tcflow-0.1.0/tcflow/NEMD_run.py
--rw-rw-rw-   0        0        0        0 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/__init__.py
--rw-rw-rw-   0        0        0     9272 2023-05-29 13:04:41.000000 tcflow-0.1.0/tcflow/input_gen.py
--rw-rw-rw-   0        0        0     1395 2023-05-28 09:19:52.000000 tcflow-0.1.0/tcflow/submit.py
-drwxrwxrwx   0        0        0        0 2023-06-06 08:05:48.509075 tcflow-0.1.0/tcflow.egg-info/
--rw-rw-rw-   0        0        0    16106 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 08:05:48.000000 tcflow-0.1.0/tcflow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 17:35:08.908954 tcflow-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-28 09:19:52.000000 tcflow-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    16277 2024-05-15 17:35:08.907954 tcflow-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15282 2023-05-29 20:07:24.000000 tcflow-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:35:08.908954 tcflow-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-15 17:34:24.000000 tcflow-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:35:08.899953 tcflow-0.1.1/tcflow/
+-rw-rw-rw-   0        0        0     2816 2024-05-15 17:15:45.000000 tcflow-0.1.1/tcflow/EMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     3891 2023-05-28 09:19:52.000000 tcflow-0.1.1/tcflow/EMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     7088 2024-05-15 17:13:49.000000 tcflow-0.1.1/tcflow/EMD_run.py
+-rw-rw-rw-   0        0        0     1973 2023-05-28 20:00:32.000000 tcflow-0.1.1/tcflow/NEMD_MD_OPs.py
+-rw-rw-rw-   0        0        0     6240 2023-05-28 09:19:52.000000 tcflow-0.1.1/tcflow/NEMD_reprocess_OPs.py
+-rw-rw-rw-   0        0        0     6638 2023-05-28 19:48:42.000000 tcflow-0.1.1/tcflow/NEMD_run.py
+-rw-rw-rw-   0        0        0        0 2023-05-28 09:19:52.000000 tcflow-0.1.1/tcflow/__init__.py
+-rw-rw-rw-   0        0        0     9272 2023-05-29 13:04:41.000000 tcflow-0.1.1/tcflow/input_gen.py
+-rw-rw-rw-   0        0        0     1395 2023-05-28 09:19:52.000000 tcflow-0.1.1/tcflow/submit.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:35:08.906956 tcflow-0.1.1/tcflow.egg-info/
+-rw-rw-rw-   0        0        0    16277 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 17:35:08.000000 tcflow-0.1.1/tcflow.egg-info/top_level.txt
```

### Comparing `tcflow-0.1.0/LICENSE` & `tcflow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/PKG-INFO` & `tcflow-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: tcflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A framework for thermal conductivity calculation based on EMD&NEMD methods
 Home-page: https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git
 Author: Wenjie Zhang
 Author-email: gdbhcxhmjk@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides: tcflow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydflow>=1.6.27
+Requires-Dist: lbg>=1.2.13
+Requires-Dist: dpdata>=0.2.7
+Requires-Dist: matplotlib>=3.6.3
+Requires-Dist: sportran
+Requires-Dist: numpy
 
 # Table of contents
 - [About ThermalConductivity-Workflow](#ThermalConductivity-Workflow)
 - [Workflow Framework](#Workflow-Framework)
 - [Prepare Input File](#Prepare-input-file)
 # About ThermalConductivity-Workflow
 ThermalConductivity-Workflow is designed to compute thermal conductivity of different materials based on Non-Equilibrium &amp; Equilibrium Molecular Dynamics Simulations. It is supported by [dflow](https://github.com/deepmodeling/dflow), a Python framework for constructing scientific computing workflows.
```

### Comparing `tcflow-0.1.0/README.md` & `tcflow-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/setup.py` & `tcflow-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tcflow",
-    version="0.1.0",
+    version="0.1.1",
     author="Wenjie Zhang",
     author_email="gdbhcxhmjk@163.com",
     description="A framework for thermal conductivity calculation based on EMD&NEMD methods",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git",
     packages=setuptools.find_packages(),
```

### Comparing `tcflow-0.1.0/tcflow/EMD_MD_OPs.py` & `tcflow-0.1.1/tcflow/EMD_MD_OPs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     @OP.exec_sign_check
     def execute(
             self,
             op_in: OPIO,
     ) -> OPIO:
         input =op_in["input"]
+        param = op_in["param"]
         data = op_in["data"]
         force_field = op_in["force_field"]
         print(input)
         print(data)
         print(force_field)
         Path('in.lammps').symlink_to(input)
         Path('data.lammps').symlink_to(data)
```

### Comparing `tcflow-0.1.0/tcflow/EMD_reprocess_OPs.py` & `tcflow-0.1.1/tcflow/EMD_reprocess_OPs.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow/EMD_run.py` & `tcflow-0.1.1/tcflow/EMD_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     if (param["force_field"]):force_field = upload_artifact(param["force_field"])
     else:force_field = upload_artifact(param["structure"])
     gpu_dispatcher_executor,cpu_dispatcher_executor=load_machine(machine_param)
 
     wf = Workflow("emd-tc")
     NVT = Step("NVT",
                 PythonOPTemplate(RunNVT,image="python:3.8" if type=="cluster" else lammps_image,python_packages=upload_python_packages,),
-                artifacts={"data":data_input,"input":NVT_input,"force_field":force_field},#"input_gen":gen,
+                artifacts={"data":data_input,"param":param,"input":NVT_input,"force_field":force_field},#"input_gen":gen,
                 executor=gpu_dispatcher_executor)
     wf.add(NVT)
     Configurations=Step("Config",
                 PythonOPTemplate(MakeConfigurations,image="python:3.8" if type=="cluster" else tc_image),
                 parameters={"numb_lmp":param['num_configurations']},
                 artifacts={"dump": NVT.outputs.artifacts["dump"]},
                 executor=cpu_dispatcher_executor)
```

### Comparing `tcflow-0.1.0/tcflow/NEMD_MD_OPs.py` & `tcflow-0.1.1/tcflow/NEMD_MD_OPs.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow/NEMD_reprocess_OPs.py` & `tcflow-0.1.1/tcflow/NEMD_reprocess_OPs.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow/NEMD_run.py` & `tcflow-0.1.1/tcflow/NEMD_run.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow/input_gen.py` & `tcflow-0.1.1/tcflow/input_gen.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow/submit.py` & `tcflow-0.1.1/tcflow/submit.py`

 * *Files identical despite different names*

### Comparing `tcflow-0.1.0/tcflow.egg-info/PKG-INFO` & `tcflow-0.1.1/tcflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: tcflow
-Version: 0.1.0
+Version: 0.1.1
 Summary: A framework for thermal conductivity calculation based on EMD&NEMD methods
 Home-page: https://github.com/gdbhcxhmjk-z/ThermalConductivity-Workflow.git
 Author: Wenjie Zhang
 Author-email: gdbhcxhmjk@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Provides: tcflow
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydflow>=1.6.27
+Requires-Dist: lbg>=1.2.13
+Requires-Dist: dpdata>=0.2.7
+Requires-Dist: matplotlib>=3.6.3
+Requires-Dist: sportran
+Requires-Dist: numpy
 
 # Table of contents
 - [About ThermalConductivity-Workflow](#ThermalConductivity-Workflow)
 - [Workflow Framework](#Workflow-Framework)
 - [Prepare Input File](#Prepare-input-file)
 # About ThermalConductivity-Workflow
 ThermalConductivity-Workflow is designed to compute thermal conductivity of different materials based on Non-Equilibrium &amp; Equilibrium Molecular Dynamics Simulations. It is supported by [dflow](https://github.com/deepmodeling/dflow), a Python framework for constructing scientific computing workflows.
```

