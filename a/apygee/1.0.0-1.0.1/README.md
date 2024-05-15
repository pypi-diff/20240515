# Comparing `tmp/apygee-1.0.0.tar.gz` & `tmp/apygee-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apygee-1.0.0.tar", max compression
+gzip compressed data, was "apygee-1.0.1.tar", max compression
```

## Comparing `apygee-1.0.0.tar` & `apygee-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1060 2024-05-09 20:41:16.249841 apygee-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     1013 2024-05-09 20:52:50.019840 apygee-1.0.0/README.md
--rw-r--r--   0        0        0      555 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/__init__.py
--rw-r--r--   0        0        0     4014 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/constants.py
--rw-r--r--   0        0        0    10159 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/kepler.py
--rw-r--r--   0        0        0     2863 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/nb.py
--rw-r--r--   0        0        0    37115 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/orbit.py
--rw-r--r--   0        0        0    19124 2024-05-09 20:52:09.269840 apygee-1.0.0/apygee/plot.py
--rw-r--r--   0        0        0     6234 2024-05-09 20:41:16.249841 apygee-1.0.0/apygee/utils.py
--rw-r--r--   0        0        0      716 2024-05-09 20:51:50.249840 apygee-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 apygee-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-15 20:02:54.236495 apygee-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1072 2024-05-15 20:02:54.240495 apygee-1.0.1/README.md
+-rw-r--r--   0        0        0      555 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/__init__.py
+-rw-r--r--   0        0        0     4014 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/constants.py
+-rw-r--r--   0        0        0    10159 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/kepler.py
+-rw-r--r--   0        0        0     2863 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/nb.py
+-rw-r--r--   0        0        0    37115 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/orbit.py
+-rw-r--r--   0        0        0    19124 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/plot.py
+-rw-r--r--   0        0        0     6234 2024-05-15 20:02:54.240495 apygee-1.0.1/apygee/utils.py
+-rw-r--r--   0        0        0      716 2024-05-15 20:02:54.244495 apygee-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 apygee-1.0.1/PKG-INFO
```

### Comparing `apygee-1.0.0/LICENSE.md` & `apygee-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/README.md` & `apygee-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Apygee
 
 <p align="start">
   <a href="https://github.com/Pocket-titan/apygee">
-    <img src="logo.jpg" alt="Logo" width="200">
+    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.jpg" alt="Logo" width="200">
   </a>
 </p>
 
 Apygee (apogee + `py`) is a lightweight Python package for creating, manipulating and visualizing Kepler orbits.
 
 ## Installation
```

### Comparing `apygee-1.0.0/apygee/__init__.py` & `apygee-1.0.1/apygee/__init__.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/constants.py` & `apygee-1.0.1/apygee/constants.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/kepler.py` & `apygee-1.0.1/apygee/kepler.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/nb.py` & `apygee-1.0.1/apygee/nb.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/orbit.py` & `apygee-1.0.1/apygee/orbit.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/plot.py` & `apygee-1.0.1/apygee/plot.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/apygee/utils.py` & `apygee-1.0.1/apygee/utils.py`

 * *Files identical despite different names*

### Comparing `apygee-1.0.0/pyproject.toml` & `apygee-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apygee"
-version = "1.0.0"
+version = "1.0.1"
 description = "A package for creating, manipulating and visualizing Kepler orbits"
 authors = ["Jelmar Gerritsen <jelmargerritsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 matplotlib = "^3.8.3"
```

### Comparing `apygee-1.0.0/PKG-INFO` & `apygee-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: apygee
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for creating, manipulating and visualizing Kepler orbits
 Author: Jelmar Gerritsen
 Author-email: jelmargerritsen@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: plotly (>=5.20.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Apygee
 
 <p align="start">
   <a href="https://github.com/Pocket-titan/apygee">
-    <img src="logo.jpg" alt="Logo" width="200">
+    <img src="https://raw.githubusercontent.com/Pocket-titan/apygee/main/logo.jpg" alt="Logo" width="200">
   </a>
 </p>
 
 Apygee (apogee + `py`) is a lightweight Python package for creating, manipulating and visualizing Kepler orbits.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: apygee Version: 1.0.0 Summary: A package for
+Metadata-Version: 2.1 Name: apygee Version: 1.0.1 Summary: A package for
 creating, manipulating and visualizing Kepler orbits Author: Jelmar Gerritsen
 Author-email: jelmargerritsen@gmail.com Requires-Python: >=3.12,<4.0
-Classifier: Programming Language :: Python :: 3 Requires-Dist: ipywidgets
-(>=8.1.2,<9.0.0) Requires-Dist: matplotlib (>=3.8.3,<4.0.0) Requires-Dist:
-numpy (>=1.26.4,<2.0.0) Requires-Dist: plotly (>=5.20.0,<6.0.0) Description-
-Content-Type: text/markdown # Apygee
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0) Requires-
+Dist: matplotlib (>=3.8.3,<4.0.0) Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: plotly (>=5.20.0,<6.0.0) Description-Content-Type: text/markdown
+# Apygee
 _[_L_o_g_o_]
 Apygee (apogee + `py`) is a lightweight Python package for creating,
 manipulating and visualizing Kepler orbits. ## Installation ```bash pip install
 apygee ``` ## Usage The main export of Apygee is the `Orbit` class, which
 stores the keplerian elements and provides easy access to the astrodynamical
 properties of the orbit. It also contains methods for visualizing the orbit,
 and for performing mauevers in order to transfer to other orbits. ```python
```

