# Comparing `tmp/pymrm-1.3.4.tar.gz` & `tmp/pymrm-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymrm-1.3.4.tar", last modified: Sun May 12 23:29:19 2024, max compression
+gzip compressed data, was "pymrm-1.3.5.tar", last modified: Wed May 15 07:08:13 2024, max compression
```

## Comparing `pymrm-1.3.4.tar` & `pymrm-1.3.5.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:19.145528 pymrm-1.3.4/
--rw-rw-rw-   0        0        0       57 2024-02-01 11:20:15.000000 pymrm-1.3.4/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:18.579045 pymrm-1.3.4/.vscode/
--rw-rw-rw-   0        0        0      236 2024-04-17 10:45:15.000000 pymrm-1.3.4/.vscode/settings.json
--rw-rw-rw-   0        0        0      634 2023-07-13 10:36:17.000000 pymrm-1.3.4/Makefile
--rw-rw-rw-   0        0        0     2297 2024-05-12 23:29:19.143862 pymrm-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1461 2024-04-17 14:36:26.000000 pymrm-1.3.4/README.md
--rw-rw-rw-   0        0        0     2002 2024-04-18 08:57:14.000000 pymrm-1.3.4/conf.py
--rw-rw-rw-   0        0        0      107 2023-07-13 10:48:43.000000 pymrm-1.3.4/conf.rst
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:18.766348 pymrm-1.3.4/examples/
--rw-rw-rw-   0        0        0    72097 2024-05-01 15:57:28.000000 pymrm-1.3.4/examples/L3_demo_diffusion_reaction.ipynb
--rw-rw-rw-   0        0        0    72371 2024-05-01 15:56:54.000000 pymrm-1.3.4/examples/L3_demo_mrm_implementation_as_class.ipynb
--rw-rw-rw-   0        0        0    19000 2024-05-03 20:56:31.000000 pymrm-1.3.4/examples/L3_particle_model_non_linear.ipynb
--rw-rw-rw-   0        0        0    21475 2024-05-08 10:51:08.000000 pymrm-1.3.4/examples/L5_convection_diffusion_2D.ipynb
--rw-rw-rw-   0        0        0    12885 2024-05-08 18:45:38.000000 pymrm-1.3.4/examples/L5_demo.ipynb
--rw-rw-rw-   0        0        0   116764 2024-04-24 07:32:19.000000 pymrm-1.3.4/examples/annular_flow_reaction.ipynb
--rw-rw-rw-   0        0        0      526 2024-04-18 11:22:50.000000 pymrm-1.3.4/examples/debugging_pymrm_local.ipynb
--rw-rw-rw-   0        0        0    42800 2024-05-08 21:57:07.000000 pymrm-1.3.4/examples/different_diffusion_coefficients.ipynb
--rw-rw-rw-   0        0        0   702981 2024-04-20 14:00:38.000000 pymrm-1.3.4/examples/pymrm_examples.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:18.470147 pymrm-1.3.4/exercises/
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:18.885506 pymrm-1.3.4/exercises/L1/
--rw-rw-rw-   0        0        0   108821 2024-04-22 15:15:06.000000 pymrm-1.3.4/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb
--rw-rw-rw-   0        0        0   235059 2024-04-23 07:15:48.000000 pymrm-1.3.4/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb
--rw-rw-rw-   0        0        0   120538 2024-04-22 15:15:09.000000 pymrm-1.3.4/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:18.911391 pymrm-1.3.4/exercises/L2/
--rw-rw-rw-   0        0        0    97596 2024-04-29 20:12:56.000000 pymrm-1.3.4/exercises/L2/Exercise 2.1 - Single component convection.ipynb
--rw-rw-rw-   0        0        0     3192 2024-04-25 20:59:16.000000 pymrm-1.3.4/exercises/L2/Exercise 2.1 - Single component convection.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:19.064259 pymrm-1.3.4/exercises/L3/
--rw-rw-rw-   0        0        0    23669 2024-05-01 11:30:11.000000 pymrm-1.3.4/exercises/L3/Exercise 3.1 - one component 1D diffusion.ipynb
--rw-rw-rw-   0        0        0   111390 2024-05-09 17:43:32.000000 pymrm-1.3.4/exercises/L3/Exercise 3.2 - Multicomponent Diffusion.ipynb
--rw-rw-rw-   0        0        0   109502 2024-05-01 22:31:57.000000 pymrm-1.3.4/exercises/L3/Exercise 3.2 - counter diffusion.ipynb
--rw-rw-rw-   0        0        0    58536 2024-04-28 23:25:55.000000 pymrm-1.3.4/exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb
--rw-rw-rw-   0        0        0    52232 2024-05-03 13:52:02.000000 pymrm-1.3.4/exercises/L3/Exercise 3.4 - Convection Diffusion.ipynb
--rw-rw-rw-   0        0        0    35311 2024-05-03 13:21:05.000000 pymrm-1.3.4/exercises/L3/Exercise 3.5 - Particle model.ipynb
--rw-rw-rw-   0        0        0   208169 2024-05-09 23:33:18.000000 pymrm-1.3.4/exercises/L3/Exercise 3.6 - WeiszHicks.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:19.085472 pymrm-1.3.4/exercises/L4/
--rw-rw-rw-   0        0        0    38580 2024-05-02 08:34:30.000000 pymrm-1.3.4/exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb
--rw-rw-rw-   0        0        0     6148 2024-05-03 07:45:07.000000 pymrm-1.3.4/exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb
--rwxrwxrwx   0        0        0      800 2023-07-13 10:36:17.000000 pymrm-1.3.4/make.bat
--rw-rw-rw-   0        0        0       49 2023-07-13 10:56:28.000000 pymrm-1.3.4/modules.rst
--rw-rw-rw-   0        0        0      243 2024-05-08 19:51:43.000000 pymrm-1.3.4/mrm_environment.yml
--rw-rw-rw-   0        0        0     2528 2024-04-19 14:16:59.000000 pymrm-1.3.4/mrm_python_install.md
--rw-rw-rw-   0        0        0      111 2024-05-08 19:51:29.000000 pymrm-1.3.4/mrm_requirements.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:19.097902 pymrm-1.3.4/pymrm/
--rw-rw-rw-   0        0        0      389 2024-04-17 13:10:51.000000 pymrm-1.3.4/pymrm/__init__.py
--rw-rw-rw-   0        0        0    51266 2024-05-12 23:14:42.000000 pymrm-1.3.4/pymrm/pymrm.py
-drwxrwxrwx   0        0        0        0 2024-05-12 23:29:19.135777 pymrm-1.3.4/pymrm.egg-info/
--rw-rw-rw-   0        0        0     2297 2024-05-12 23:29:18.000000 pymrm-1.3.4/pymrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2024-05-12 23:29:18.000000 pymrm-1.3.4/pymrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 23:29:18.000000 pymrm-1.3.4/pymrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-12 23:29:18.000000 pymrm-1.3.4/pymrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-12 23:29:18.000000 pymrm-1.3.4/pymrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1060 2024-05-12 23:19:26.000000 pymrm-1.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 23:29:19.146502 pymrm-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      121 2023-07-13 10:48:43.000000 pymrm-1.3.4/test_mrm.rst
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:13.125311 pymrm-1.3.5/
+-rw-rw-rw-   0        0        0       57 2024-02-01 11:20:15.000000 pymrm-1.3.5/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.342704 pymrm-1.3.5/.vscode/
+-rw-rw-rw-   0        0        0      236 2024-04-17 10:45:15.000000 pymrm-1.3.5/.vscode/settings.json
+-rw-rw-rw-   0        0        0      634 2023-07-13 10:36:17.000000 pymrm-1.3.5/Makefile
+-rw-rw-rw-   0        0        0     2297 2024-05-15 07:08:13.124258 pymrm-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1461 2024-04-17 14:36:26.000000 pymrm-1.3.5/README.md
+-rw-rw-rw-   0        0        0     2002 2024-04-18 08:57:14.000000 pymrm-1.3.5/conf.py
+-rw-rw-rw-   0        0        0      107 2023-07-13 10:48:43.000000 pymrm-1.3.5/conf.rst
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.607140 pymrm-1.3.5/examples/
+-rw-rw-rw-   0        0        0    72097 2024-05-01 15:57:28.000000 pymrm-1.3.5/examples/L3_demo_diffusion_reaction.ipynb
+-rw-rw-rw-   0        0        0    72371 2024-05-01 15:56:54.000000 pymrm-1.3.5/examples/L3_demo_mrm_implementation_as_class.ipynb
+-rw-rw-rw-   0        0        0    19000 2024-05-03 20:56:31.000000 pymrm-1.3.5/examples/L3_particle_model_non_linear.ipynb
+-rw-rw-rw-   0        0        0    21475 2024-05-08 10:51:08.000000 pymrm-1.3.5/examples/L5_convection_diffusion_2D.ipynb
+-rw-rw-rw-   0        0        0    12885 2024-05-08 18:45:38.000000 pymrm-1.3.5/examples/L5_demo.ipynb
+-rw-rw-rw-   0        0        0   116764 2024-04-24 07:32:19.000000 pymrm-1.3.5/examples/annular_flow_reaction.ipynb
+-rw-rw-rw-   0        0        0      526 2024-04-18 11:22:50.000000 pymrm-1.3.5/examples/debugging_pymrm_local.ipynb
+-rw-rw-rw-   0        0        0    42800 2024-05-08 21:57:07.000000 pymrm-1.3.5/examples/different_diffusion_coefficients.ipynb
+-rw-rw-rw-   0        0        0   702981 2024-04-20 14:00:38.000000 pymrm-1.3.5/examples/pymrm_examples.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.202113 pymrm-1.3.5/exercises/
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.757710 pymrm-1.3.5/exercises/L1/
+-rw-rw-rw-   0        0        0   108821 2024-04-22 15:15:06.000000 pymrm-1.3.5/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb
+-rw-rw-rw-   0        0        0   235059 2024-04-23 07:15:48.000000 pymrm-1.3.5/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb
+-rw-rw-rw-   0        0        0   120538 2024-04-22 15:15:09.000000 pymrm-1.3.5/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.770550 pymrm-1.3.5/exercises/L2/
+-rw-rw-rw-   0        0        0    97596 2024-04-29 20:12:56.000000 pymrm-1.3.5/exercises/L2/Exercise 2.1 - Single component convection.ipynb
+-rw-rw-rw-   0        0        0     3192 2024-04-25 20:59:16.000000 pymrm-1.3.5/exercises/L2/Exercise 2.1 - Single component convection.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:12.975304 pymrm-1.3.5/exercises/L3/
+-rw-rw-rw-   0        0        0    23669 2024-05-01 11:30:11.000000 pymrm-1.3.5/exercises/L3/Exercise 3.1 - one component 1D diffusion.ipynb
+-rw-rw-rw-   0        0        0   111390 2024-05-09 17:43:32.000000 pymrm-1.3.5/exercises/L3/Exercise 3.2 - Multicomponent Diffusion.ipynb
+-rw-rw-rw-   0        0        0   109502 2024-05-01 22:31:57.000000 pymrm-1.3.5/exercises/L3/Exercise 3.2 - counter diffusion.ipynb
+-rw-rw-rw-   0        0        0    58536 2024-04-28 23:25:55.000000 pymrm-1.3.5/exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb
+-rw-rw-rw-   0        0        0    52232 2024-05-03 13:52:02.000000 pymrm-1.3.5/exercises/L3/Exercise 3.4 - Convection Diffusion.ipynb
+-rw-rw-rw-   0        0        0    35311 2024-05-03 13:21:05.000000 pymrm-1.3.5/exercises/L3/Exercise 3.5 - Particle model.ipynb
+-rw-rw-rw-   0        0        0   208169 2024-05-09 23:33:18.000000 pymrm-1.3.5/exercises/L3/Exercise 3.6 - WeiszHicks.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:13.009517 pymrm-1.3.5/exercises/L4/
+-rw-rw-rw-   0        0        0    38580 2024-05-02 08:34:30.000000 pymrm-1.3.5/exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb
+-rw-rw-rw-   0        0        0     6148 2024-05-03 07:45:07.000000 pymrm-1.3.5/exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:13.038022 pymrm-1.3.5/exercises/L7/
+-rw-rw-rw-   0        0        0   104550 2024-05-12 23:49:47.000000 pymrm-1.3.5/exercises/L7/Exercise 7.2.ipynb
+-rw-rw-rw-   0        0        0     5507 2024-05-13 05:42:05.000000 pymrm-1.3.5/exercises/L7/Exercise 7.2.py
+-rwxrwxrwx   0        0        0      800 2023-07-13 10:36:17.000000 pymrm-1.3.5/make.bat
+-rw-rw-rw-   0        0        0       49 2023-07-13 10:56:28.000000 pymrm-1.3.5/modules.rst
+-rw-rw-rw-   0        0        0      243 2024-05-08 19:51:43.000000 pymrm-1.3.5/mrm_environment.yml
+-rw-rw-rw-   0        0        0     2528 2024-04-19 14:16:59.000000 pymrm-1.3.5/mrm_python_install.md
+-rw-rw-rw-   0        0        0      111 2024-05-08 19:51:29.000000 pymrm-1.3.5/mrm_requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:13.057463 pymrm-1.3.5/pymrm/
+-rw-rw-rw-   0        0        0      389 2024-04-17 13:10:51.000000 pymrm-1.3.5/pymrm/__init__.py
+-rw-rw-rw-   0        0        0    51620 2024-05-15 07:06:52.000000 pymrm-1.3.5/pymrm/pymrm.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:08:13.121253 pymrm-1.3.5/pymrm.egg-info/
+-rw-rw-rw-   0        0        0     2297 2024-05-15 07:08:11.000000 pymrm-1.3.5/pymrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1707 2024-05-15 07:08:12.000000 pymrm-1.3.5/pymrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 07:08:11.000000 pymrm-1.3.5/pymrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-15 07:08:11.000000 pymrm-1.3.5/pymrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 07:08:11.000000 pymrm-1.3.5/pymrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1060 2024-05-15 07:07:12.000000 pymrm-1.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 07:08:13.125311 pymrm-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      121 2023-07-13 10:48:43.000000 pymrm-1.3.5/test_mrm.rst
```

### Comparing `pymrm-1.3.4/Makefile` & `pymrm-1.3.5/Makefile`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/PKG-INFO` & `pymrm-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrm
-Version: 1.3.4
+Version: 1.3.5
 Summary: Functions for multiphase reactor modeling
 Author-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>, "M. van Sint Annaland" <M.v.SintAnnaland@tue.nl>, "M. Galanti" <m.galanti@tue.nl>, "D.R. Rieder" <d.r.rieder@tue.nl>
 Maintainer-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>
 Project-URL: Homepage, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Project-URL: Repository, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Keywords: MRM,modeling,multiphase,diffusion,convection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pymrm-1.3.4/README.md` & `pymrm-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/conf.py` & `pymrm-1.3.5/conf.py`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/L3_demo_diffusion_reaction.ipynb` & `pymrm-1.3.5/examples/L3_demo_diffusion_reaction.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/L3_demo_mrm_implementation_as_class.ipynb` & `pymrm-1.3.5/examples/L3_demo_mrm_implementation_as_class.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/L3_particle_model_non_linear.ipynb` & `pymrm-1.3.5/examples/L3_particle_model_non_linear.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/L5_convection_diffusion_2D.ipynb` & `pymrm-1.3.5/examples/L5_convection_diffusion_2D.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/L5_demo.ipynb` & `pymrm-1.3.5/examples/L5_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/annular_flow_reaction.ipynb` & `pymrm-1.3.5/examples/annular_flow_reaction.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/debugging_pymrm_local.ipynb` & `pymrm-1.3.5/examples/debugging_pymrm_local.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/different_diffusion_coefficients.ipynb` & `pymrm-1.3.5/examples/different_diffusion_coefficients.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/examples/pymrm_examples.ipynb` & `pymrm-1.3.5/examples/pymrm_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb` & `pymrm-1.3.5/exercises/L1/Exercise 1.1 - First order reaction in a batch reactor.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb` & `pymrm-1.3.5/exercises/L1/Exercise 1.2 - Equilibrium-consecutive reaction system in a batch reactor.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb` & `pymrm-1.3.5/exercises/L1/Exercise 1.3 - Steady-state 1D adiabatic fixed bed reactor model.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L2/Exercise 2.1 - Single component convection.ipynb` & `pymrm-1.3.5/exercises/L2/Exercise 2.1 - Single component convection.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L2/Exercise 2.1 - Single component convection.py` & `pymrm-1.3.5/exercises/L2/Exercise 2.1 - Single component convection.py`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.1 - one component 1D diffusion.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.1 - one component 1D diffusion.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.2 - Multicomponent Diffusion.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.2 - Multicomponent Diffusion.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.2 - counter diffusion.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.2 - counter diffusion.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.4 - Convection Diffusion.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.4 - Convection Diffusion.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.5 - Particle model.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.5 - Particle model.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L3/Exercise 3.6 - WeiszHicks.ipynb` & `pymrm-1.3.5/exercises/L3/Exercise 3.6 - WeiszHicks.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb` & `pymrm-1.3.5/exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb` & `pymrm-1.3.5/exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/make.bat` & `pymrm-1.3.5/make.bat`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/mrm_python_install.md` & `pymrm-1.3.5/mrm_python_install.md`

 * *Files identical despite different names*

### Comparing `pymrm-1.3.4/pymrm/pymrm.py` & `pymrm-1.3.5/pymrm/pymrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,16 @@
     # spatially discretize a direction, but still use a BC, e.g. with a mass transfer coefficient
     # It is a bit subtle because in this case the two opposite faces influence each other
     if (shape_t[1] == 1):
         if (x_c is None):
             x_c = 0.5*(x_f[0:-1] + x_f[1:])
         i_c = shape_t[2] * np.arange(shape_t[0]).reshape((-1, 1, 1)) + np.array(
             (0, 0)).reshape((1, -1, 1)) + np.arange(shape_t[2]).reshape((1, 1, -1))
+        i_f = shape_t[2] * np.arange(shape_t[0]).reshape((-1, 1, 1)) + shape_t[2] * np.array([0,1]).reshape((
+            1, -1, 1)) + np.arange(shape_t[2]).reshape((1, 1, -1))
         values = np.zeros(shape_f_t)
         alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
         alpha_0R = alpha_1 - alpha_2R
         fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
@@ -482,14 +484,16 @@
 
     # Handle special case with one cell in the dimension axis
     if (shape_t[1] == 1):
         if (x_c is None):
             x_c = 0.5*(x_f[0:-1] + x_f[1:])
         i_c = shape_t[2] * np.arange(shape_t[0]).reshape((-1, 1, 1)) + np.array(
             (0, 0)).reshape((1, -1, 1)) + np.arange(shape_t[2]).reshape((1, 1, -1))
+        i_f = shape_t[2] * np.arange(shape_t[0]).reshape((-1, 1, 1)) + shape_t[2] * np.array([0,1]).reshape((
+            1, -1, 1)) + np.arange(shape_t[2]).reshape((1, 1, -1))
         values = np.zeros(shape_f_t)
         alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
         alpha_0R = alpha_1 - alpha_2R        
         fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
```

### Comparing `pymrm-1.3.4/pymrm.egg-info/PKG-INFO` & `pymrm-1.3.5/pymrm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymrm
-Version: 1.3.4
+Version: 1.3.5
 Summary: Functions for multiphase reactor modeling
 Author-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>, "M. van Sint Annaland" <M.v.SintAnnaland@tue.nl>, "M. Galanti" <m.galanti@tue.nl>, "D.R. Rieder" <d.r.rieder@tue.nl>
 Maintainer-email: "E.A.J.F. Peters" <e.a.j.f.peters@tue.nl>
 Project-URL: Homepage, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Project-URL: Repository, https://gitlab.tue.nl/SMM/research_projects/eajfpeters/pymrm/
 Keywords: MRM,modeling,multiphase,diffusion,convection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pymrm-1.3.4/pymrm.egg-info/SOURCES.txt` & `pymrm-1.3.5/pymrm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 exercises/L3/Exercise 3.2 - counter diffusion.ipynb
 exercises/L3/Exercise 3.3 - Multi-component 1D counter-current convection with reaction.ipynb
 exercises/L3/Exercise 3.4 - Convection Diffusion.ipynb
 exercises/L3/Exercise 3.5 - Particle model.ipynb
 exercises/L3/Exercise 3.6 - WeiszHicks.ipynb
 exercises/L4/Exercise 4.1 - Counter-current column processes.ipynb
 exercises/L4/Exercise 4.2 - Reactor model for heterogeneous bubble columns.ipynb
+exercises/L7/Exercise 7.2.ipynb
+exercises/L7/Exercise 7.2.py
 pymrm/__init__.py
 pymrm/pymrm.py
 pymrm.egg-info/PKG-INFO
 pymrm.egg-info/SOURCES.txt
 pymrm.egg-info/dependency_links.txt
 pymrm.egg-info/requires.txt
 pymrm.egg-info/top_level.txt
```

### Comparing `pymrm-1.3.4/pyproject.toml` & `pymrm-1.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymrm"
-version = "1.3.4"
+version = "1.3.5"
 dependencies = [
     "numpy>=1.26",
     "scipy>=1.13",
 ]
 authors = [
     {name = "E.A.J.F. Peters", email = "e.a.j.f.peters@tue.nl"},
     {name = "M. van Sint Annaland", email= "M.v.SintAnnaland@tue.nl"},
```

