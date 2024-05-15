# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.4.3.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.3.tar", last modified: Tue May 14 12:55:50 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.4.4.tar", last modified: Tue May 14 13:14:03 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.4.3.tar` & `pyrt_lib_rasmusklitgaard-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.3/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.3/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-14 12:55:45.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.124553 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11578 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/parameter_parser.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32694 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/pyrt_database.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/resample.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-14 12:55:47.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 12:55:50.124553 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-14 12:55:50.000000 pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-14 12:55:50.128553 pyrt_lib_rasmusklitgaard-0.4.3/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 13:14:03.489951 pyrt_lib_rasmusklitgaard-0.4.4/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.4/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 13:14:03.489951 pyrt_lib_rasmusklitgaard-0.4.4/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.4.4/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)     1061 2024-05-14 13:13:57.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 13:14:03.489951 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      150 2024-05-01 13:21:00.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    11580 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    14910 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     8758 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/parameter_parser.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32657 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12316 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/pyrt_database.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4724 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/resample.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-05-14 13:14:01.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-05-14 13:14:03.489951 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1777 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      714 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      134 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/entry_points.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      141 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-05-14 13:14:03.000000 pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-05-14 13:14:03.489951 pyrt_lib_rasmusklitgaard-0.4.4/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/LICENSE` & `pyrt_lib_rasmusklitgaard-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.3
+Version: 0.4.4
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/README.md` & `pyrt_lib_rasmusklitgaard-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 			subset = dose_array[np.where(dose_array>=d)] 
 			subset = subset[np.where(subset <d+dose_step)]
 			volume = len(subset.flatten()) / N
 			eud += volume * (d + dose_step/2)**(1/n)
 	except ValueError:
 		print("ValueError in eud_calculator_dose_array")
 		print("Entering interactive for investigation")
-		code_interact(globals(), locals())
+		# code_interact(globals(), locals())
 		exit()
 
 	return eud**n
 
 def get_differential_dvh(dose_array, dose_step):
 	if np.prod(np.shape(dose_array)) == 0:
 		return np.array([np.array([]),np.array([])])
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/parameter_parser.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/parameter_parser.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 		try:
 			if self.wanted_structures == "default":
 				self.wanted_structures = ["ctv", "bladder", "bladder wall", "rectum", "rectal wall", "Bladder Wall", "Rectal Wall", "Rectum", "Bladder", "CTV", "Rectal_Wall", "Bladder_Wall"]
 			self.actual_structure_names = self.get_actual_structure_names(self.wanted_structures , *args, **kwargs)
 		except AttributeError as e:
 			print("THERE HAS BEEN AN ATTRIBUTE ERROR")
 			print(str(e))
-			code_interact(globals(),locals())
 		t7=time.time()
 
 		self.set_structure_indices()
 		t8=time.time()
 
 
 	def get_dvh_param(self, structure, model, key) -> float:
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/pyrt_database.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/pyrt_database.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/resample.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/resample.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.4.3
+Version: 0.4.4
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.4.3/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.4.4/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

