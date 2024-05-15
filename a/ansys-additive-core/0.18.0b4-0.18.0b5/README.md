# Comparing `tmp/ansys_additive_core-0.18.0b4.tar.gz` & `tmp/ansys_additive_core-0.18.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_additive_core-0.18.0b4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_additive_core-0.18.0b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_additive_core-0.18.0b4.tar` & `ansys_additive_core-0.18.0b5.tar`

### file list

```diff
@@ -1,41 +1,34 @@
--rw-r--r--   0        0        0     1097 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/LICENSE
--rw-r--r--   0        0        0     3904 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/README.rst
--rw-r--r--   0        0        0     3679 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/pyproject.toml
--rw-r--r--   0        0        0     3136 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/__init__.py
--rw-r--r--   0        0        0    26598 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/additive.py
--rw-r--r--   0        0        0     1764 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/conversions.py
--rw-r--r--   0        0        0     3224 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/download.py
--rw-r--r--   0        0        0     1437 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/__init__.py
--rw-r--r--   0        0        0     9864 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/downloads.py
--rw-r--r--   0        0        0     1314 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/exceptions.py
--rw-r--r--   0        0        0     5315 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/geometry_file.py
--rw-r--r--   0        0        0     9107 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/logger.py
--rw-r--r--   0        0        0    13089 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/machine.py
--rw-r--r--   0        0        0    33644 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/material.py
--rw-r--r--   0        0        0     8255 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/material_tuning.py
--rw-r--r--   0        0        0    25863 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure.py
--rw-r--r--   0        0        0    17413 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure_3d.py
--rw-r--r--   0        0        0     1393 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/misc.py
--rw-r--r--   0        0        0     1629 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/__init__.py
--rw-r--r--   0        0        0     6296 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/constants.py
--rw-r--r--   0        0        0     1485 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/__init__.py
--rw-r--r--   0        0        0     3318 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/_common_controls.py
--rw-r--r--   0        0        0     8111 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/ave_grain_size_plot.py
--rw-r--r--   0        0        0    10178 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_contour_plot.py
--rw-r--r--   0        0        0     8770 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/porosity_eval_plot.py
--rw-r--r--   0        0        0     6387 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/show_table.py
--rw-r--r--   0        0        0     8617 2024-04-30 21:46:08.687844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/single_bead_eval_plot.py
--rw-r--r--   0        0        0    10207 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_runner.py
--rw-r--r--   0        0        0    93178 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_study.py
--rw-r--r--   0        0        0     3252 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_utils.py
--rw-r--r--   0        0        0     6943 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/porosity.py
--rw-r--r--   0        0        0     4835 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/progress_handler.py
--rw-r--r--   0        0        0     1373 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/__init__.py
--rw-r--r--   0        0        0     1711 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/constants.py
--rw-r--r--   0        0        0     5563 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/local_server.py
--rw-r--r--   0        0        0     2627 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/network_utils.py
--rw-r--r--   0        0        0     8078 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/server_connection.py
--rw-r--r--   0        0        0     2739 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/simulation.py
--rw-r--r--   0        0        0     8059 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/single_bead.py
--rw-r--r--   0        0        0    10190 2024-04-30 21:46:08.691844 ansys_additive_core-0.18.0b4/src/ansys/additive/core/thermal_history.py
--rw-r--r--   0        0        0     7566 1970-01-01 00:00:00.000000 ansys_additive_core-0.18.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-15 16:53:27.488986 ansys_additive_core-0.18.0b5/LICENSE
+-rw-r--r--   0        0        0     3904 2024-05-15 16:53:27.488986 ansys_additive_core-0.18.0b5/README.rst
+-rw-r--r--   0        0        0     3336 2024-05-15 16:53:27.488986 ansys_additive_core-0.18.0b5/pyproject.toml
+-rw-r--r--   0        0        0     3439 2024-05-15 16:53:27.488986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/__init__.py
+-rw-r--r--   0        0        0    26598 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/additive.py
+-rw-r--r--   0        0        0     1764 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/conversions.py
+-rw-r--r--   0        0        0     3224 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/download.py
+-rw-r--r--   0        0        0     1437 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/examples/__init__.py
+-rw-r--r--   0        0        0     9864 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/examples/downloads.py
+-rw-r--r--   0        0        0     1314 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/exceptions.py
+-rw-r--r--   0        0        0     5315 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/geometry_file.py
+-rw-r--r--   0        0        0     9107 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/logger.py
+-rw-r--r--   0        0        0    13089 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/machine.py
+-rw-r--r--   0        0        0    33644 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/material.py
+-rw-r--r--   0        0        0     8255 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/material_tuning.py
+-rw-r--r--   0        0        0    25863 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/microstructure.py
+-rw-r--r--   0        0        0    17413 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/microstructure_3d.py
+-rw-r--r--   0        0        0     1393 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/misc.py
+-rw-r--r--   0        0        0     1698 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/__init__.py
+-rw-r--r--   0        0        0     6296 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/constants.py
+-rw-r--r--   0        0        0    10207 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_runner.py
+-rw-r--r--   0        0        0    93729 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_study.py
+-rw-r--r--   0        0        0     3252 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_utils.py
+-rw-r--r--   0        0        0     6943 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/porosity.py
+-rw-r--r--   0        0        0     4835 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/progress_handler.py
+-rw-r--r--   0        0        0     1373 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/__init__.py
+-rw-r--r--   0        0        0     1711 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/constants.py
+-rw-r--r--   0        0        0     5563 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/local_server.py
+-rw-r--r--   0        0        0     2627 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/network_utils.py
+-rw-r--r--   0        0        0     8102 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/server_connection.py
+-rw-r--r--   0        0        0     2739 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/simulation.py
+-rw-r--r--   0        0        0     8059 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/single_bead.py
+-rw-r--r--   0        0        0    10190 2024-05-15 16:53:27.492986 ansys_additive_core-0.18.0b5/src/ansys/additive/core/thermal_history.py
+-rw-r--r--   0        0        0     7273 1970-01-01 00:00:00.000000 ansys_additive_core-0.18.0b5/PKG-INFO
```

### Comparing `ansys_additive_core-0.18.0b4/LICENSE` & `ansys_additive_core-0.18.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/README.rst` & `ansys_additive_core-0.18.0b5/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/pyproject.toml` & `ansys_additive_core-0.18.0b5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-additive-core"
-version = "0.18.0b4"
+version = "0.18.0b5"
 description = "A Python client for the Ansys Additive service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -31,17 +31,15 @@
     "google-api-python-client>=1.7.11",
     "googleapis-common-protos>=1.52.0",
     "grpcio>=1.35.0",
     "grpcio-health-checking>=1.45.0",
     "importlib-metadata>=4.0",
     "numpy>=1.20.3",
     "pandas>=1.3.2",
-    "panel>=1.2.1",
     "platformdirs>=3.8.0",
-    "plotly>=5.16.1",
     "protobuf>=3.20.2,<5",
     "six>=1.16.0",
     "tqdm>=4.45.0",
     "pydantic>=2.6.3",
 ]
 
 [project.optional-dependencies]
@@ -50,39 +48,33 @@
     "dill==0.3.8",
     "google-api-python-client==2.122.0",
     "googleapis-common-protos==1.63.0",
     "grpcio==1.60.0",
     "grpcio-health-checking==1.48.2",
     "numpy==1.26.4",
     "pandas==2.2.2",
-    "panel==1.4.2",
     "platformdirs==4.2.1",
-    "plotly==5.21.0",
     "protobuf==4.25.3",
     "six==1.16.0",
-    "tqdm==4.66.2",
+    "tqdm==4.66.4",
     "pydantic==2.7.1",
     "pytest==8.2.0",
     "pytest-cov==5.0.0",
 ]
 
 doc = [
-    "ansys-sphinx-theme==0.15.2",
+    "ansys-sphinx-theme[autoapi]==0.15.2",
     "enum-tools==0.12.0",
     "jupyter_sphinx==0.5.3",
     "matplotlib==3.8.4",
     "numpydoc==1.7.0",
-    "panel==1.4.2",
     "phantomjs==1.4.1",
     "pypandoc==1.13",
-    "pyvista==0.43.6",
-    "selenium==4.20.0",
+    "pyvista==0.43.7",
     "sphinx==7.3.7",
-    "sphinx-autoapi==3.0.0",
-    #"sphinx-autoapi @ git+https://github.com/ansys/sphinx-autoapi@feat/single-page-stable",
     "sphinx-autodoc-typehints==2.1.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-design==0.5.0",
     "sphinx-gallery==0.16.0",
     "sphinx-jinja==2.0.2",
     "sphinx-notfound-page==1.0.0",
     "sphinx-toolbox==3.5.0",
@@ -107,15 +99,14 @@
 force_sort_within_sections = true
 line_length = 100
 default_section = "THIRDPARTY"
 src_paths = ["doc", "src", "tests"]
 
 [tool.coverage.run]
 source = ["ansys.additive.core"]
-omit = ["*/parametric_study/display/*"] # TODO: Remove this once unit tests are added for these files
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.pytest.ini_options]
 minversion = "7.1"
 addopts = "-ra --cov=ansys.additive.core --cov-report html:.cov/html --cov-report xml:.cov/xml --cov-report term -vv --cov-fail-under 95"
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/__init__.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,38 +41,48 @@
     os.makedirs(USER_DATA_PATH)
 
 EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
 """Storage path for example data."""
 if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
     os.makedirs(EXAMPLES_PATH)
 
-from ansys.additive.core.additive import Additive
-from ansys.additive.core.exceptions import BetaFeatureNotEnabledError
-from ansys.additive.core.geometry_file import BuildFile, MachineType, StlFile
-from ansys.additive.core.logger import LOG
-from ansys.additive.core.machine import AdditiveMachine, MachineConstants
-from ansys.additive.core.material import (
+from ansys.additive.core.additive import Additive  # noqa: F401, E402
+from ansys.additive.core.exceptions import BetaFeatureNotEnabledError  # noqa: F401, E402
+from ansys.additive.core.geometry_file import BuildFile, MachineType, StlFile  # noqa: F401, E402
+from ansys.additive.core.logger import LOG  # noqa: F401, E402
+from ansys.additive.core.machine import AdditiveMachine, MachineConstants  # noqa: F401, E402
+from ansys.additive.core.material import (  # noqa: F401, E402
     AdditiveMaterial,
     CharacteristicWidthDataPoint,
     ThermalPropertiesDataPoint,
 )
-from ansys.additive.core.material_tuning import MaterialTuningInput, MaterialTuningSummary
-from ansys.additive.core.microstructure import (
+from ansys.additive.core.material_tuning import (  # noqa: F401, E402
+    MaterialTuningInput,
+    MaterialTuningSummary,
+)
+from ansys.additive.core.microstructure import (  # noqa: F401, E402
     CircleEquivalenceColumnNames,
     MicrostructureInput,
     MicrostructureSummary,
 )
-from ansys.additive.core.microstructure_3d import Microstructure3DInput, Microstructure3DSummary
-from ansys.additive.core.porosity import PorosityInput, PorositySummary
-from ansys.additive.core.simulation import SimulationError, SimulationStatus, SimulationType
-from ansys.additive.core.single_bead import (
+from ansys.additive.core.microstructure_3d import (  # noqa: F401, E402
+    Microstructure3DInput,
+    Microstructure3DSummary,
+)
+from ansys.additive.core.porosity import PorosityInput, PorositySummary  # noqa: F401, E402
+from ansys.additive.core.simulation import (  # noqa: F401, E402
+    SimulationError,
+    SimulationStatus,
+    SimulationType,
+)
+from ansys.additive.core.single_bead import (  # noqa: F401, E402
     MeltPool,
     MeltPoolColumnNames,
     SingleBeadInput,
     SingleBeadSummary,
 )
-from ansys.additive.core.thermal_history import (
+from ansys.additive.core.thermal_history import (  # noqa: F401, E402
     CoaxialAverageSensorInputs,
     Range,
     ThermalHistoryInput,
     ThermalHistorySummary,
 )
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/additive.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/additive.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/conversions.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/download.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/download.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/__init__.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/examples/downloads.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/exceptions.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/geometry_file.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/geometry_file.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/logger.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/machine.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/machine.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/material.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/material.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/material_tuning.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/material_tuning.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/microstructure.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/microstructure_3d.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/microstructure_3d.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/misc.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/__init__.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides data storage and utility methods for a parametric study."""
-from ansys.additive.core.parametric_study.constants import (
+from ansys.additive.core.parametric_study.constants import (  # noqa: F401
     DEFAULT_ITERATION,
     DEFAULT_PRIORITY,
     FORMAT_VERSION,
     ColumnNames,
 )
-from ansys.additive.core.parametric_study.parametric_runner import ParametricRunner
-from ansys.additive.core.parametric_study.parametric_study import ParametricStudy
-from ansys.additive.core.parametric_study.parametric_utils import build_rate, energy_density
+from ansys.additive.core.parametric_study.parametric_runner import ParametricRunner  # noqa: F401
+from ansys.additive.core.parametric_study.parametric_study import ParametricStudy  # noqa: F401
+from ansys.additive.core.parametric_study.parametric_utils import (  # noqa: F401
+    build_rate,
+    energy_density,
+)
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/constants.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/display/__init__.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Provides plots and interactive interfaces for parametric study results."""
+"""Constants used for server connections."""
 
-from .ave_grain_size_plot import ave_grain_size_plot
-from .porosity_contour_plot import porosity_contour_plot
-from .porosity_eval_plot import porosity_eval_plot
-from .show_table import show_table
-from .single_bead_eval_plot import single_bead_eval_plot
+from pathlib import Path
+
+LOCALHOST = "127.0.0.1"
+"""IP address for localhost."""
+PYPIM_PRODUCT_NAME = "additive"
+"""Product name for the Additive server in a PyPIM environment."""
+DEFAULT_PRODUCT_VERSION = "242"
+"""Default Ansys product version to use for the Additive server."""
+ADDITIVE_SERVER_EXE_NAME = "additiveserver"
+"""Name of the Additive server executable."""
+ADDITIVE_SERVER_SUBDIR = Path("Additive") / "additiveserver"
+"""Subdirectory for the Additive server in the Ansys installation directory."""
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_runner.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_runner.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_study.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_study.py`

 * *Files 1% similar despite different names*

```diff
@@ -4810,1015 +4810,1050 @@
 00012c90: 206b 6565 703d 2266 6972 7374 2229 2c0a   keep="first"),.
 00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012cb0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
 00012cc0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
 00012cd0: 2073 656c 662e 5f64 6174 615f 6672 616d   self._data_fram
 00012ce0: 6520 3d20 6475 706c 6963 6174 6573 5f72  e = duplicates_r
 00012cf0: 656d 6f76 6564 5f64 660a 2020 2020 2020  emoved_df.      
-00012d00: 2020 6e5f 7265 6d6f 7665 6420 3d20 6c65    n_removed = le
-00012d10: 6e28 6375 7272 656e 745f 6466 2920 2d20  n(current_df) - 
-00012d20: 6c65 6e28 6475 706c 6963 6174 6573 5f72  len(duplicates_r
-00012d30: 656d 6f76 6564 5f64 6629 0a20 2020 2020  emoved_df).     
-00012d40: 2020 204c 4f47 2e64 6562 7567 2866 2252     LOG.debug(f"R
-00012d50: 656d 6f76 6564 207b 6e5f 7265 6d6f 7665  emoved {n_remove
-00012d60: 647d 2064 7570 6c69 6361 7465 2073 696d  d} duplicate sim
-00012d70: 756c 6174 696f 6e28 7329 2e22 290a 2020  ulation(s).").  
-00012d80: 2020 2020 2020 7265 7475 726e 206e 5f72        return n_r
-00012d90: 656d 6f76 6564 0a0a 2020 2020 4073 6176  emoved..    @sav
-00012da0: 655f 6f6e 5f72 6574 7572 6e0a 2020 2020  e_on_return.    
-00012db0: 6465 6620 7265 6d6f 7665 2873 656c 662c  def remove(self,
-00012dc0: 2069 6473 3a20 7374 7220 7c20 6c69 7374   ids: str | list
-00012dd0: 5b73 7472 5d29 3a0a 2020 2020 2020 2020  [str]):.        
-00012de0: 2222 2252 656d 6f76 6520 7369 6d75 6c61  """Remove simula
-00012df0: 7469 6f6e 7320 6672 6f6d 2074 6865 2070  tions from the p
-00012e00: 6172 616d 6574 7269 6320 7374 7564 792e  arametric study.
-00012e10: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00012e20: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00012e30: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00012e40: 6964 7320 3a20 7374 722c 206c 6973 745b  ids : str, list[
-00012e50: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
-00012e60: 204f 6e65 206f 7220 6d6f 7265 2049 4420   One or more ID 
-00012e70: 7661 6c75 6573 2066 6f72 2074 6865 2073  values for the s
-00012e80: 696d 756c 6174 696f 6e73 2074 6f20 7265  imulations to re
-00012e90: 6d6f 7665 2e0a 2020 2020 2020 2020 2222  move..        ""
-00012ea0: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
-00012eb0: 6e73 7461 6e63 6528 6964 732c 2073 7472  nstance(ids, str
-00012ec0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00012ed0: 6473 203d 205b 6964 735d 0a20 2020 2020  ds = [ids].     
-00012ee0: 2020 2069 6478 203d 2073 656c 662e 5f64     idx = self._d
-00012ef0: 6174 615f 6672 616d 652e 696e 6465 785b  ata_frame.index[
-00012f00: 7365 6c66 2e5f 6461 7461 5f66 7261 6d65  self._data_frame
-00012f10: 5b43 6f6c 756d 6e4e 616d 6573 2e49 445d  [ColumnNames.ID]
-00012f20: 2e69 7369 6e28 6964 7329 5d2e 746f 6c69  .isin(ids)].toli
-00012f30: 7374 2829 0a20 2020 2020 2020 2073 656c  st().        sel
-00012f40: 662e 5f64 6174 615f 6672 616d 652e 6472  f._data_frame.dr
-00012f50: 6f70 2869 6e64 6578 3d69 6478 2c20 696e  op(index=idx, in
-00012f60: 706c 6163 653d 5472 7565 290a 0a20 2020  place=True)..   
-00012f70: 2040 7361 7665 5f6f 6e5f 7265 7475 726e   @save_on_return
-00012f80: 0a20 2020 2064 6566 2073 6574 5f73 7461  .    def set_sta
-00012f90: 7475 7328 7365 6c66 2c20 6964 733a 2073  tus(self, ids: s
-00012fa0: 7472 207c 206c 6973 745b 7374 725d 2c20  tr | list[str], 
-00012fb0: 7374 6174 7573 3a20 5369 6d75 6c61 7469  status: Simulati
-00012fc0: 6f6e 5374 6174 7573 293a 0a20 2020 2020  onStatus):.     
-00012fd0: 2020 2022 2222 5365 7420 7468 6520 7374     """Set the st
-00012fe0: 6174 7573 206f 6620 7369 6d75 6c61 7469  atus of simulati
-00012ff0: 6f6e 7320 696e 2074 6865 2070 6172 616d  ons in the param
-00013000: 6574 7269 6320 7374 7564 792e 0a0a 2020  etric study...  
-00013010: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00013020: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00013030: 2d2d 2d0a 2020 2020 2020 2020 6964 7320  ---.        ids 
-00013040: 3a20 7374 722c 206c 6973 745b 7374 725d  : str, list[str]
-00013050: 0a20 2020 2020 2020 2020 2020 204f 6e65  .            One
-00013060: 206f 7220 6d6f 7265 2049 4473 206f 6620   or more IDs of 
-00013070: 7468 6520 7369 6d75 6c61 7469 6f6e 7320  the simulations 
-00013080: 746f 2075 7064 6174 652e 0a0a 2020 2020  to update...    
-00013090: 2020 2020 7374 6174 7573 203a 2053 696d      status : Sim
-000130a0: 756c 6174 696f 6e53 7461 7475 730a 2020  ulationStatus.  
-000130b0: 2020 2020 2020 2020 2020 5374 6174 7573            Status
-000130c0: 2066 6f72 2074 6865 2073 696d 756c 6174   for the simulat
-000130d0: 696f 6e73 2e0a 2020 2020 2020 2020 2222  ions..        ""
-000130e0: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
-000130f0: 6e73 7461 6e63 6528 6964 732c 2073 7472  nstance(ids, str
-00013100: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00013110: 6473 203d 205b 6964 735d 0a20 2020 2020  ds = [ids].     
-00013120: 2020 2069 6478 203d 2073 656c 662e 5f64     idx = self._d
-00013130: 6174 615f 6672 616d 652e 696e 6465 785b  ata_frame.index[
-00013140: 7365 6c66 2e5f 6461 7461 5f66 7261 6d65  self._data_frame
-00013150: 5b43 6f6c 756d 6e4e 616d 6573 2e49 445d  [ColumnNames.ID]
-00013160: 2e69 7369 6e28 6964 7329 5d0a 2020 2020  .isin(ids)].    
-00013170: 2020 2020 7365 6c66 2e5f 6461 7461 5f66      self._data_f
-00013180: 7261 6d65 2e6c 6f63 5b69 6478 2c20 436f  rame.loc[idx, Co
-00013190: 6c75 6d6e 4e61 6d65 732e 5354 4154 5553  lumnNames.STATUS
-000131a0: 5d20 3d20 7374 6174 7573 0a0a 2020 2020  ] = status..    
-000131b0: 4073 6176 655f 6f6e 5f72 6574 7572 6e0a  @save_on_return.
-000131c0: 2020 2020 6465 6620 7365 745f 7072 696f      def set_prio
-000131d0: 7269 7479 2873 656c 662c 2069 6473 3a20  rity(self, ids: 
-000131e0: 7374 7220 7c20 6c69 7374 5b73 7472 5d2c  str | list[str],
-000131f0: 2070 7269 6f72 6974 793a 2069 6e74 293a   priority: int):
-00013200: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
-00013210: 7468 6520 7072 696f 7269 7479 206f 6620  the priority of 
-00013220: 7369 6d75 6c61 7469 6f6e 7320 696e 2074  simulations in t
-00013230: 6865 2070 6172 616d 6574 7269 6320 7374  he parametric st
-00013240: 7564 792e 0a0a 2020 2020 2020 2020 5061  udy...        Pa
-00013250: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00013260: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00013270: 2020 2020 6964 7320 3a20 7374 722c 206c      ids : str, l
-00013280: 6973 745b 7374 725d 0a20 2020 2020 2020  ist[str].       
-00013290: 2020 2020 204f 6e65 206f 7220 6d6f 7265       One or more
-000132a0: 2049 4473 206f 6620 7468 6520 7369 6d75   IDs of the simu
-000132b0: 6c61 7469 6f6e 7320 746f 2075 7064 6174  lations to updat
-000132c0: 652e 0a0a 2020 2020 2020 2020 7072 696f  e...        prio
-000132d0: 7269 7479 203a 2069 6e74 0a20 2020 2020  rity : int.     
-000132e0: 2020 2020 2020 2050 7269 6f72 6974 7920         Priority 
-000132f0: 666f 7220 7468 6520 7369 6d75 6c61 7469  for the simulati
-00013300: 6f6e 732e 0a20 2020 2020 2020 2022 2222  ons..        """
-00013310: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00013320: 7374 616e 6365 2869 6473 2c20 7374 7229  stance(ids, str)
-00013330: 3a0a 2020 2020 2020 2020 2020 2020 6964  :.            id
-00013340: 7320 3d20 5b69 6473 5d0a 2020 2020 2020  s = [ids].      
-00013350: 2020 6964 7820 3d20 7365 6c66 2e5f 6461    idx = self._da
-00013360: 7461 5f66 7261 6d65 2e69 6e64 6578 5b73  ta_frame.index[s
-00013370: 656c 662e 5f64 6174 615f 6672 616d 655b  elf._data_frame[
-00013380: 436f 6c75 6d6e 4e61 6d65 732e 4944 5d2e  ColumnNames.ID].
-00013390: 6973 696e 2869 6473 295d 0a20 2020 2020  isin(ids)].     
-000133a0: 2020 2073 656c 662e 5f64 6174 615f 6672     self._data_fr
-000133b0: 616d 652e 6c6f 635b 6964 782c 2043 6f6c  ame.loc[idx, Col
-000133c0: 756d 6e4e 616d 6573 2e50 5249 4f52 4954  umnNames.PRIORIT
-000133d0: 595d 203d 2070 7269 6f72 6974 790a 0a20  Y] = priority.. 
-000133e0: 2020 2040 7361 7665 5f6f 6e5f 7265 7475     @save_on_retu
-000133f0: 726e 0a20 2020 2064 6566 2073 6574 5f69  rn.    def set_i
-00013400: 7465 7261 7469 6f6e 2873 656c 662c 2069  teration(self, i
-00013410: 6473 3a20 7374 7220 7c20 6c69 7374 5b73  ds: str | list[s
-00013420: 7472 5d2c 2069 7465 7261 7469 6f6e 3a20  tr], iteration: 
-00013430: 696e 7429 3a0a 2020 2020 2020 2020 2222  int):.        ""
-00013440: 2253 6574 2074 6865 2069 7465 7261 7469  "Set the iterati
-00013450: 6f6e 206e 756d 6265 7220 6f66 2073 696d  on number of sim
-00013460: 756c 6174 696f 6e73 2069 6e20 7468 6520  ulations in the 
-00013470: 7061 7261 6d65 7472 6963 2073 7475 6479  parametric study
-00013480: 2e0a 0a20 2020 2020 2020 2054 6865 2069  ...        The i
-00013490: 7465 7261 7469 6f6e 206e 756d 6265 7220  teration number 
-000134a0: 6973 2075 7365 6420 746f 2074 7261 636b  is used to track
-000134b0: 2074 6865 2065 766f 6c75 7469 6f6e 206f   the evolution o
-000134c0: 6620 610a 2020 2020 2020 2020 6465 7369  f a.        desi
-000134d0: 676e 206f 6620 6578 7065 7269 6d65 6e74  gn of experiment
-000134e0: 732e 2049 7473 2075 7365 2069 7320 6f70  s. Its use is op
-000134f0: 7469 6f6e 616c 2e0a 0a20 2020 2020 2020  tional...       
-00013500: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00013510: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00013520: 2020 2020 2020 2069 6473 203a 2073 7472         ids : str
-00013530: 2c20 6c69 7374 5b73 7472 5d0a 2020 2020  , list[str].    
-00013540: 2020 2020 2020 2020 4f6e 6520 6f72 206d          One or m
-00013550: 6f72 6520 4944 7320 6f66 2074 6865 2073  ore IDs of the s
-00013560: 696d 756c 6174 696f 6e73 2074 6f20 7570  imulations to up
-00013570: 6461 7465 2e0a 0a20 2020 2020 2020 2069  date...        i
-00013580: 7465 7261 7469 6f6e 203a 2069 6e74 0a20  teration : int. 
-00013590: 2020 2020 2020 2020 2020 2049 7465 7261             Itera
-000135a0: 7469 6f6e 2066 6f72 2074 6865 2073 696d  tion for the sim
-000135b0: 756c 6174 696f 6e73 2e0a 2020 2020 2020  ulations..      
-000135c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000135d0: 2069 7369 6e73 7461 6e63 6528 6964 732c   isinstance(ids,
-000135e0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-000135f0: 2020 2069 6473 203d 205b 6964 735d 0a20     ids = [ids]. 
-00013600: 2020 2020 2020 2069 6478 203d 2073 656c         idx = sel
-00013610: 662e 5f64 6174 615f 6672 616d 652e 696e  f._data_frame.in
-00013620: 6465 785b 7365 6c66 2e5f 6461 7461 5f66  dex[self._data_f
-00013630: 7261 6d65 5b43 6f6c 756d 6e4e 616d 6573  rame[ColumnNames
-00013640: 2e49 445d 2e69 7369 6e28 6964 7329 5d0a  .ID].isin(ids)].
-00013650: 2020 2020 2020 2020 7365 6c66 2e5f 6461          self._da
-00013660: 7461 5f66 7261 6d65 2e6c 6f63 5b69 6478  ta_frame.loc[idx
-00013670: 2c20 436f 6c75 6d6e 4e61 6d65 732e 4954  , ColumnNames.IT
-00013680: 4552 4154 494f 4e5d 203d 2069 7465 7261  ERATION] = itera
-00013690: 7469 6f6e 0a0a 2020 2020 6465 6620 5f63  tion..    def _c
-000136a0: 7265 6174 655f 756e 6971 7565 5f69 6428  reate_unique_id(
-000136b0: 7365 6c66 2c20 7072 6566 6978 3a20 7374  self, prefix: st
-000136c0: 7220 7c20 4e6f 6e65 203d 204e 6f6e 652c  r | None = None,
-000136d0: 2069 643a 2073 7472 207c 204e 6f6e 6520   id: str | None 
-000136e0: 3d20 4e6f 6e65 2920 2d3e 2073 7472 3a0a  = None) -> str:.
-000136f0: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00013700: 6520 6120 756e 6971 7565 2073 696d 756c  e a unique simul
-00013710: 6174 696f 6e20 4944 2066 6f72 2061 2070  ation ID for a p
-00013720: 6572 6d75 7461 7469 6f6e 2e0a 0a20 2020  ermutation...   
-00013730: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00013740: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00013750: 2d2d 0a20 2020 2020 2020 2070 7265 6669  --.        prefi
-00013760: 7820 3a20 7374 722c 2064 6566 6175 6c74  x : str, default
-00013770: 3a20 4e6f 6e65 0a20 2020 2020 2020 2020  : None.         
-00013780: 2020 2050 7265 6669 7820 666f 7220 7468     Prefix for th
-00013790: 6520 4944 2e0a 2020 2020 2020 2020 6964  e ID..        id
+00012d00: 2020 7365 6c66 2e5f 6461 7461 5f66 7261    self._data_fra
+00012d10: 6d65 2e72 6573 6574 5f69 6e64 6578 2864  me.reset_index(d
+00012d20: 726f 703d 5472 7565 2c20 696e 706c 6163  rop=True, inplac
+00012d30: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+00012d40: 6e5f 7265 6d6f 7665 6420 3d20 6c65 6e28  n_removed = len(
+00012d50: 6375 7272 656e 745f 6466 2920 2d20 6c65  current_df) - le
+00012d60: 6e28 6475 706c 6963 6174 6573 5f72 656d  n(duplicates_rem
+00012d70: 6f76 6564 5f64 6629 0a20 2020 2020 2020  oved_df).       
+00012d80: 204c 4f47 2e64 6562 7567 2866 2252 656d   LOG.debug(f"Rem
+00012d90: 6f76 6564 207b 6e5f 7265 6d6f 7665 647d  oved {n_removed}
+00012da0: 2064 7570 6c69 6361 7465 2073 696d 756c   duplicate simul
+00012db0: 6174 696f 6e28 7329 2e22 290a 2020 2020  ation(s).").    
+00012dc0: 2020 2020 7265 7475 726e 206e 5f72 656d      return n_rem
+00012dd0: 6f76 6564 0a0a 2020 2020 4073 6176 655f  oved..    @save_
+00012de0: 6f6e 5f72 6574 7572 6e0a 2020 2020 6465  on_return.    de
+00012df0: 6620 7265 6d6f 7665 2873 656c 662c 2069  f remove(self, i
+00012e00: 6473 3a20 7374 7220 7c20 6c69 7374 5b73  ds: str | list[s
+00012e10: 7472 5d29 3a0a 2020 2020 2020 2020 2222  tr]):.        ""
+00012e20: 2252 656d 6f76 6520 7369 6d75 6c61 7469  "Remove simulati
+00012e30: 6f6e 7320 6672 6f6d 2074 6865 2070 6172  ons from the par
+00012e40: 616d 6574 7269 6320 7374 7564 792e 0a0a  ametric study...
+00012e50: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00012e60: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00012e70: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6964  -----.        id
+00012e80: 7320 3a20 7374 722c 206c 6973 745b 7374  s : str, list[st
+00012e90: 725d 0a20 2020 2020 2020 2020 2020 204f  r].            O
+00012ea0: 6e65 206f 7220 6d6f 7265 2049 4420 7661  ne or more ID va
+00012eb0: 6c75 6573 2066 6f72 2074 6865 2073 696d  lues for the sim
+00012ec0: 756c 6174 696f 6e73 2074 6f20 7265 6d6f  ulations to remo
+00012ed0: 7665 2e0a 2020 2020 2020 2020 2222 220a  ve..        """.
+00012ee0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00012ef0: 7461 6e63 6528 6964 732c 2073 7472 293a  tance(ids, str):
+00012f00: 0a20 2020 2020 2020 2020 2020 2069 6473  .            ids
+00012f10: 203d 205b 6964 735d 0a20 2020 2020 2020   = [ids].       
+00012f20: 2069 6478 203d 2073 656c 662e 5f64 6174   idx = self._dat
+00012f30: 615f 6672 616d 652e 696e 6465 785b 7365  a_frame.index[se
+00012f40: 6c66 2e5f 6461 7461 5f66 7261 6d65 5b43  lf._data_frame[C
+00012f50: 6f6c 756d 6e4e 616d 6573 2e49 445d 2e69  olumnNames.ID].i
+00012f60: 7369 6e28 6964 7329 5d2e 746f 6c69 7374  sin(ids)].tolist
+00012f70: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00012f80: 5f64 6174 615f 6672 616d 652e 6472 6f70  _data_frame.drop
+00012f90: 2869 6e64 6578 3d69 6478 2c20 696e 706c  (index=idx, inpl
+00012fa0: 6163 653d 5472 7565 290a 0a20 2020 2040  ace=True)..    @
+00012fb0: 7361 7665 5f6f 6e5f 7265 7475 726e 0a20  save_on_return. 
+00012fc0: 2020 2064 6566 2073 6574 5f73 7461 7475     def set_statu
+00012fd0: 7328 7365 6c66 2c20 6964 733a 2073 7472  s(self, ids: str
+00012fe0: 207c 206c 6973 745b 7374 725d 2c20 7374   | list[str], st
+00012ff0: 6174 7573 3a20 5369 6d75 6c61 7469 6f6e  atus: Simulation
+00013000: 5374 6174 7573 293a 0a20 2020 2020 2020  Status):.       
+00013010: 2022 2222 5365 7420 7468 6520 7374 6174   """Set the stat
+00013020: 7573 206f 6620 7369 6d75 6c61 7469 6f6e  us of simulation
+00013030: 7320 696e 2074 6865 2070 6172 616d 6574  s in the paramet
+00013040: 7269 6320 7374 7564 792e 0a0a 2020 2020  ric study...    
+00013050: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00013060: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00013070: 2d0a 2020 2020 2020 2020 6964 7320 3a20  -.        ids : 
+00013080: 7374 722c 206c 6973 745b 7374 725d 0a20  str, list[str]. 
+00013090: 2020 2020 2020 2020 2020 204f 6e65 206f             One o
+000130a0: 7220 6d6f 7265 2049 4473 206f 6620 7468  r more IDs of th
+000130b0: 6520 7369 6d75 6c61 7469 6f6e 7320 746f  e simulations to
+000130c0: 2075 7064 6174 652e 0a0a 2020 2020 2020   update...      
+000130d0: 2020 7374 6174 7573 203a 2053 696d 756c    status : Simul
+000130e0: 6174 696f 6e53 7461 7475 730a 2020 2020  ationStatus.    
+000130f0: 2020 2020 2020 2020 5374 6174 7573 2066          Status f
+00013100: 6f72 2074 6865 2073 696d 756c 6174 696f  or the simulatio
+00013110: 6e73 2e0a 2020 2020 2020 2020 2222 220a  ns..        """.
+00013120: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00013130: 7461 6e63 6528 6964 732c 2073 7472 293a  tance(ids, str):
+00013140: 0a20 2020 2020 2020 2020 2020 2069 6473  .            ids
+00013150: 203d 205b 6964 735d 0a20 2020 2020 2020   = [ids].       
+00013160: 2069 6478 203d 2073 656c 662e 5f64 6174   idx = self._dat
+00013170: 615f 6672 616d 652e 696e 6465 785b 7365  a_frame.index[se
+00013180: 6c66 2e5f 6461 7461 5f66 7261 6d65 5b43  lf._data_frame[C
+00013190: 6f6c 756d 6e4e 616d 6573 2e49 445d 2e69  olumnNames.ID].i
+000131a0: 7369 6e28 6964 7329 5d0a 2020 2020 2020  sin(ids)].      
+000131b0: 2020 7365 6c66 2e5f 6461 7461 5f66 7261    self._data_fra
+000131c0: 6d65 2e6c 6f63 5b69 6478 2c20 436f 6c75  me.loc[idx, Colu
+000131d0: 6d6e 4e61 6d65 732e 5354 4154 5553 5d20  mnNames.STATUS] 
+000131e0: 3d20 7374 6174 7573 0a0a 2020 2020 4073  = status..    @s
+000131f0: 6176 655f 6f6e 5f72 6574 7572 6e0a 2020  ave_on_return.  
+00013200: 2020 6465 6620 7365 745f 7072 696f 7269    def set_priori
+00013210: 7479 2873 656c 662c 2069 6473 3a20 7374  ty(self, ids: st
+00013220: 7220 7c20 6c69 7374 5b73 7472 5d2c 2070  r | list[str], p
+00013230: 7269 6f72 6974 793a 2069 6e74 293a 0a20  riority: int):. 
+00013240: 2020 2020 2020 2022 2222 5365 7420 7468         """Set th
+00013250: 6520 7072 696f 7269 7479 206f 6620 7369  e priority of si
+00013260: 6d75 6c61 7469 6f6e 7320 696e 2074 6865  mulations in the
+00013270: 2070 6172 616d 6574 7269 6320 7374 7564   parametric stud
+00013280: 792e 0a0a 2020 2020 2020 2020 5061 7261  y...        Para
+00013290: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+000132a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000132b0: 2020 6964 7320 3a20 7374 722c 206c 6973    ids : str, lis
+000132c0: 745b 7374 725d 0a20 2020 2020 2020 2020  t[str].         
+000132d0: 2020 204f 6e65 206f 7220 6d6f 7265 2049     One or more I
+000132e0: 4473 206f 6620 7468 6520 7369 6d75 6c61  Ds of the simula
+000132f0: 7469 6f6e 7320 746f 2075 7064 6174 652e  tions to update.
+00013300: 0a0a 2020 2020 2020 2020 7072 696f 7269  ..        priori
+00013310: 7479 203a 2069 6e74 0a20 2020 2020 2020  ty : int.       
+00013320: 2020 2020 2050 7269 6f72 6974 7920 666f       Priority fo
+00013330: 7220 7468 6520 7369 6d75 6c61 7469 6f6e  r the simulation
+00013340: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00013350: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00013360: 616e 6365 2869 6473 2c20 7374 7229 3a0a  ance(ids, str):.
+00013370: 2020 2020 2020 2020 2020 2020 6964 7320              ids 
+00013380: 3d20 5b69 6473 5d0a 2020 2020 2020 2020  = [ids].        
+00013390: 6964 7820 3d20 7365 6c66 2e5f 6461 7461  idx = self._data
+000133a0: 5f66 7261 6d65 2e69 6e64 6578 5b73 656c  _frame.index[sel
+000133b0: 662e 5f64 6174 615f 6672 616d 655b 436f  f._data_frame[Co
+000133c0: 6c75 6d6e 4e61 6d65 732e 4944 5d2e 6973  lumnNames.ID].is
+000133d0: 696e 2869 6473 295d 0a20 2020 2020 2020  in(ids)].       
+000133e0: 2073 656c 662e 5f64 6174 615f 6672 616d   self._data_fram
+000133f0: 652e 6c6f 635b 6964 782c 2043 6f6c 756d  e.loc[idx, Colum
+00013400: 6e4e 616d 6573 2e50 5249 4f52 4954 595d  nNames.PRIORITY]
+00013410: 203d 2070 7269 6f72 6974 790a 0a20 2020   = priority..   
+00013420: 2040 7361 7665 5f6f 6e5f 7265 7475 726e   @save_on_return
+00013430: 0a20 2020 2064 6566 2073 6574 5f69 7465  .    def set_ite
+00013440: 7261 7469 6f6e 2873 656c 662c 2069 6473  ration(self, ids
+00013450: 3a20 7374 7220 7c20 6c69 7374 5b73 7472  : str | list[str
+00013460: 5d2c 2069 7465 7261 7469 6f6e 3a20 696e  ], iteration: in
+00013470: 7429 3a0a 2020 2020 2020 2020 2222 2253  t):.        """S
+00013480: 6574 2074 6865 2069 7465 7261 7469 6f6e  et the iteration
+00013490: 206e 756d 6265 7220 6f66 2073 696d 756c   number of simul
+000134a0: 6174 696f 6e73 2069 6e20 7468 6520 7061  ations in the pa
+000134b0: 7261 6d65 7472 6963 2073 7475 6479 2e0a  rametric study..
+000134c0: 0a20 2020 2020 2020 2054 6865 2069 7465  .        The ite
+000134d0: 7261 7469 6f6e 206e 756d 6265 7220 6973  ration number is
+000134e0: 2075 7365 6420 746f 2074 7261 636b 2074   used to track t
+000134f0: 6865 2065 766f 6c75 7469 6f6e 206f 6620  he evolution of 
+00013500: 610a 2020 2020 2020 2020 6465 7369 676e  a.        design
+00013510: 206f 6620 6578 7065 7269 6d65 6e74 732e   of experiments.
+00013520: 2049 7473 2075 7365 2069 7320 6f70 7469   Its use is opti
+00013530: 6f6e 616c 2e0a 0a20 2020 2020 2020 2050  onal...        P
+00013540: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00013550: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00013560: 2020 2020 2069 6473 203a 2073 7472 2c20       ids : str, 
+00013570: 6c69 7374 5b73 7472 5d0a 2020 2020 2020  list[str].      
+00013580: 2020 2020 2020 4f6e 6520 6f72 206d 6f72        One or mor
+00013590: 6520 4944 7320 6f66 2074 6865 2073 696d  e IDs of the sim
+000135a0: 756c 6174 696f 6e73 2074 6f20 7570 6461  ulations to upda
+000135b0: 7465 2e0a 0a20 2020 2020 2020 2069 7465  te...        ite
+000135c0: 7261 7469 6f6e 203a 2069 6e74 0a20 2020  ration : int.   
+000135d0: 2020 2020 2020 2020 2049 7465 7261 7469           Iterati
+000135e0: 6f6e 2066 6f72 2074 6865 2073 696d 756c  on for the simul
+000135f0: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
+00013600: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+00013610: 7369 6e73 7461 6e63 6528 6964 732c 2073  sinstance(ids, s
+00013620: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00013630: 2069 6473 203d 205b 6964 735d 0a20 2020   ids = [ids].   
+00013640: 2020 2020 2069 6478 203d 2073 656c 662e       idx = self.
+00013650: 5f64 6174 615f 6672 616d 652e 696e 6465  _data_frame.inde
+00013660: 785b 7365 6c66 2e5f 6461 7461 5f66 7261  x[self._data_fra
+00013670: 6d65 5b43 6f6c 756d 6e4e 616d 6573 2e49  me[ColumnNames.I
+00013680: 445d 2e69 7369 6e28 6964 7329 5d0a 2020  D].isin(ids)].  
+00013690: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
+000136a0: 5f66 7261 6d65 2e6c 6f63 5b69 6478 2c20  _frame.loc[idx, 
+000136b0: 436f 6c75 6d6e 4e61 6d65 732e 4954 4552  ColumnNames.ITER
+000136c0: 4154 494f 4e5d 203d 2069 7465 7261 7469  ATION] = iterati
+000136d0: 6f6e 0a0a 2020 2020 6465 6620 5f63 7265  on..    def _cre
+000136e0: 6174 655f 756e 6971 7565 5f69 6428 7365  ate_unique_id(se
+000136f0: 6c66 2c20 7072 6566 6978 3a20 7374 7220  lf, prefix: str 
+00013700: 7c20 4e6f 6e65 203d 204e 6f6e 652c 2069  | None = None, i
+00013710: 643a 2073 7472 207c 204e 6f6e 6520 3d20  d: str | None = 
+00013720: 4e6f 6e65 2920 2d3e 2073 7472 3a0a 2020  None) -> str:.  
+00013730: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+00013740: 6120 756e 6971 7565 2073 696d 756c 6174  a unique simulat
+00013750: 696f 6e20 4944 2066 6f72 2061 2070 6572  ion ID for a per
+00013760: 6d75 7461 7469 6f6e 2e0a 0a20 2020 2020  mutation...     
+00013770: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00013780: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00013790: 0a20 2020 2020 2020 2070 7265 6669 7820  .        prefix 
 000137a0: 3a20 7374 722c 2064 6566 6175 6c74 3a20  : str, default: 
 000137b0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000137c0: 2049 4420 746f 2075 7365 2069 6620 6974   ID to use if it
-000137d0: 2069 7320 756e 6971 7565 2e20 6060 6964   is unique. ``id
-000137e0: 6060 2069 7320 7573 6564 2061 7320 7468  `` is used as th
-000137f0: 6520 7072 6566 6978 2069 660a 2020 2020  e prefix if.    
-00013800: 2020 2020 2020 2020 7468 6520 4944 2069          the ID i
-00013810: 7320 6e6f 7420 756e 6971 7565 2e0a 0a20  s not unique... 
-00013820: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00013830: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00013840: 2020 2020 2020 2073 7472 0a20 2020 2020         str.     
-00013850: 2020 2020 2020 2055 6e69 7175 6520 4944         Unique ID
-00013860: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00013870: 2020 2020 2020 2069 6620 6964 2069 7320         if id is 
-00013880: 6e6f 7420 4e6f 6e65 2061 6e64 206e 6f74  not None and not
-00013890: 2073 656c 662e 5f64 6174 615f 6672 616d   self._data_fram
-000138a0: 655b 436f 6c75 6d6e 4e61 6d65 732e 4944  e[ColumnNames.ID
-000138b0: 5d2e 7374 722e 6d61 7463 6828 6622 7b69  ].str.match(f"{i
-000138c0: 647d 2229 2e61 6e79 2829 3a0a 2020 2020  d}").any():.    
-000138d0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-000138e0: 640a 2020 2020 2020 2020 5f70 7265 6669  d.        _prefi
-000138f0: 7820 3d20 6964 206f 7220 7072 6566 6978  x = id or prefix
-00013900: 206f 7220 2273 696d 220a 2020 2020 2020   or "sim".      
-00013910: 2020 7569 6420 3d20 6622 7b5f 7072 6566    uid = f"{_pref
-00013920: 6978 7d5f 7b6d 6973 632e 7368 6f72 745f  ix}_{misc.short_
-00013930: 7575 6964 2829 7d22 0a20 2020 2020 2020  uuid()}".       
-00013940: 2077 6869 6c65 2073 656c 662e 5f64 6174   while self._dat
-00013950: 615f 6672 616d 655b 436f 6c75 6d6e 4e61  a_frame[ColumnNa
-00013960: 6d65 732e 4944 5d2e 7374 722e 6d61 7463  mes.ID].str.matc
-00013970: 6828 6622 7b75 6964 7d22 292e 616e 7928  h(f"{uid}").any(
-00013980: 293a 0a20 2020 2020 2020 2020 2020 2075  ):.            u
-00013990: 6964 203d 2066 227b 5f70 7265 6669 787d  id = f"{_prefix}
-000139a0: 5f7b 6d69 7363 2e73 686f 7274 5f75 7569  _{misc.short_uui
-000139b0: 6428 297d 220a 2020 2020 2020 2020 7265  d()}".        re
-000139c0: 7475 726e 2075 6964 0a0a 2020 2020 4073  turn uid..    @s
-000139d0: 6176 655f 6f6e 5f72 6574 7572 6e0a 2020  ave_on_return.  
-000139e0: 2020 6465 6620 636c 6561 7228 7365 6c66    def clear(self
-000139f0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00013a00: 6d6f 7665 2061 6c6c 2070 6572 6d75 7461  move all permuta
-00013a10: 7469 6f6e 7320 6672 6f6d 2074 6865 2070  tions from the p
-00013a20: 6172 616d 6574 7269 6320 7374 7564 792e  arametric study.
-00013a30: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00013a40: 2e5f 6461 7461 5f66 7261 6d65 203d 2073  ._data_frame = s
-00013a50: 656c 662e 5f64 6174 615f 6672 616d 655b  elf._data_frame[
-00013a60: 303a 305d 0a0a 2020 2020 4073 7461 7469  0:0]..    @stati
-00013a70: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-00013a80: 7570 6461 7465 5f66 6f72 6d61 7428 7374  update_format(st
-00013a90: 7564 793a 2050 6172 616d 6574 7269 6353  udy: ParametricS
-00013aa0: 7475 6479 2920 2d3e 2050 6172 616d 6574  tudy) -> Paramet
-00013ab0: 7269 6353 7475 6479 3a0a 2020 2020 2020  ricStudy:.      
-00013ac0: 2020 2222 2255 7064 6174 6520 6120 7061    """Update a pa
-00013ad0: 7261 6d65 7472 6963 2073 7475 6479 2074  rametric study t
-00013ae0: 6f20 7468 6520 6c61 7465 7374 2066 6f72  o the latest for
-00013af0: 6d61 7420 7665 7273 696f 6e2e 0a0a 2020  mat version...  
-00013b00: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00013b10: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00013b20: 2d2d 2d0a 2020 2020 2020 2020 7374 7564  ---.        stud
-00013b30: 7920 3a20 5061 7261 6d65 7472 6963 5374  y : ParametricSt
-00013b40: 7564 790a 2020 2020 2020 2020 2020 2020  udy.            
-00013b50: 5061 7261 6d65 7472 6963 2073 7475 6479  Parametric study
-00013b60: 2074 6f20 7570 6461 7465 2e0a 0a20 2020   to update...   
-00013b70: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00013b80: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00013b90: 2020 2020 2050 6172 616d 6574 7269 6353       ParametricS
-00013ba0: 7475 6479 0a20 2020 2020 2020 2020 2020  tudy.           
-00013bb0: 2055 7064 6174 6564 2070 6172 616d 6574   Updated paramet
-00013bc0: 7269 6320 7374 7564 792e 0a20 2020 2020  ric study..     
-00013bd0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00013be0: 2320 5468 6520 666f 726d 6174 5f76 6572  # The format_ver
-00013bf0: 7369 6f6e 2070 726f 7065 7274 7920 7761  sion property wa
-00013c00: 7320 696d 706c 656d 656e 7465 6420 696e  s implemented in
-00013c10: 636f 7272 6563 746c 7920 696e 2076 6572  correctly in ver
-00013c20: 7369 6f6e 2031 2e0a 2020 2020 2020 2020  sion 1..        
-00013c30: 2320 4368 6563 6b20 7468 6520 636f 6c75  # Check the colu
-00013c40: 6d6e 206e 616d 6573 2074 6f20 6465 7465  mn names to dete
-00013c50: 726d 696e 6520 6966 2074 6865 2073 7475  rmine if the stu
-00013c60: 6479 2069 7320 7665 7273 696f 6e20 312e  dy is version 1.
-00013c70: 0a20 2020 2020 2020 2069 6620 2248 6561  .        if "Hea
-00013c80: 7465 7220 5465 6d70 2028 c2b0 4329 2220  ter Temp (..C)" 
-00013c90: 696e 2073 7475 6479 2e64 6174 615f 6672  in study.data_fr
-00013ca0: 616d 6528 292e 636f 6c75 6d6e 733a 0a20  ame().columns:. 
-00013cb0: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-00013cc0: 6f6e 203d 2031 0a20 2020 2020 2020 2065  on = 1.        e
-00013cd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00013ce0: 2076 6572 7369 6f6e 203d 2073 7475 6479   version = study
-00013cf0: 2e66 6f72 6d61 745f 7665 7273 696f 6e0a  .format_version.
-00013d00: 0a20 2020 2020 2020 2069 6620 7665 7273  .        if vers
-00013d10: 696f 6e20 3e20 464f 524d 4154 5f56 4552  ion > FORMAT_VER
-00013d20: 5349 4f4e 3a0a 2020 2020 2020 2020 2020  SION:.          
-00013d30: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00013d40: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00013d50: 2020 2020 6622 556e 7375 7070 6f72 7465      f"Unsupporte
-00013d60: 6420 7665 7273 696f 6e2c 2073 7475 6479  d version, study
-00013d70: 2076 6572 7369 6f6e 203d 207b 7665 7273   version = {vers
-00013d80: 696f 6e7d 2c22 0a20 2020 2020 2020 2020  ion},".         
-00013d90: 2020 2020 2020 202b 2022 6c61 7465 7374         + "latest
-00013da0: 2073 7570 706f 7274 6564 2076 6572 7369   supported versi
-00013db0: 6f6e 2069 7320 7b46 4f52 4d41 545f 5645  on is {FORMAT_VE
-00013dc0: 5253 494f 4e7d 2e22 0a20 2020 2020 2020  RSION}.".       
-00013dd0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00013de0: 6966 2076 6572 7369 6f6e 203d 3d20 464f  if version == FO
-00013df0: 524d 4154 5f56 4552 5349 4f4e 3a0a 2020  RMAT_VERSION:.  
-00013e00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013e10: 2073 7475 6479 0a0a 2020 2020 2020 2020   study..        
-00013e20: 7072 696e 7428 2255 7064 6174 696e 6720  print("Updating 
-00013e30: 7061 7261 6d65 7472 6963 2073 7475 6479  parametric study
-00013e40: 2074 6f20 6c61 7465 7374 2076 6572 7369   to latest versi
-00013e50: 6f6e 2e22 290a 0a20 2020 2020 2020 2064  on.")..        d
-00013e60: 6620 3d20 7374 7564 792e 6461 7461 5f66  f = study.data_f
-00013e70: 7261 6d65 2829 0a20 2020 2020 2020 2069  rame().        i
-00013e80: 6620 7665 7273 696f 6e20 3c20 323a 0a20  f version < 2:. 
-00013e90: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00013ea0: 6466 2e72 656e 616d 6528 0a20 2020 2020  df.rename(.     
-00013eb0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00013ec0: 6e73 3d7b 0a20 2020 2020 2020 2020 2020  ns={.           
-00013ed0: 2020 2020 2020 2020 2022 4865 6174 6572           "Heater
-00013ee0: 2054 656d 7020 28c2 b043 2922 3a20 436f   Temp (..C)": Co
-00013ef0: 6c75 6d6e 4e61 6d65 732e 4845 4154 4552  lumnNames.HEATER
-00013f00: 5f54 454d 5045 5241 5455 5245 2c0a 2020  _TEMPERATURE,.  
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 2020 2253 7461 7274 2041 6e67 6c65 2028    "Start Angle (
-00013f30: c2b0 2922 3a20 436f 6c75 6d6e 4e61 6d65  ..)": ColumnName
-00013f40: 732e 5354 4152 545f 414e 474c 452c 0a20  s.START_ANGLE,. 
+000137c0: 2050 7265 6669 7820 666f 7220 7468 6520   Prefix for the 
+000137d0: 4944 2e0a 2020 2020 2020 2020 6964 3a20  ID..        id: 
+000137e0: 7374 722c 2064 6566 6175 6c74 3a20 4e6f  str, default: No
+000137f0: 6e65 0a20 2020 2020 2020 2020 2020 2049  ne.            I
+00013800: 4420 746f 2075 7365 2069 6620 6974 2069  D to use if it i
+00013810: 7320 756e 6971 7565 2e20 6060 6964 6060  s unique. ``id``
+00013820: 2069 7320 7573 6564 2061 7320 7468 6520   is used as the 
+00013830: 7072 6566 6978 2069 660a 2020 2020 2020  prefix if.      
+00013840: 2020 2020 2020 7468 6520 4944 2069 7320        the ID is 
+00013850: 6e6f 7420 756e 6971 7565 2e0a 0a20 2020  not unique...   
+00013860: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00013870: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00013880: 2020 2020 2073 7472 0a20 2020 2020 2020       str.       
+00013890: 2020 2020 2055 6e69 7175 6520 4944 2e0a       Unique ID..
+000138a0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+000138b0: 2020 2020 2069 6620 6964 2069 7320 6e6f       if id is no
+000138c0: 7420 4e6f 6e65 2061 6e64 206e 6f74 2073  t None and not s
+000138d0: 656c 662e 5f64 6174 615f 6672 616d 655b  elf._data_frame[
+000138e0: 436f 6c75 6d6e 4e61 6d65 732e 4944 5d2e  ColumnNames.ID].
+000138f0: 7374 722e 6d61 7463 6828 6622 7b69 647d  str.match(f"{id}
+00013900: 2229 2e61 6e79 2829 3a0a 2020 2020 2020  ").any():.      
+00013910: 2020 2020 2020 7265 7475 726e 2069 640a        return id.
+00013920: 2020 2020 2020 2020 5f70 7265 6669 7820          _prefix 
+00013930: 3d20 6964 206f 7220 7072 6566 6978 206f  = id or prefix o
+00013940: 7220 2273 696d 220a 2020 2020 2020 2020  r "sim".        
+00013950: 7569 6420 3d20 6622 7b5f 7072 6566 6978  uid = f"{_prefix
+00013960: 7d5f 7b6d 6973 632e 7368 6f72 745f 7575  }_{misc.short_uu
+00013970: 6964 2829 7d22 0a20 2020 2020 2020 2077  id()}".        w
+00013980: 6869 6c65 2073 656c 662e 5f64 6174 615f  hile self._data_
+00013990: 6672 616d 655b 436f 6c75 6d6e 4e61 6d65  frame[ColumnName
+000139a0: 732e 4944 5d2e 7374 722e 6d61 7463 6828  s.ID].str.match(
+000139b0: 6622 7b75 6964 7d22 292e 616e 7928 293a  f"{uid}").any():
+000139c0: 0a20 2020 2020 2020 2020 2020 2075 6964  .            uid
+000139d0: 203d 2066 227b 5f70 7265 6669 787d 5f7b   = f"{_prefix}_{
+000139e0: 6d69 7363 2e73 686f 7274 5f75 7569 6428  misc.short_uuid(
+000139f0: 297d 220a 2020 2020 2020 2020 7265 7475  )}".        retu
+00013a00: 726e 2075 6964 0a0a 2020 2020 4073 6176  rn uid..    @sav
+00013a10: 655f 6f6e 5f72 6574 7572 6e0a 2020 2020  e_on_return.    
+00013a20: 6465 6620 636c 6561 7228 7365 6c66 293a  def clear(self):
+00013a30: 0a20 2020 2020 2020 2022 2222 5265 6d6f  .        """Remo
+00013a40: 7665 2061 6c6c 2070 6572 6d75 7461 7469  ve all permutati
+00013a50: 6f6e 7320 6672 6f6d 2074 6865 2070 6172  ons from the par
+00013a60: 616d 6574 7269 6320 7374 7564 792e 2222  ametric study.""
+00013a70: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+00013a80: 6461 7461 5f66 7261 6d65 203d 2073 656c  data_frame = sel
+00013a90: 662e 5f64 6174 615f 6672 616d 655b 303a  f._data_frame[0:
+00013aa0: 305d 0a0a 2020 2020 4073 7461 7469 636d  0]..    @staticm
+00013ab0: 6574 686f 640a 2020 2020 6465 6620 7570  ethod.    def up
+00013ac0: 6461 7465 5f66 6f72 6d61 7428 7374 7564  date_format(stud
+00013ad0: 793a 2050 6172 616d 6574 7269 6353 7475  y: ParametricStu
+00013ae0: 6479 2920 2d3e 2050 6172 616d 6574 7269  dy) -> Parametri
+00013af0: 6353 7475 6479 3a0a 2020 2020 2020 2020  cStudy:.        
+00013b00: 2222 2255 7064 6174 6520 6120 7061 7261  """Update a para
+00013b10: 6d65 7472 6963 2073 7475 6479 2074 6f20  metric study to 
+00013b20: 7468 6520 6c61 7465 7374 2066 6f72 6d61  the latest forma
+00013b30: 7420 7665 7273 696f 6e2e 0a0a 2020 2020  t version...    
+00013b40: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00013b50: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00013b60: 2d0a 2020 2020 2020 2020 7374 7564 7920  -.        study 
+00013b70: 3a20 5061 7261 6d65 7472 6963 5374 7564  : ParametricStud
+00013b80: 790a 2020 2020 2020 2020 2020 2020 5061  y.            Pa
+00013b90: 7261 6d65 7472 6963 2073 7475 6479 2074  rametric study t
+00013ba0: 6f20 7570 6461 7465 2e0a 0a20 2020 2020  o update...     
+00013bb0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00013bc0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00013bd0: 2020 2050 6172 616d 6574 7269 6353 7475     ParametricStu
+00013be0: 6479 0a20 2020 2020 2020 2020 2020 2055  dy.            U
+00013bf0: 7064 6174 6564 2070 6172 616d 6574 7269  pdated parametri
+00013c00: 6320 7374 7564 792e 0a20 2020 2020 2020  c study..       
+00013c10: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
+00013c20: 5468 6520 666f 726d 6174 5f76 6572 7369  The format_versi
+00013c30: 6f6e 2070 726f 7065 7274 7920 7761 7320  on property was 
+00013c40: 696d 706c 656d 656e 7465 6420 696e 636f  implemented inco
+00013c50: 7272 6563 746c 7920 696e 2076 6572 7369  rrectly in versi
+00013c60: 6f6e 2031 2e0a 2020 2020 2020 2020 2320  on 1..        # 
+00013c70: 4368 6563 6b20 7468 6520 636f 6c75 6d6e  Check the column
+00013c80: 206e 616d 6573 2074 6f20 6465 7465 726d   names to determ
+00013c90: 696e 6520 6966 2074 6865 2073 7475 6479  ine if the study
+00013ca0: 2069 7320 7665 7273 696f 6e20 312e 0a20   is version 1.. 
+00013cb0: 2020 2020 2020 2069 6620 2248 6561 7465         if "Heate
+00013cc0: 7220 5465 6d70 2028 c2b0 4329 2220 696e  r Temp (..C)" in
+00013cd0: 2073 7475 6479 2e64 6174 615f 6672 616d   study.data_fram
+00013ce0: 6528 292e 636f 6c75 6d6e 733a 0a20 2020  e().columns:.   
+00013cf0: 2020 2020 2020 2020 2076 6572 7369 6f6e           version
+00013d00: 203d 2031 0a20 2020 2020 2020 2065 6c73   = 1.        els
+00013d10: 653a 0a20 2020 2020 2020 2020 2020 2076  e:.            v
+00013d20: 6572 7369 6f6e 203d 2073 7475 6479 2e66  ersion = study.f
+00013d30: 6f72 6d61 745f 7665 7273 696f 6e0a 0a20  ormat_version.. 
+00013d40: 2020 2020 2020 2069 6620 7665 7273 696f         if versio
+00013d50: 6e20 3e20 464f 524d 4154 5f56 4552 5349  n > FORMAT_VERSI
+00013d60: 4f4e 3a0a 2020 2020 2020 2020 2020 2020  ON:.            
+00013d70: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00013d80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013d90: 2020 6622 556e 7375 7070 6f72 7465 6420    f"Unsupported 
+00013da0: 7665 7273 696f 6e2c 2073 7475 6479 2076  version, study v
+00013db0: 6572 7369 6f6e 203d 207b 7665 7273 696f  ersion = {versio
+00013dc0: 6e7d 2c22 0a20 2020 2020 2020 2020 2020  n},".           
+00013dd0: 2020 2020 202b 2022 6c61 7465 7374 2073       + "latest s
+00013de0: 7570 706f 7274 6564 2076 6572 7369 6f6e  upported version
+00013df0: 2069 7320 7b46 4f52 4d41 545f 5645 5253   is {FORMAT_VERS
+00013e00: 494f 4e7d 2e22 0a20 2020 2020 2020 2020  ION}.".         
+00013e10: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00013e20: 2076 6572 7369 6f6e 203d 3d20 464f 524d   version == FORM
+00013e30: 4154 5f56 4552 5349 4f4e 3a0a 2020 2020  AT_VERSION:.    
+00013e40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00013e50: 7475 6479 0a0a 2020 2020 2020 2020 7072  tudy..        pr
+00013e60: 696e 7428 2255 7064 6174 696e 6720 7061  int("Updating pa
+00013e70: 7261 6d65 7472 6963 2073 7475 6479 2074  rametric study t
+00013e80: 6f20 6c61 7465 7374 2076 6572 7369 6f6e  o latest version
+00013e90: 2e22 290a 0a20 2020 2020 2020 2064 6620  .")..        df 
+00013ea0: 3d20 7374 7564 792e 6461 7461 5f66 7261  = study.data_fra
+00013eb0: 6d65 2829 0a20 2020 2020 2020 2069 6620  me().        if 
+00013ec0: 7665 7273 696f 6e20 3c20 323a 0a20 2020  version < 2:.   
+00013ed0: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+00013ee0: 2e72 656e 616d 6528 0a20 2020 2020 2020  .rename(.       
+00013ef0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00013f00: 3d7b 0a20 2020 2020 2020 2020 2020 2020  ={.             
+00013f10: 2020 2020 2020 2022 4865 6174 6572 2054         "Heater T
+00013f20: 656d 7020 28c2 b043 2922 3a20 436f 6c75  emp (..C)": Colu
+00013f30: 6d6e 4e61 6d65 732e 4845 4154 4552 5f54  mnNames.HEATER_T
+00013f40: 454d 5045 5241 5455 5245 2c0a 2020 2020  EMPERATURE,.    
 00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f60: 2020 2022 526f 7461 7469 6f6e 2041 6e67     "Rotation Ang
-00013f70: 6c65 2028 c2b0 2922 3a20 436f 6c75 6d6e  le (..)": Column
-00013f80: 4e61 6d65 732e 524f 5441 5449 4f4e 5f41  Names.ROTATION_A
-00013f90: 4e47 4c45 2c0a 2020 2020 2020 2020 2020  NGLE,.          
-00013fa0: 2020 2020 2020 2020 2020 2243 6f6f 6c69            "Cooli
-00013fb0: 6e67 2052 6174 6520 28c2 b04b 2f73 2922  ng Rate (..K/s)"
-00013fc0: 3a20 436f 6c75 6d6e 4e61 6d65 732e 434f  : ColumnNames.CO
-00013fd0: 4f4c 494e 475f 5241 5445 2c0a 2020 2020  OLING_RATE,.    
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 2254 6865 726d 616c 2047 7261 6469 656e  "Thermal Gradien
-00014000: 7420 28c2 b04b 2f6d 2922 3a20 436f 6c75  t (..K/m)": Colu
-00014010: 6d6e 4e61 6d65 732e 5448 4552 4d41 4c5f  mnNames.THERMAL_
-00014020: 4752 4144 4945 4e54 2c0a 2020 2020 2020  GRADIENT,.      
-00014030: 2020 2020 2020 2020 2020 2020 2020 2258                "X
-00014040: 5920 4176 6572 6167 6520 4772 6169 6e20  Y Average Grain 
-00014050: 5369 7a65 2028 c2b5 6d29 223a 2043 6f6c  Size (..m)": Col
-00014060: 756d 6e4e 616d 6573 2e58 595f 4156 4552  umnNames.XY_AVER
-00014070: 4147 455f 4752 4149 4e5f 5349 5a45 2c0a  AGE_GRAIN_SIZE,.
-00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2020 2258 5a20 4176 6572 6167 6520      "XZ Average 
-000140a0: 4772 6169 6e20 5369 7a65 2028 c2b5 6d29  Grain Size (..m)
-000140b0: 223a 2043 6f6c 756d 6e4e 616d 6573 2e58  ": ColumnNames.X
-000140c0: 5a5f 4156 4552 4147 455f 4752 4149 4e5f  Z_AVERAGE_GRAIN_
-000140d0: 5349 5a45 2c0a 2020 2020 2020 2020 2020  SIZE,.          
-000140e0: 2020 2020 2020 2020 2020 2259 5a20 4176            "YZ Av
-000140f0: 6572 6167 6520 4772 6169 6e20 5369 7a65  erage Grain Size
-00014100: 2028 c2b5 6d29 223a 2043 6f6c 756d 6e4e   (..m)": ColumnN
-00014110: 616d 6573 2e59 5a5f 4156 4552 4147 455f  ames.YZ_AVERAGE_
-00014120: 4752 4149 4e5f 5349 5a45 2c0a 2020 2020  GRAIN_SIZE,.    
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 224d 656c 7420 506f 6f6c 204c 656e 6774  "Melt Pool Lengt
-00014150: 682f 5769 6474 6820 286d 2922 3a20 436f  h/Width (m)": Co
-00014160: 6c75 6d6e 4e61 6d65 732e 4d45 4c54 5f50  lumnNames.MELT_P
-00014170: 4f4f 4c5f 4c45 4e47 5448 5f4f 5645 525f  OOL_LENGTH_OVER_
-00014180: 5749 4454 482c 0a20 2020 2020 2020 2020  WIDTH,.         
-00014190: 2020 2020 2020 2020 2020 2022 4d65 6c74             "Melt
-000141a0: 2050 6f6f 6c20 5265 6620 4465 7074 682f   Pool Ref Depth/
-000141b0: 5769 6474 6820 286d 2922 3a20 436f 6c75  Width (m)": Colu
-000141c0: 6d6e 4e61 6d65 732e 4d45 4c54 5f50 4f4f  mnNames.MELT_POO
-000141d0: 4c5f 5245 4645 5245 4e43 455f 4445 5054  L_REFERENCE_DEPT
-000141e0: 485f 4f56 4552 5f57 4944 5448 2c0a 2020  H_OVER_WIDTH,.  
-000141f0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00014200: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00014210: 2020 2020 2020 2020 2020 7665 7273 696f            versio
-00014220: 6e20 3d20 320a 0a20 2020 2020 2020 206e  n = 2..        n
-00014230: 6577 5f73 7475 6479 203d 2050 6172 616d  ew_study = Param
-00014240: 6574 7269 6353 7475 6479 2e5f 6e65 7728  etricStudy._new(
-00014250: 7374 7564 792e 6669 6c65 5f6e 616d 6529  study.file_name)
-00014260: 0a20 2020 2020 2020 206e 6577 5f73 7475  .        new_stu
-00014270: 6479 2e5f 6461 7461 5f66 7261 6d65 203d  dy._data_frame =
-00014280: 2064 660a 2020 2020 2020 2020 7265 7475   df.        retu
-00014290: 726e 206e 6577 5f73 7475 6479 0a0a 2020  rn new_study..  
-000142a0: 2020 4073 6176 655f 6f6e 5f72 6574 7572    @save_on_retur
-000142b0: 6e0a 2020 2020 6465 6620 6164 645f 7369  n.    def add_si
-000142c0: 6d75 6c61 7469 6f6e 735f 6672 6f6d 5f64  mulations_from_d
-000142d0: 6174 615f 6672 616d 6528 7365 6c66 2c20  ata_frame(self, 
-000142e0: 6466 3a20 7064 2e44 6174 6146 7261 6d65  df: pd.DataFrame
-000142f0: 2920 2d3e 206c 6973 745b 7374 725d 3a0a  ) -> list[str]:.
-00014300: 2020 2020 2020 2020 2222 2241 6464 2073          """Add s
-00014310: 696d 756c 6174 696f 6e73 2066 726f 6d20  imulations from 
-00014320: 616e 2069 6d70 6f72 7465 6420 4353 5620  an imported CSV 
-00014330: 6669 6c65 2074 6f20 7468 6520 7061 7261  file to the para
-00014340: 6d65 7472 6963 2073 7475 6479 2e0a 0a20  metric study... 
-00014350: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00014360: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00014370: 2d2d 2d2d 0a20 2020 2020 2020 2064 6620  ----.        df 
-00014380: 3a20 7064 2e44 6174 6146 7261 6d65 0a20  : pd.DataFrame. 
-00014390: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
-000143a0: 6672 616d 6520 6f66 2074 6865 2063 7376  frame of the csv
-000143b0: 2066 696c 6520 636f 6e74 6169 6e69 6e67   file containing
-000143c0: 2073 696d 756c 6174 696f 6e73 2074 6f20   simulations to 
-000143d0: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-000143e0: 7061 7261 6d65 7472 6963 2073 7475 6479  parametric study
-000143f0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00014400: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00014410: 2d2d 0a20 2020 2020 2020 206c 6973 745b  --.        list[
-00014420: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
-00014430: 204c 6973 7420 6f66 2065 7272 6f72 206d   List of error m
-00014440: 6573 7361 6765 7320 666f 7220 696e 7661  essages for inva
-00014450: 6c69 6420 7369 6d75 6c61 7469 6f6e 732e  lid simulations.
-00014460: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00014470: 2020 2020 2020 2320 6368 6563 6b20 7661        # check va
-00014480: 6c69 6420 696e 7075 7473 0a20 2020 2020  lid inputs.     
-00014490: 2020 2064 726f 705f 696e 6469 6365 732c     drop_indices,
-000144a0: 2065 7272 6f72 5f6c 6973 7420 3d20 6c69   error_list = li
-000144b0: 7374 2829 2c20 6c69 7374 2829 0a20 2020  st(), list().   
-000144c0: 2020 2020 2064 7570 6c69 6361 7465 7320       duplicates 
-000144d0: 3d20 300a 2020 2020 2020 2020 616c 6c6f  = 0.        allo
-000144e0: 7765 645f 7374 6174 7573 203d 205b 0a20  wed_status = [. 
-000144f0: 2020 2020 2020 2020 2020 2053 696d 756c             Simul
-00014500: 6174 696f 6e53 7461 7475 732e 434f 4d50  ationStatus.COMP
-00014510: 4c45 5445 442c 0a20 2020 2020 2020 2020  LETED,.         
-00014520: 2020 2053 696d 756c 6174 696f 6e53 7461     SimulationSta
-00014530: 7475 732e 5045 4e44 494e 472c 0a20 2020  tus.PENDING,.   
-00014540: 2020 2020 2020 2020 2053 696d 756c 6174           Simulat
-00014550: 696f 6e53 7461 7475 732e 534b 4950 2c0a  ionStatus.SKIP,.
-00014560: 2020 2020 2020 2020 2020 2020 5369 6d75              Simu
-00014570: 6c61 7469 6f6e 5374 6174 7573 2e45 5252  lationStatus.ERR
-00014580: 4f52 2c0a 2020 2020 2020 2020 5d0a 2020  OR,.        ].  
-00014590: 2020 2020 2020 666f 7220 696e 6465 782c        for index,
-000145a0: 2072 6f77 2069 6e20 6466 2e69 7465 7272   row in df.iterr
-000145b0: 6f77 7328 293a 0a20 2020 2020 2020 2020  ows():.         
-000145c0: 2020 2076 616c 6964 203d 2046 616c 7365     valid = False
-000145d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000145e0: 726f 775b 436f 6c75 6d6e 4e61 6d65 732e  row[ColumnNames.
-000145f0: 5354 4154 5553 5d20 696e 2061 6c6c 6f77  STATUS] in allow
-00014600: 6564 5f73 7461 7475 733a 0a20 2020 2020  ed_status:.     
-00014610: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-00014620: 2c20 6572 726f 7220 3d20 7365 6c66 2e5f  , error = self._
-00014630: 7661 6c69 6461 7465 5f69 6e70 7574 2872  validate_input(r
-00014640: 6f77 290a 2020 2020 2020 2020 2020 2020  ow).            
-00014650: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014660: 2020 2020 2020 7661 6c69 642c 2065 7272        valid, err
-00014670: 6f72 203d 2028 4661 6c73 652c 2066 2249  or = (False, f"I
-00014680: 6e76 616c 6964 2073 696d 756c 6174 696f  nvalid simulatio
-00014690: 6e20 7374 6174 7573 207b 726f 775b 436f  n status {row[Co
-000146a0: 6c75 6d6e 4e61 6d65 732e 5354 4154 5553  lumnNames.STATUS
-000146b0: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-000146c0: 2069 6620 6e6f 7420 7661 6c69 643a 0a20   if not valid:. 
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000146e0: 726f 705f 696e 6469 6365 732e 6170 7065  rop_indices.appe
-000146f0: 6e64 2869 6e64 6578 290a 2020 2020 2020  nd(index).      
-00014700: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00014710: 6c69 7374 2e61 7070 656e 6428 6572 726f  list.append(erro
-00014720: 7229 0a0a 2020 2020 2020 2020 2320 6472  r)..        # dr
-00014730: 6f70 2069 6e76 616c 6964 2069 6e70 7574  op invalid input
-00014740: 730a 2020 2020 2020 2020 6466 203d 2064  s.        df = d
-00014750: 662e 6472 6f70 2864 726f 705f 696e 6469  f.drop(drop_indi
-00014760: 6365 7329 0a0a 2020 2020 2020 2020 2320  ces)..        # 
-00014770: 6164 6420 7369 6d75 6c61 7469 6f6e 7320  add simulations 
-00014780: 746f 2074 6865 2070 6172 616d 6574 7269  to the parametri
-00014790: 6320 7374 7564 7920 616e 6420 6472 6f70  c study and drop
-000147a0: 2064 7570 6c69 6361 7465 730a 2020 2020   duplicates.    
-000147b0: 2020 2020 666f 7220 7374 6174 7573 2c20      for status, 
-000147c0: 6f76 6572 7772 6974 6520 696e 205b 0a20  overwrite in [. 
-000147d0: 2020 2020 2020 2020 2020 2028 5369 6d75             (Simu
-000147e0: 6c61 7469 6f6e 5374 6174 7573 2e43 4f4d  lationStatus.COM
-000147f0: 504c 4554 4544 2c20 5472 7565 292c 0a20  PLETED, True),. 
-00014800: 2020 2020 2020 2020 2020 2028 5369 6d75             (Simu
-00014810: 6c61 7469 6f6e 5374 6174 7573 2e50 454e  lationStatus.PEN
-00014820: 4449 4e47 2c20 4661 6c73 6529 2c0a 2020  DING, False),.  
-00014830: 2020 2020 2020 2020 2020 2853 696d 756c            (Simul
-00014840: 6174 696f 6e53 7461 7475 732e 534b 4950  ationStatus.SKIP
-00014850: 2c20 4661 6c73 6529 2c0a 2020 2020 2020  , False),.      
-00014860: 2020 2020 2020 2853 696d 756c 6174 696f        (Simulatio
-00014870: 6e53 7461 7475 732e 4552 524f 522c 2046  nStatus.ERROR, F
-00014880: 616c 7365 292c 0a20 2020 2020 2020 205d  alse),.        ]
-00014890: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000148a0: 206c 656e 2864 665b 6466 5b43 6f6c 756d   len(df[df[Colum
-000148b0: 6e4e 616d 6573 2e53 5441 5455 535d 203d  nNames.STATUS] =
-000148c0: 3d20 7374 6174 7573 5d29 203e 2030 3a0a  = status]) > 0:.
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 7365 6c66 2e5f 6461 7461 5f66 7261 6d65  self._data_frame
-000148f0: 203d 2070 642e 636f 6e63 6174 280a 2020   = pd.concat(.  
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 5b73 656c 662e 5f64 6174 615f 6672    [self._data_fr
-00014920: 616d 652c 2064 665b 6466 5b43 6f6c 756d  ame, df[df[Colum
-00014930: 6e4e 616d 6573 2e53 5441 5455 535d 203d  nNames.STATUS] =
-00014940: 3d20 7374 6174 7573 5d5d 2c0a 2020 2020  = status]],.    
-00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014960: 6967 6e6f 7265 5f69 6e64 6578 3d54 7275  ignore_index=Tru
-00014970: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00014980: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00014990: 2020 2020 2064 7570 6c69 6361 7465 7320       duplicates 
-000149a0: 2b3d 2073 656c 662e 5f72 656d 6f76 655f  += self._remove_
-000149b0: 6475 706c 6963 6174 655f 656e 7472 6965  duplicate_entrie
-000149c0: 7328 6f76 6572 7772 6974 653d 6f76 6572  s(overwrite=over
-000149d0: 7772 6974 6529 0a0a 2020 2020 2020 2020  write)..        
-000149e0: 6966 2064 7570 6c69 6361 7465 7320 3e20  if duplicates > 
-000149f0: 303a 0a20 2020 2020 2020 2020 2020 2065  0:.            e
-00014a00: 7272 6f72 5f6c 6973 742e 6170 7065 6e64  rror_list.append
-00014a10: 2866 2252 656d 6f76 6564 207b 6475 706c  (f"Removed {dupl
-00014a20: 6963 6174 6573 7d20 6475 706c 6963 6174  icates} duplicat
-00014a30: 6520 7369 6d75 6c61 7469 6f6e 2873 292e  e simulation(s).
-00014a40: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00014a50: 6e20 6572 726f 725f 6c69 7374 0a0a 2020  n error_list..  
-00014a60: 2020 6465 6620 5f76 616c 6964 6174 655f    def _validate_
-00014a70: 696e 7075 7428 7365 6c66 2c20 696e 7075  input(self, inpu
-00014a80: 743a 2070 642e 5365 7269 6573 293a 0a20  t: pd.Series):. 
-00014a90: 2020 2020 2020 2022 2222 5465 7374 2069         """Test i
-00014aa0: 6e70 7574 2066 726f 6d20 6120 726f 7720  nput from a row 
-00014ab0: 6f66 2061 2043 5356 2066 696c 6520 666f  of a CSV file fo
-00014ac0: 7220 7661 6c69 6420 696e 7075 7420 7061  r valid input pa
-00014ad0: 7261 6d65 7465 7273 2e0a 0a20 2020 2020  rameters...     
-00014ae0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00014af0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00014b00: 0a20 2020 2020 2020 2069 6e70 7574 203a  .        input :
-00014b10: 2070 642e 5365 7269 6573 0a20 2020 2020   pd.Series.     
-00014b20: 2020 2020 2020 2052 6f77 206f 6620 6120         Row of a 
-00014b30: 4353 5620 6669 6c65 2063 6f6e 7461 696e  CSV file contain
-00014b40: 696e 6720 7468 6520 7369 6d75 6c61 7469  ing the simulati
-00014b50: 6f6e 2069 6e70 7574 2e0a 0a20 2020 2020  on input...     
-00014b60: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00014b70: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00014b80: 2020 2074 7570 6c65 5b62 6f6f 6c2c 2073     tuple[bool, s
-00014b90: 7472 5d0a 2020 2020 2020 2020 2020 2020  tr].            
-00014ba0: 626f 6f6c 2c20 5472 7565 2069 6620 7468  bool, True if th
-00014bb0: 6520 696e 7075 7420 6973 2076 616c 6964  e input is valid
-00014bc0: 2c20 4661 6c73 6520 6f74 6865 7277 6973  , False otherwis
-00014bd0: 652e 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00014be0: 7472 696e 672c 2045 7272 6f72 206d 6573  tring, Error mes
-00014bf0: 7361 6765 2069 6620 7468 6520 696e 7075  sage if the inpu
-00014c00: 7420 6973 2069 6e76 616c 6964 2e0a 2020  t is invalid..  
-00014c10: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00014c20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00014c30: 2020 2020 616c 6c6f 7765 645f 7479 7065      allowed_type
-00014c40: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00014c50: 2020 2020 2020 5369 6d75 6c61 7469 6f6e        Simulation
-00014c60: 5479 7065 2e53 494e 474c 455f 4245 4144  Type.SINGLE_BEAD
-00014c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014c80: 2020 5369 6d75 6c61 7469 6f6e 5479 7065    SimulationType
-00014c90: 2e50 4f52 4f53 4954 592c 0a20 2020 2020  .POROSITY,.     
-00014ca0: 2020 2020 2020 2020 2020 2053 696d 756c             Simul
-00014cb0: 6174 696f 6e54 7970 652e 4d49 4352 4f53  ationType.MICROS
-00014cc0: 5452 5543 5455 5245 2c0a 2020 2020 2020  TRUCTURE,.      
-00014cd0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00014ce0: 2020 2020 6966 2069 6e70 7574 5b43 6f6c      if input[Col
-00014cf0: 756d 6e4e 616d 6573 2e54 5950 455d 206e  umnNames.TYPE] n
-00014d00: 6f74 2069 6e20 616c 6c6f 7765 645f 7479  ot in allowed_ty
-00014d10: 7065 733a 0a20 2020 2020 2020 2020 2020  pes:.           
-00014d20: 2020 2020 2072 6574 7572 6e20 2846 616c       return (Fal
-00014d30: 7365 2c20 6622 496e 7661 6c69 6420 7369  se, f"Invalid si
-00014d40: 6d75 6c61 7469 6f6e 2074 7970 653a 207b  mulation type: {
-00014d50: 696e 7075 745b 436f 6c75 6d6e 4e61 6d65  input[ColumnName
-00014d60: 732e 5459 5045 5d7d 2e22 290a 0a20 2020  s.TYPE]}.")..   
-00014d70: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
-00014d80: 7274 206e 616e 2074 6f20 6465 6661 756c  rt nan to defaul
-00014d90: 7420 7661 6c75 6573 206f 6e6c 7920 666f  t values only fo
-00014da0: 7220 7369 6e67 6c65 2062 6561 6420 7369  r single bead si
-00014db0: 6d75 6c61 7469 6f6e 730a 2020 2020 2020  mulations.      
-00014dc0: 2020 2020 2020 2320 666f 7220 6f74 6865        # for othe
-00014dd0: 7220 7369 6d75 6c61 7469 6f6e 2074 7970  r simulation typ
-00014de0: 6573 2c20 6e61 6e20 7661 6c75 6573 2061  es, nan values a
-00014df0: 7265 206e 6f74 2061 6c6c 6f77 6564 0a20  re not allowed. 
-00014e00: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00014e10: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
-00014e20: 5459 5045 5d20 3d3d 2053 696d 756c 6174  TYPE] == Simulat
-00014e30: 696f 6e54 7970 652e 5349 4e47 4c45 5f42  ionType.SINGLE_B
-00014e40: 4541 443a 0a20 2020 2020 2020 2020 2020  EAD:.           
-00014e50: 2020 2020 2069 6620 6e70 2e69 736e 616e       if np.isnan
-00014e60: 2869 6e70 7574 5b43 6f6c 756d 6e4e 616d  (input[ColumnNam
-00014e70: 6573 2e53 5441 5254 5f41 4e47 4c45 5d29  es.START_ANGLE])
-00014e80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014e90: 2020 2020 2020 696e 7075 745b 436f 6c75        input[Colu
-00014ea0: 6d6e 4e61 6d65 732e 5354 4152 545f 414e  mnNames.START_AN
-00014eb0: 474c 455d 203d 204d 6163 6869 6e65 436f  GLE] = MachineCo
-00014ec0: 6e73 7461 6e74 732e 4445 4641 554c 545f  nstants.DEFAULT_
-00014ed0: 5354 4152 5449 4e47 5f4c 4159 4552 5f41  STARTING_LAYER_A
-00014ee0: 4e47 4c45 0a20 2020 2020 2020 2020 2020  NGLE.           
-00014ef0: 2020 2020 2069 6620 6e70 2e69 736e 616e       if np.isnan
-00014f00: 2869 6e70 7574 5b43 6f6c 756d 6e4e 616d  (input[ColumnNam
-00014f10: 6573 2e52 4f54 4154 494f 4e5f 414e 474c  es.ROTATION_ANGL
-00014f20: 455d 293a 0a20 2020 2020 2020 2020 2020  E]):.           
-00014f30: 2020 2020 2020 2020 2069 6e70 7574 5b0a           input[.
-00014f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f50: 2020 2020 2020 2020 436f 6c75 6d6e 4e61          ColumnNa
-00014f60: 6d65 732e 524f 5441 5449 4f4e 5f41 4e47  mes.ROTATION_ANG
-00014f70: 4c45 0a20 2020 2020 2020 2020 2020 2020  LE.             
-00014f80: 2020 2020 2020 205d 203d 204d 6163 6869         ] = Machi
-00014f90: 6e65 436f 6e73 7461 6e74 732e 4445 4641  neConstants.DEFA
-00014fa0: 554c 545f 4c41 5945 525f 524f 5441 5449  ULT_LAYER_ROTATI
-00014fb0: 4f4e 5f41 4e47 4c45 0a20 2020 2020 2020  ON_ANGLE.       
-00014fc0: 2020 2020 2020 2020 2069 6620 6e70 2e69           if np.i
-00014fd0: 736e 616e 2869 6e70 7574 5b43 6f6c 756d  snan(input[Colum
-00014fe0: 6e4e 616d 6573 2e48 4154 4348 5f53 5041  nNames.HATCH_SPA
-00014ff0: 4349 4e47 5d29 3a0a 2020 2020 2020 2020  CING]):.        
-00015000: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-00015010: 745b 436f 6c75 6d6e 4e61 6d65 732e 4841  t[ColumnNames.HA
-00015020: 5443 485f 5350 4143 494e 475d 203d 204d  TCH_SPACING] = M
-00015030: 6163 6869 6e65 436f 6e73 7461 6e74 732e  achineConstants.
-00015040: 4445 4641 554c 545f 4841 5443 485f 5350  DEFAULT_HATCH_SP
-00015050: 4143 494e 470a 2020 2020 2020 2020 2020  ACING.          
-00015060: 2020 2020 2020 6966 206e 702e 6973 6e61        if np.isna
-00015070: 6e28 696e 7075 745b 436f 6c75 6d6e 4e61  n(input[ColumnNa
-00015080: 6d65 732e 5354 5249 5045 5f57 4944 5448  mes.STRIPE_WIDTH
-00015090: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-000150a0: 2020 2020 2020 2020 696e 7075 745b 436f          input[Co
-000150b0: 6c75 6d6e 4e61 6d65 732e 5354 5249 5045  lumnNames.STRIPE
-000150c0: 5f57 4944 5448 5d20 3d20 4d61 6368 696e  _WIDTH] = Machin
-000150d0: 6543 6f6e 7374 616e 7473 2e44 4546 4155  eConstants.DEFAU
-000150e0: 4c54 5f53 4c49 4349 4e47 5f53 5452 4950  LT_SLICING_STRIP
-000150f0: 455f 5749 4454 480a 0a20 2020 2020 2020  E_WIDTH..       
-00015100: 2020 2020 206d 6163 6869 6e65 203d 2041       machine = A
-00015110: 6464 6974 6976 654d 6163 6869 6e65 280a  dditiveMachine(.
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 6c61 7365 725f 706f 7765 723d 696e 7075  laser_power=inpu
-00015140: 745b 436f 6c75 6d6e 4e61 6d65 732e 4c41  t[ColumnNames.LA
-00015150: 5345 525f 504f 5745 525d 2c0a 2020 2020  SER_POWER],.    
-00015160: 2020 2020 2020 2020 2020 2020 7363 616e              scan
-00015170: 5f73 7065 6564 3d69 6e70 7574 5b43 6f6c  _speed=input[Col
-00015180: 756d 6e4e 616d 6573 2e53 4341 4e5f 5350  umnNames.SCAN_SP
-00015190: 4545 445d 2c0a 2020 2020 2020 2020 2020  EED],.          
-000151a0: 2020 2020 2020 6865 6174 6572 5f74 656d        heater_tem
-000151b0: 7065 7261 7475 7265 3d69 6e70 7574 5b43  perature=input[C
-000151c0: 6f6c 756d 6e4e 616d 6573 2e48 4541 5445  olumnNames.HEATE
-000151d0: 525f 5445 4d50 4552 4154 5552 455d 2c0a  R_TEMPERATURE],.
+00013f60: 2253 7461 7274 2041 6e67 6c65 2028 c2b0  "Start Angle (..
+00013f70: 2922 3a20 436f 6c75 6d6e 4e61 6d65 732e  )": ColumnNames.
+00013f80: 5354 4152 545f 414e 474c 452c 0a20 2020  START_ANGLE,.   
+00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fa0: 2022 526f 7461 7469 6f6e 2041 6e67 6c65   "Rotation Angle
+00013fb0: 2028 c2b0 2922 3a20 436f 6c75 6d6e 4e61   (..)": ColumnNa
+00013fc0: 6d65 732e 524f 5441 5449 4f4e 5f41 4e47  mes.ROTATION_ANG
+00013fd0: 4c45 2c0a 2020 2020 2020 2020 2020 2020  LE,.            
+00013fe0: 2020 2020 2020 2020 2243 6f6f 6c69 6e67          "Cooling
+00013ff0: 2052 6174 6520 28c2 b04b 2f73 2922 3a20   Rate (..K/s)": 
+00014000: 436f 6c75 6d6e 4e61 6d65 732e 434f 4f4c  ColumnNames.COOL
+00014010: 494e 475f 5241 5445 2c0a 2020 2020 2020  ING_RATE,.      
+00014020: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+00014030: 6865 726d 616c 2047 7261 6469 656e 7420  hermal Gradient 
+00014040: 28c2 b04b 2f6d 2922 3a20 436f 6c75 6d6e  (..K/m)": Column
+00014050: 4e61 6d65 732e 5448 4552 4d41 4c5f 4752  Names.THERMAL_GR
+00014060: 4144 4945 4e54 2c0a 2020 2020 2020 2020  ADIENT,.        
+00014070: 2020 2020 2020 2020 2020 2020 2258 5920              "XY 
+00014080: 4176 6572 6167 6520 4772 6169 6e20 5369  Average Grain Si
+00014090: 7a65 2028 c2b5 6d29 223a 2043 6f6c 756d  ze (..m)": Colum
+000140a0: 6e4e 616d 6573 2e58 595f 4156 4552 4147  nNames.XY_AVERAG
+000140b0: 455f 4752 4149 4e5f 5349 5a45 2c0a 2020  E_GRAIN_SIZE,.  
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140d0: 2020 2258 5a20 4176 6572 6167 6520 4772    "XZ Average Gr
+000140e0: 6169 6e20 5369 7a65 2028 c2b5 6d29 223a  ain Size (..m)":
+000140f0: 2043 6f6c 756d 6e4e 616d 6573 2e58 5a5f   ColumnNames.XZ_
+00014100: 4156 4552 4147 455f 4752 4149 4e5f 5349  AVERAGE_GRAIN_SI
+00014110: 5a45 2c0a 2020 2020 2020 2020 2020 2020  ZE,.            
+00014120: 2020 2020 2020 2020 2259 5a20 4176 6572          "YZ Aver
+00014130: 6167 6520 4772 6169 6e20 5369 7a65 2028  age Grain Size (
+00014140: c2b5 6d29 223a 2043 6f6c 756d 6e4e 616d  ..m)": ColumnNam
+00014150: 6573 2e59 5a5f 4156 4552 4147 455f 4752  es.YZ_AVERAGE_GR
+00014160: 4149 4e5f 5349 5a45 2c0a 2020 2020 2020  AIN_SIZE,.      
+00014170: 2020 2020 2020 2020 2020 2020 2020 224d                "M
+00014180: 656c 7420 506f 6f6c 204c 656e 6774 682f  elt Pool Length/
+00014190: 5769 6474 6820 286d 2922 3a20 436f 6c75  Width (m)": Colu
+000141a0: 6d6e 4e61 6d65 732e 4d45 4c54 5f50 4f4f  mnNames.MELT_POO
+000141b0: 4c5f 4c45 4e47 5448 5f4f 5645 525f 5749  L_LENGTH_OVER_WI
+000141c0: 4454 482c 0a20 2020 2020 2020 2020 2020  DTH,.           
+000141d0: 2020 2020 2020 2020 2022 4d65 6c74 2050           "Melt P
+000141e0: 6f6f 6c20 5265 6620 4465 7074 682f 5769  ool Ref Depth/Wi
+000141f0: 6474 6820 286d 2922 3a20 436f 6c75 6d6e  dth (m)": Column
+00014200: 4e61 6d65 732e 4d45 4c54 5f50 4f4f 4c5f  Names.MELT_POOL_
+00014210: 5245 4645 5245 4e43 455f 4445 5054 485f  REFERENCE_DEPTH_
+00014220: 4f56 4552 5f57 4944 5448 2c0a 2020 2020  OVER_WIDTH,.    
+00014230: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00014240: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014250: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
+00014260: 3d20 320a 0a20 2020 2020 2020 206e 6577  = 2..        new
+00014270: 5f73 7475 6479 203d 2050 6172 616d 6574  _study = Paramet
+00014280: 7269 6353 7475 6479 2e5f 6e65 7728 7374  ricStudy._new(st
+00014290: 7564 792e 6669 6c65 5f6e 616d 6529 0a20  udy.file_name). 
+000142a0: 2020 2020 2020 206e 6577 5f73 7475 6479         new_study
+000142b0: 2e5f 6461 7461 5f66 7261 6d65 203d 2064  ._data_frame = d
+000142c0: 660a 2020 2020 2020 2020 7265 7475 726e  f.        return
+000142d0: 206e 6577 5f73 7475 6479 0a0a 2020 2020   new_study..    
+000142e0: 4073 6176 655f 6f6e 5f72 6574 7572 6e0a  @save_on_return.
+000142f0: 2020 2020 6465 6620 6164 645f 7369 6d75      def add_simu
+00014300: 6c61 7469 6f6e 735f 6672 6f6d 5f64 6174  lations_from_dat
+00014310: 615f 6672 616d 6528 7365 6c66 2c20 6466  a_frame(self, df
+00014320: 3a20 7064 2e44 6174 6146 7261 6d65 2920  : pd.DataFrame) 
+00014330: 2d3e 206c 6973 745b 7374 725d 3a0a 2020  -> list[str]:.  
+00014340: 2020 2020 2020 2222 2241 6464 2073 696d        """Add sim
+00014350: 756c 6174 696f 6e73 2066 726f 6d20 616e  ulations from an
+00014360: 2069 6d70 6f72 7465 6420 4353 5620 6669   imported CSV fi
+00014370: 6c65 2074 6f20 7468 6520 7061 7261 6d65  le to the parame
+00014380: 7472 6963 2073 7475 6479 2e0a 0a20 2020  tric study...   
+00014390: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000143a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000143b0: 2d2d 0a20 2020 2020 2020 2064 6620 3a20  --.        df : 
+000143c0: 7064 2e44 6174 6146 7261 6d65 0a20 2020  pd.DataFrame.   
+000143d0: 2020 2020 2020 2020 2044 6174 6120 6672           Data fr
+000143e0: 616d 6520 6f66 2074 6865 2063 7376 2066  ame of the csv f
+000143f0: 696c 6520 636f 6e74 6169 6e69 6e67 2073  ile containing s
+00014400: 696d 756c 6174 696f 6e73 2074 6f20 6265  imulations to be
+00014410: 2061 6464 6564 2074 6f20 7468 6520 7061   added to the pa
+00014420: 7261 6d65 7472 6963 2073 7475 6479 2e0a  rametric study..
+00014430: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00014440: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00014450: 0a20 2020 2020 2020 206c 6973 745b 7374  .        list[st
+00014460: 725d 0a20 2020 2020 2020 2020 2020 204c  r].            L
+00014470: 6973 7420 6f66 2065 7272 6f72 206d 6573  ist of error mes
+00014480: 7361 6765 7320 666f 7220 696e 7661 6c69  sages for invali
+00014490: 6420 7369 6d75 6c61 7469 6f6e 732e 0a20  d simulations.. 
+000144a0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000144b0: 2020 2020 2320 6368 6563 6b20 7661 6c69      # check vali
+000144c0: 6420 696e 7075 7473 0a20 2020 2020 2020  d inputs.       
+000144d0: 2064 726f 705f 696e 6469 6365 732c 2065   drop_indices, e
+000144e0: 7272 6f72 5f6c 6973 7420 3d20 6c69 7374  rror_list = list
+000144f0: 2829 2c20 6c69 7374 2829 0a20 2020 2020  (), list().     
+00014500: 2020 2064 7570 6c69 6361 7465 7320 3d20     duplicates = 
+00014510: 300a 2020 2020 2020 2020 616c 6c6f 7765  0.        allowe
+00014520: 645f 7374 6174 7573 203d 205b 0a20 2020  d_status = [.   
+00014530: 2020 2020 2020 2020 2053 696d 756c 6174           Simulat
+00014540: 696f 6e53 7461 7475 732e 434f 4d50 4c45  ionStatus.COMPLE
+00014550: 5445 442c 0a20 2020 2020 2020 2020 2020  TED,.           
+00014560: 2053 696d 756c 6174 696f 6e53 7461 7475   SimulationStatu
+00014570: 732e 5045 4e44 494e 472c 0a20 2020 2020  s.PENDING,.     
+00014580: 2020 2020 2020 2053 696d 756c 6174 696f         Simulatio
+00014590: 6e53 7461 7475 732e 534b 4950 2c0a 2020  nStatus.SKIP,.  
+000145a0: 2020 2020 2020 2020 2020 5369 6d75 6c61            Simula
+000145b0: 7469 6f6e 5374 6174 7573 2e45 5252 4f52  tionStatus.ERROR
+000145c0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+000145d0: 2020 2020 666f 7220 696e 6465 782c 2072      for index, r
+000145e0: 6f77 2069 6e20 6466 2e69 7465 7272 6f77  ow in df.iterrow
+000145f0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00014600: 2076 616c 6964 203d 2046 616c 7365 0a20   valid = False. 
+00014610: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+00014620: 775b 436f 6c75 6d6e 4e61 6d65 732e 5354  w[ColumnNames.ST
+00014630: 4154 5553 5d20 696e 2061 6c6c 6f77 6564  ATUS] in allowed
+00014640: 5f73 7461 7475 733a 0a20 2020 2020 2020  _status:.       
+00014650: 2020 2020 2020 2020 2076 616c 6964 2c20           valid, 
+00014660: 6572 726f 7220 3d20 7365 6c66 2e5f 7661  error = self._va
+00014670: 6c69 6461 7465 5f69 6e70 7574 2872 6f77  lidate_input(row
+00014680: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00014690: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000146a0: 2020 2020 7661 6c69 642c 2065 7272 6f72      valid, error
+000146b0: 203d 2028 4661 6c73 652c 2066 2249 6e76   = (False, f"Inv
+000146c0: 616c 6964 2073 696d 756c 6174 696f 6e20  alid simulation 
+000146d0: 7374 6174 7573 207b 726f 775b 436f 6c75  status {row[Colu
+000146e0: 6d6e 4e61 6d65 732e 5354 4154 5553 5d7d  mnNames.STATUS]}
+000146f0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00014700: 6620 6e6f 7420 7661 6c69 643a 0a20 2020  f not valid:.   
+00014710: 2020 2020 2020 2020 2020 2020 2064 726f               dro
+00014720: 705f 696e 6469 6365 732e 6170 7065 6e64  p_indices.append
+00014730: 2869 6e64 6578 290a 2020 2020 2020 2020  (index).        
+00014740: 2020 2020 2020 2020 6572 726f 725f 6c69          error_li
+00014750: 7374 2e61 7070 656e 6428 6572 726f 7229  st.append(error)
+00014760: 0a0a 2020 2020 2020 2020 2320 6472 6f70  ..        # drop
+00014770: 2069 6e76 616c 6964 2069 6e70 7574 730a   invalid inputs.
+00014780: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00014790: 6472 6f70 2864 726f 705f 696e 6469 6365  drop(drop_indice
+000147a0: 7329 0a0a 2020 2020 2020 2020 2320 6164  s)..        # ad
+000147b0: 6420 7369 6d75 6c61 7469 6f6e 7320 746f  d simulations to
+000147c0: 2074 6865 2070 6172 616d 6574 7269 6320   the parametric 
+000147d0: 7374 7564 7920 616e 6420 6472 6f70 2064  study and drop d
+000147e0: 7570 6c69 6361 7465 730a 2020 2020 2020  uplicates.      
+000147f0: 2020 666f 7220 7374 6174 7573 2c20 6f76    for status, ov
+00014800: 6572 7772 6974 6520 696e 205b 0a20 2020  erwrite in [.   
+00014810: 2020 2020 2020 2020 2028 5369 6d75 6c61           (Simula
+00014820: 7469 6f6e 5374 6174 7573 2e43 4f4d 504c  tionStatus.COMPL
+00014830: 4554 4544 2c20 5472 7565 292c 0a20 2020  ETED, True),.   
+00014840: 2020 2020 2020 2020 2028 5369 6d75 6c61           (Simula
+00014850: 7469 6f6e 5374 6174 7573 2e50 454e 4449  tionStatus.PENDI
+00014860: 4e47 2c20 4661 6c73 6529 2c0a 2020 2020  NG, False),.    
+00014870: 2020 2020 2020 2020 2853 696d 756c 6174          (Simulat
+00014880: 696f 6e53 7461 7475 732e 534b 4950 2c20  ionStatus.SKIP, 
+00014890: 4661 6c73 6529 2c0a 2020 2020 2020 2020  False),.        
+000148a0: 2020 2020 2853 696d 756c 6174 696f 6e53      (SimulationS
+000148b0: 7461 7475 732e 4552 524f 522c 2046 616c  tatus.ERROR, Fal
+000148c0: 7365 292c 0a20 2020 2020 2020 205d 3a0a  se),.        ]:.
+000148d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000148e0: 656e 2864 665b 6466 5b43 6f6c 756d 6e4e  en(df[df[ColumnN
+000148f0: 616d 6573 2e53 5441 5455 535d 203d 3d20  ames.STATUS] == 
+00014900: 7374 6174 7573 5d29 203e 2030 3a0a 2020  status]) > 0:.  
+00014910: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014920: 6c66 2e5f 6461 7461 5f66 7261 6d65 203d  lf._data_frame =
+00014930: 2070 642e 636f 6e63 6174 280a 2020 2020   pd.concat(.    
+00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014950: 5b73 656c 662e 5f64 6174 615f 6672 616d  [self._data_fram
+00014960: 652c 2064 665b 6466 5b43 6f6c 756d 6e4e  e, df[df[ColumnN
+00014970: 616d 6573 2e53 5441 5455 535d 203d 3d20  ames.STATUS] == 
+00014980: 7374 6174 7573 5d5d 2c0a 2020 2020 2020  status]],.      
+00014990: 2020 2020 2020 2020 2020 2020 2020 6967                ig
+000149a0: 6e6f 7265 5f69 6e64 6578 3d54 7275 652c  nore_index=True,
+000149b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000149c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000149d0: 2020 2064 7570 6c69 6361 7465 7320 2b3d     duplicates +=
+000149e0: 2073 656c 662e 5f72 656d 6f76 655f 6475   self._remove_du
+000149f0: 706c 6963 6174 655f 656e 7472 6965 7328  plicate_entries(
+00014a00: 6f76 6572 7772 6974 653d 6f76 6572 7772  overwrite=overwr
+00014a10: 6974 6529 0a0a 2020 2020 2020 2020 2320  ite)..        # 
+00014a20: 636f 6e76 6572 7420 7072 696f 7269 7479  convert priority
+00014a30: 2c20 6974 6572 6174 696f 6e2c 2061 6e64  , iteration, and
+00014a40: 2072 616e 646f 6d20 7365 6564 2074 6f20   random seed to 
+00014a50: 696e 7420 7479 7065 2065 7870 6c69 6369  int type explici
+00014a60: 746c 790a 2020 2020 2020 2020 7365 6c66  tly.        self
+00014a70: 2e5f 6461 7461 5f66 7261 6d65 5b43 6f6c  ._data_frame[Col
+00014a80: 756d 6e4e 616d 6573 2e50 5249 4f52 4954  umnNames.PRIORIT
+00014a90: 595d 203d 2073 656c 662e 5f64 6174 615f  Y] = self._data_
+00014aa0: 6672 616d 655b 436f 6c75 6d6e 4e61 6d65  frame[ColumnName
+00014ab0: 732e 5052 494f 5249 5459 5d2e 6173 7479  s.PRIORITY].asty
+00014ac0: 7065 280a 2020 2020 2020 2020 2020 2020  pe(.            
+00014ad0: 7064 2e49 6e74 3634 4474 7970 6528 290a  pd.Int64Dtype().
+00014ae0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00014af0: 2020 7365 6c66 2e5f 6461 7461 5f66 7261    self._data_fra
+00014b00: 6d65 5b43 6f6c 756d 6e4e 616d 6573 2e49  me[ColumnNames.I
+00014b10: 5445 5241 5449 4f4e 5d20 3d20 7365 6c66  TERATION] = self
+00014b20: 2e5f 6461 7461 5f66 7261 6d65 5b43 6f6c  ._data_frame[Col
+00014b30: 756d 6e4e 616d 6573 2e49 5445 5241 5449  umnNames.ITERATI
+00014b40: 4f4e 5d2e 6173 7479 7065 280a 2020 2020  ON].astype(.    
+00014b50: 2020 2020 2020 2020 7064 2e49 6e74 3634          pd.Int64
+00014b60: 4474 7970 6528 290a 2020 2020 2020 2020  Dtype().        
+00014b70: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00014b80: 6461 7461 5f66 7261 6d65 5b43 6f6c 756d  data_frame[Colum
+00014b90: 6e4e 616d 6573 2e52 414e 444f 4d5f 5345  nNames.RANDOM_SE
+00014ba0: 4544 5d20 3d20 7365 6c66 2e5f 6461 7461  ED] = self._data
+00014bb0: 5f66 7261 6d65 5b0a 2020 2020 2020 2020  _frame[.        
+00014bc0: 2020 2020 436f 6c75 6d6e 4e61 6d65 732e      ColumnNames.
+00014bd0: 5241 4e44 4f4d 5f53 4545 440a 2020 2020  RANDOM_SEED.    
+00014be0: 2020 2020 5d2e 6173 7479 7065 2870 642e      ].astype(pd.
+00014bf0: 496e 7436 3444 7479 7065 2829 290a 0a20  Int64Dtype()).. 
+00014c00: 2020 2020 2020 2069 6620 6475 706c 6963         if duplic
+00014c10: 6174 6573 203e 2030 3a0a 2020 2020 2020  ates > 0:.      
+00014c20: 2020 2020 2020 6572 726f 725f 6c69 7374        error_list
+00014c30: 2e61 7070 656e 6428 6622 5265 6d6f 7665  .append(f"Remove
+00014c40: 6420 7b64 7570 6c69 6361 7465 737d 2064  d {duplicates} d
+00014c50: 7570 6c69 6361 7465 2073 696d 756c 6174  uplicate simulat
+00014c60: 696f 6e28 7329 2e22 290a 2020 2020 2020  ion(s).").      
+00014c70: 2020 7265 7475 726e 2065 7272 6f72 5f6c    return error_l
+00014c80: 6973 740a 0a20 2020 2064 6566 205f 7661  ist..    def _va
+00014c90: 6c69 6461 7465 5f69 6e70 7574 2873 656c  lidate_input(sel
+00014ca0: 662c 2069 6e70 7574 3a20 7064 2e53 6572  f, input: pd.Ser
+00014cb0: 6965 7329 3a0a 2020 2020 2020 2020 2222  ies):.        ""
+00014cc0: 2254 6573 7420 696e 7075 7420 6672 6f6d  "Test input from
+00014cd0: 2061 2072 6f77 206f 6620 6120 4353 5620   a row of a CSV 
+00014ce0: 6669 6c65 2066 6f72 2076 616c 6964 2069  file for valid i
+00014cf0: 6e70 7574 2070 6172 616d 6574 6572 732e  nput parameters.
+00014d00: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00014d10: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00014d20: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00014d30: 696e 7075 7420 3a20 7064 2e53 6572 6965  input : pd.Serie
+00014d40: 730a 2020 2020 2020 2020 2020 2020 526f  s.            Ro
+00014d50: 7720 6f66 2061 2043 5356 2066 696c 6520  w of a CSV file 
+00014d60: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
+00014d70: 696d 756c 6174 696f 6e20 696e 7075 742e  imulation input.
+00014d80: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00014d90: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00014da0: 2d0a 2020 2020 2020 2020 7475 706c 655b  -.        tuple[
+00014db0: 626f 6f6c 2c20 7374 725d 0a20 2020 2020  bool, str].     
+00014dc0: 2020 2020 2020 2062 6f6f 6c2c 2054 7275         bool, Tru
+00014dd0: 6520 6966 2074 6865 2069 6e70 7574 2069  e if the input i
+00014de0: 7320 7661 6c69 642c 2046 616c 7365 206f  s valid, False o
+00014df0: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
+00014e00: 2020 2020 2020 7374 7269 6e67 2c20 4572        string, Er
+00014e10: 726f 7220 6d65 7373 6167 6520 6966 2074  ror message if t
+00014e20: 6865 2069 6e70 7574 2069 7320 696e 7661  he input is inva
+00014e30: 6c69 642e 0a20 2020 2020 2020 2022 2222  lid..        """
+00014e40: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
+00014e50: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
+00014e60: 6564 5f74 7970 6573 203d 205b 0a20 2020  ed_types = [.   
+00014e70: 2020 2020 2020 2020 2020 2020 2053 696d               Sim
+00014e80: 756c 6174 696f 6e54 7970 652e 5349 4e47  ulationType.SING
+00014e90: 4c45 5f42 4541 442c 0a20 2020 2020 2020  LE_BEAD,.       
+00014ea0: 2020 2020 2020 2020 2053 696d 756c 6174           Simulat
+00014eb0: 696f 6e54 7970 652e 504f 524f 5349 5459  ionType.POROSITY
+00014ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014ed0: 2020 5369 6d75 6c61 7469 6f6e 5479 7065    SimulationType
+00014ee0: 2e4d 4943 524f 5354 5255 4354 5552 452c  .MICROSTRUCTURE,
+00014ef0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00014f00: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00014f10: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
+00014f20: 5459 5045 5d20 6e6f 7420 696e 2061 6c6c  TYPE] not in all
+00014f30: 6f77 6564 5f74 7970 6573 3a0a 2020 2020  owed_types:.    
+00014f40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014f50: 726e 2028 4661 6c73 652c 2066 2249 6e76  rn (False, f"Inv
+00014f60: 616c 6964 2073 696d 756c 6174 696f 6e20  alid simulation 
+00014f70: 7479 7065 3a20 7b69 6e70 7574 5b43 6f6c  type: {input[Col
+00014f80: 756d 6e4e 616d 6573 2e54 5950 455d 7d2e  umnNames.TYPE]}.
+00014f90: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00014fa0: 2320 636f 6e76 6572 7420 6e61 6e20 746f  # convert nan to
+00014fb0: 2064 6566 6175 6c74 2076 616c 7565 7320   default values 
+00014fc0: 6f6e 6c79 2066 6f72 2073 696e 676c 6520  only for single 
+00014fd0: 6265 6164 2073 696d 756c 6174 696f 6e73  bead simulations
+00014fe0: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
+00014ff0: 6f72 206f 7468 6572 2073 696d 756c 6174  or other simulat
+00015000: 696f 6e20 7479 7065 732c 206e 616e 2076  ion types, nan v
+00015010: 616c 7565 7320 6172 6520 6e6f 7420 616c  alues are not al
+00015020: 6c6f 7765 640a 2020 2020 2020 2020 2020  lowed.          
+00015030: 2020 6966 2069 6e70 7574 5b43 6f6c 756d    if input[Colum
+00015040: 6e4e 616d 6573 2e54 5950 455d 203d 3d20  nNames.TYPE] == 
+00015050: 5369 6d75 6c61 7469 6f6e 5479 7065 2e53  SimulationType.S
+00015060: 494e 474c 455f 4245 4144 3a0a 2020 2020  INGLE_BEAD:.    
+00015070: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00015080: 702e 6973 6e61 6e28 696e 7075 745b 436f  p.isnan(input[Co
+00015090: 6c75 6d6e 4e61 6d65 732e 5354 4152 545f  lumnNames.START_
+000150a0: 414e 474c 455d 293a 0a20 2020 2020 2020  ANGLE]):.       
+000150b0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+000150c0: 7574 5b43 6f6c 756d 6e4e 616d 6573 2e53  ut[ColumnNames.S
+000150d0: 5441 5254 5f41 4e47 4c45 5d20 3d20 4d61  TART_ANGLE] = Ma
+000150e0: 6368 696e 6543 6f6e 7374 616e 7473 2e44  chineConstants.D
+000150f0: 4546 4155 4c54 5f53 5441 5254 494e 475f  EFAULT_STARTING_
+00015100: 4c41 5945 525f 414e 474c 450a 2020 2020  LAYER_ANGLE.    
+00015110: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00015120: 702e 6973 6e61 6e28 696e 7075 745b 436f  p.isnan(input[Co
+00015130: 6c75 6d6e 4e61 6d65 732e 524f 5441 5449  lumnNames.ROTATI
+00015140: 4f4e 5f41 4e47 4c45 5d29 3a0a 2020 2020  ON_ANGLE]):.    
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 696e 7075 745b 0a20 2020 2020 2020 2020  input[.         
+00015170: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00015180: 6f6c 756d 6e4e 616d 6573 2e52 4f54 4154  olumnNames.ROTAT
+00015190: 494f 4e5f 414e 474c 450a 2020 2020 2020  ION_ANGLE.      
+000151a0: 2020 2020 2020 2020 2020 2020 2020 5d20                ] 
+000151b0: 3d20 4d61 6368 696e 6543 6f6e 7374 616e  = MachineConstan
+000151c0: 7473 2e44 4546 4155 4c54 5f4c 4159 4552  ts.DEFAULT_LAYER
+000151d0: 5f52 4f54 4154 494f 4e5f 414e 474c 450a  _ROTATION_ANGLE.
 000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 6c61 7965 725f 7468 6963 6b6e 6573 733d  layer_thickness=
-00015200: 696e 7075 745b 436f 6c75 6d6e 4e61 6d65  input[ColumnName
-00015210: 732e 4c41 5945 525f 5448 4943 4b4e 4553  s.LAYER_THICKNES
-00015220: 535d 2c0a 2020 2020 2020 2020 2020 2020  S],.            
-00015230: 2020 2020 6265 616d 5f64 6961 6d65 7465      beam_diamete
-00015240: 723d 696e 7075 745b 436f 6c75 6d6e 4e61  r=input[ColumnNa
-00015250: 6d65 732e 4245 414d 5f44 4941 4d45 5445  mes.BEAM_DIAMETE
-00015260: 525d 2c0a 2020 2020 2020 2020 2020 2020  R],.            
-00015270: 2020 2020 7374 6172 7469 6e67 5f6c 6179      starting_lay
-00015280: 6572 5f61 6e67 6c65 3d69 6e70 7574 5b43  er_angle=input[C
-00015290: 6f6c 756d 6e4e 616d 6573 2e53 5441 5254  olumnNames.START
-000152a0: 5f41 4e47 4c45 5d2c 0a20 2020 2020 2020  _ANGLE],.       
-000152b0: 2020 2020 2020 2020 206c 6179 6572 5f72           layer_r
-000152c0: 6f74 6174 696f 6e5f 616e 676c 653d 696e  otation_angle=in
-000152d0: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
-000152e0: 524f 5441 5449 4f4e 5f41 4e47 4c45 5d2c  ROTATION_ANGLE],
-000152f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015300: 2068 6174 6368 5f73 7061 6369 6e67 3d69   hatch_spacing=i
-00015310: 6e70 7574 5b43 6f6c 756d 6e4e 616d 6573  nput[ColumnNames
-00015320: 2e48 4154 4348 5f53 5041 4349 4e47 5d2c  .HATCH_SPACING],
-00015330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015340: 2073 6c69 6369 6e67 5f73 7472 6970 655f   slicing_stripe_
-00015350: 7769 6474 683d 696e 7075 745b 436f 6c75  width=input[Colu
-00015360: 6d6e 4e61 6d65 732e 5354 5249 5045 5f57  mnNames.STRIPE_W
-00015370: 4944 5448 5d2c 0a20 2020 2020 2020 2020  IDTH],.         
-00015380: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00015390: 2020 6d61 7465 7269 616c 203d 2041 6464    material = Add
-000153a0: 6974 6976 654d 6174 6572 6961 6c28 6e61  itiveMaterial(na
-000153b0: 6d65 3d73 7472 2869 6e70 7574 5b43 6f6c  me=str(input[Col
-000153c0: 756d 6e4e 616d 6573 2e4d 4154 4552 4941  umnNames.MATERIA
-000153d0: 4c5d 2929 0a0a 2020 2020 2020 2020 2020  L]))..          
-000153e0: 2020 6966 2069 6e70 7574 5b43 6f6c 756d    if input[Colum
-000153f0: 6e4e 616d 6573 2e54 5950 455d 203d 3d20  nNames.TYPE] == 
-00015400: 5369 6d75 6c61 7469 6f6e 5479 7065 2e53  SimulationType.S
-00015410: 494e 474c 455f 4245 4144 3a0a 2020 2020  INGLE_BEAD:.    
-00015420: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-00015430: 642c 2065 7272 6f72 203d 2073 656c 662e  d, error = self.
-00015440: 5f76 616c 6964 6174 655f 7369 6e67 6c65  _validate_single
-00015450: 5f62 6561 645f 696e 7075 7428 6d61 6368  _bead_input(mach
-00015460: 696e 652c 206d 6174 6572 6961 6c2c 2069  ine, material, i
-00015470: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-00015480: 2020 6966 2069 6e70 7574 5b43 6f6c 756d    if input[Colum
-00015490: 6e4e 616d 6573 2e54 5950 455d 203d 3d20  nNames.TYPE] == 
-000154a0: 5369 6d75 6c61 7469 6f6e 5479 7065 2e50  SimulationType.P
-000154b0: 4f52 4f53 4954 593a 0a20 2020 2020 2020  OROSITY:.       
-000154c0: 2020 2020 2020 2020 2076 616c 6964 2c20           valid, 
-000154d0: 6572 726f 7220 3d20 7365 6c66 2e5f 7661  error = self._va
-000154e0: 6c69 6461 7465 5f70 6f72 6f73 6974 795f  lidate_porosity_
-000154f0: 696e 7075 7428 6d61 6368 696e 652c 206d  input(machine, m
-00015500: 6174 6572 6961 6c2c 2069 6e70 7574 290a  aterial, input).
-00015510: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00015520: 6e70 7574 5b43 6f6c 756d 6e4e 616d 6573  nput[ColumnNames
-00015530: 2e54 5950 455d 203d 3d20 5369 6d75 6c61  .TYPE] == Simula
-00015540: 7469 6f6e 5479 7065 2e4d 4943 524f 5354  tionType.MICROST
-00015550: 5255 4354 5552 453a 0a20 2020 2020 2020  RUCTURE:.       
-00015560: 2020 2020 2020 2020 2076 616c 6964 2c20           valid, 
-00015570: 6572 726f 7220 3d20 7365 6c66 2e5f 7661  error = self._va
-00015580: 6c69 6461 7465 5f6d 6963 726f 7374 7275  lidate_microstru
-00015590: 6374 7572 655f 696e 7075 7428 6d61 6368  cture_input(mach
-000155a0: 696e 652c 206d 6174 6572 6961 6c2c 2069  ine, material, i
-000155b0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-000155c0: 2020 6966 206e 6f74 2076 616c 6964 3a0a    if not valid:.
-000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 7265 7475 726e 2028 4661 6c73 652c 2065  return (False, e
-000155f0: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00015600: 2020 7265 7475 726e 2028 5472 7565 2c20    return (True, 
-00015610: 2222 290a 0a20 2020 2020 2020 2065 7863  "")..        exc
-00015620: 6570 7420 5661 6c75 6545 7272 6f72 2061  ept ValueError a
-00015630: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00015640: 2072 6574 7572 6e20 2846 616c 7365 2c20   return (False, 
-00015650: 2866 2249 6e76 616c 6964 2070 6172 616d  (f"Invalid param
-00015660: 6574 6572 2063 6f6d 6269 6e61 7469 6f6e  eter combination
-00015670: 3a20 7b65 7d22 2929 0a0a 2020 2020 6465  : {e}"))..    de
-00015680: 6620 5f76 616c 6964 6174 655f 7369 6e67  f _validate_sing
-00015690: 6c65 5f62 6561 645f 696e 7075 7428 0a20  le_bead_input(. 
-000156a0: 2020 2020 2020 2073 656c 662c 206d 6163         self, mac
-000156b0: 6869 6e65 3a20 4164 6469 7469 7665 4d61  hine: AdditiveMa
-000156c0: 6368 696e 652c 206d 6174 6572 6961 6c3a  chine, material:
-000156d0: 2041 6464 6974 6976 654d 6174 6572 6961   AdditiveMateria
-000156e0: 6c2c 2069 6e70 7574 3a20 7064 2e53 6572  l, input: pd.Ser
-000156f0: 6965 730a 2020 2020 2920 2d3e 2074 7570  ies.    ) -> tup
-00015700: 6c65 5b62 6f6f 6c2c 2073 7472 5d3a 0a20  le[bool, str]:. 
-00015710: 2020 2020 2020 2022 2222 5661 6c69 6461         """Valida
-00015720: 7465 2073 696e 676c 6520 6265 6164 2073  te single bead s
-00015730: 696d 756c 6174 696f 6e20 696e 7075 7420  imulation input 
-00015740: 7661 6c75 6573 2e0a 0a20 2020 2020 2020  values...       
-00015750: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00015760: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00015770: 2020 2020 2020 2069 6e70 7574 203a 2070         input : p
-00015780: 642e 5365 7269 6573 0a20 2020 2020 2020  d.Series.       
-00015790: 2020 2020 2053 696e 676c 6520 6265 6164       Single bead
-000157a0: 2073 696d 756c 6174 696f 6e20 696e 7075   simulation inpu
-000157b0: 742e 0a0a 2020 2020 2020 2020 6d61 6368  t...        mach
-000157c0: 696e 6520 3a20 4164 6469 7469 7665 4d61  ine : AdditiveMa
-000157d0: 6368 696e 650a 2020 2020 2020 2020 2020  chine.          
-000157e0: 2020 4164 6469 7469 7665 206d 6163 6869    Additive machi
-000157f0: 6e65 206f 626a 6563 7420 746f 2075 7365  ne object to use
-00015800: 2066 6f72 2076 616c 6964 6174 696e 6720   for validating 
-00015810: 7468 6520 7369 6e67 6c65 2062 6561 6420  the single bead 
-00015820: 696e 7075 742e 0a0a 2020 2020 2020 2020  input...        
-00015830: 6d61 7465 7269 616c 203a 2041 6464 6974  material : Addit
-00015840: 6976 654d 6174 6572 6961 6c0a 2020 2020  iveMaterial.    
-00015850: 2020 2020 2020 2020 4164 6469 7469 7665          Additive
-00015860: 206d 6174 6572 6961 6c20 6f62 6a65 6374   material object
-00015870: 2074 6f20 7573 6520 666f 7220 7661 6c69   to use for vali
-00015880: 6461 7469 6e67 2074 6865 2073 696e 676c  dating the singl
-00015890: 6520 6265 6164 2069 6e70 7574 2e0a 0a20  e bead input... 
-000158a0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000158b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000158c0: 2020 2020 2020 2074 7570 6c65 5b62 6f6f         tuple[boo
-000158d0: 6c2c 2073 7472 5d0a 2020 2020 2020 2020  l, str].        
-000158e0: 2020 2020 626f 6f6c 2c20 5472 7565 2069      bool, True i
-000158f0: 6620 7468 6520 7369 6e67 6c65 2062 6561  f the single bea
-00015900: 6420 696e 7075 7420 6973 2076 616c 6964  d input is valid
-00015910: 2c20 4661 6c73 6520 6f74 6865 7277 6973  , False otherwis
-00015920: 652e 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00015930: 7472 696e 672c 2045 7272 6f72 206d 6573  tring, Error mes
-00015940: 7361 6765 2069 6620 7468 6520 7369 6e67  sage if the sing
-00015950: 6c65 2062 6561 6420 696e 7075 7420 6973  le bead input is
-00015960: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
-00015970: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00015980: 793a 0a20 2020 2020 2020 2020 2020 2074  y:.            t
-00015990: 6573 745f 6265 6164 5f6c 656e 6774 6820  est_bead_length 
-000159a0: 3d20 696e 7075 745b 436f 6c75 6d6e 4e61  = input[ColumnNa
-000159b0: 6d65 732e 5349 4e47 4c45 5f42 4541 445f  mes.SINGLE_BEAD_
-000159c0: 4c45 4e47 5448 5d0a 0a20 2020 2020 2020  LENGTH]..       
-000159d0: 2020 2020 2074 6573 745f 7369 6e67 6c65       test_single
-000159e0: 5f62 6561 645f 696e 7075 7420 3d20 5369  _bead_input = Si
-000159f0: 6e67 6c65 4265 6164 496e 7075 7428 0a20  ngleBeadInput(. 
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00015a10: 6561 645f 6c65 6e67 7468 3d74 6573 745f  ead_length=test_
-00015a20: 6265 6164 5f6c 656e 6774 682c 206d 6163  bead_length, mac
-00015a30: 6869 6e65 3d6d 6163 6869 6e65 2c20 6d61  hine=machine, ma
-00015a40: 7465 7269 616c 3d6d 6174 6572 6961 6c0a  terial=material.
-00015a50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00015a60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00015a70: 2028 5472 7565 2c20 2222 290a 2020 2020   (True, "").    
-00015a80: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-00015a90: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00015aa0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00015ab0: 4661 6c73 652c 2028 6622 496e 7661 6c69  False, (f"Invali
-00015ac0: 6420 7061 7261 6d65 7465 7220 636f 6d62  d parameter comb
-00015ad0: 696e 6174 696f 6e3a 207b 657d 2229 290a  ination: {e}")).
-00015ae0: 0a20 2020 2064 6566 205f 7661 6c69 6461  .    def _valida
-00015af0: 7465 5f70 6f72 6f73 6974 795f 696e 7075  te_porosity_inpu
-00015b00: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-00015b10: 206d 6163 6869 6e65 3a20 4164 6469 7469   machine: Additi
-00015b20: 7665 4d61 6368 696e 652c 206d 6174 6572  veMachine, mater
-00015b30: 6961 6c3a 2041 6464 6974 6976 654d 6174  ial: AdditiveMat
-00015b40: 6572 6961 6c2c 2069 6e70 7574 3a20 7064  erial, input: pd
-00015b50: 2e53 6572 6965 730a 2020 2020 2920 2d3e  .Series.    ) ->
-00015b60: 2074 7570 6c65 5b62 6f6f 6c2c 2073 7472   tuple[bool, str
-00015b70: 5d3a 0a20 2020 2020 2020 2022 2222 5661  ]:.        """Va
-00015b80: 6c69 6461 7465 2070 6f72 6f73 6974 7920  lidate porosity 
-00015b90: 7369 6d75 6c61 7469 6f6e 2069 6e70 7574  simulation input
-00015ba0: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00015bb0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00015bc0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00015bd0: 2020 2020 2020 2020 696e 7075 7420 3a20          input : 
-00015be0: 7064 2e53 6572 6965 730a 2020 2020 2020  pd.Series.      
-00015bf0: 2020 2020 2020 506f 726f 7369 7479 2073        Porosity s
-00015c00: 696d 756c 6174 696f 6e20 696e 7075 742e  imulation input.
-00015c10: 0a0a 2020 2020 2020 2020 6d61 6368 696e  ..        machin
-00015c20: 6520 3a20 4164 6469 7469 7665 4d61 6368  e : AdditiveMach
-00015c30: 696e 650a 2020 2020 2020 2020 2020 2020  ine.            
-00015c40: 4164 6469 7469 7665 206d 6163 6869 6e65  Additive machine
-00015c50: 206f 626a 6563 7420 746f 2075 7365 2066   object to use f
-00015c60: 6f72 2076 616c 6964 6174 696e 6720 7468  or validating th
-00015c70: 6520 706f 726f 7369 7479 2069 6e70 7574  e porosity input
-00015c80: 2e0a 0a20 2020 2020 2020 206d 6174 6572  ...        mater
-00015c90: 6961 6c20 3a20 4164 6469 7469 7665 4d61  ial : AdditiveMa
-00015ca0: 7465 7269 616c 0a20 2020 2020 2020 2020  terial.         
-00015cb0: 2020 2041 6464 6974 6976 6520 6d61 7465     Additive mate
-00015cc0: 7269 616c 206f 626a 6563 7420 746f 2075  rial object to u
-00015cd0: 7365 2066 6f72 2076 616c 6964 6174 696e  se for validatin
-00015ce0: 6720 7468 6520 706f 726f 7369 7479 2069  g the porosity i
-00015cf0: 6e70 7574 2e0a 0a20 2020 2020 2020 2052  nput...        R
-00015d00: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00015d10: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
-00015d20: 7570 6c65 5b62 6f6f 6c2c 2073 7472 5d0a  uple[bool, str].
-00015d30: 2020 2020 2020 2020 2020 2020 626f 6f6c              bool
-00015d40: 2c20 5472 7565 2069 6620 7468 6520 706f  , True if the po
-00015d50: 726f 7369 7479 2069 6e70 7574 2069 7320  rosity input is 
-00015d60: 7661 6c69 642c 2046 616c 7365 206f 7468  valid, False oth
-00015d70: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00015d80: 2020 2020 7374 7269 6e67 2c20 4572 726f      string, Erro
-00015d90: 7220 6d65 7373 6167 6520 6966 2074 6865  r message if the
-00015da0: 2070 6f72 6f73 6974 7920 696e 7075 7420   porosity input 
-00015db0: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
-00015dc0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00015dd0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00015de0: 2020 7465 7374 5f70 6f72 6f73 6974 795f    test_porosity_
-00015df0: 696e 7075 7420 3d20 506f 726f 7369 7479  input = Porosity
-00015e00: 496e 7075 7428 0a20 2020 2020 2020 2020  Input(.         
-00015e10: 2020 2020 2020 2073 697a 655f 783d 696e         size_x=in
-00015e20: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
-00015e30: 504f 524f 5349 5459 5f53 495a 455f 585d  POROSITY_SIZE_X]
-00015e40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015e50: 2020 7369 7a65 5f79 3d69 6e70 7574 5b43    size_y=input[C
-00015e60: 6f6c 756d 6e4e 616d 6573 2e50 4f52 4f53  olumnNames.POROS
-00015e70: 4954 595f 5349 5a45 5f59 5d2c 0a20 2020  ITY_SIZE_Y],.   
-00015e80: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00015e90: 655f 7a3d 696e 7075 745b 436f 6c75 6d6e  e_z=input[Column
-00015ea0: 4e61 6d65 732e 504f 524f 5349 5459 5f53  Names.POROSITY_S
-00015eb0: 495a 455f 5a5d 2c0a 2020 2020 2020 2020  IZE_Z],.        
-00015ec0: 2020 2020 2020 2020 6d61 6368 696e 653d          machine=
-00015ed0: 6d61 6368 696e 652c 0a20 2020 2020 2020  machine,.       
-00015ee0: 2020 2020 2020 2020 206d 6174 6572 6961           materia
-00015ef0: 6c3d 6d61 7465 7269 616c 2c0a 2020 2020  l=material,.    
-00015f00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00015f10: 2020 2020 2020 7265 7475 726e 2028 5472        return (Tr
-00015f20: 7565 2c20 2222 290a 2020 2020 2020 2020  ue, "").        
-00015f30: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00015f40: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-00015f50: 2020 2020 7265 7475 726e 2028 4661 6c73      return (Fals
-00015f60: 652c 2028 6622 496e 7661 6c69 6420 7061  e, (f"Invalid pa
-00015f70: 7261 6d65 7465 7220 636f 6d62 696e 6174  rameter combinat
-00015f80: 696f 6e3a 207b 657d 2229 290a 0a20 2020  ion: {e}"))..   
-00015f90: 2064 6566 205f 7661 6c69 6461 7465 5f6d   def _validate_m
-00015fa0: 6963 726f 7374 7275 6374 7572 655f 696e  icrostructure_in
-00015fb0: 7075 7428 0a20 2020 2020 2020 2073 656c  put(.        sel
-00015fc0: 662c 206d 6163 6869 6e65 3a20 4164 6469  f, machine: Addi
-00015fd0: 7469 7665 4d61 6368 696e 652c 206d 6174  tiveMachine, mat
-00015fe0: 6572 6961 6c3a 2041 6464 6974 6976 654d  erial: AdditiveM
-00015ff0: 6174 6572 6961 6c2c 2069 6e70 7574 3a20  aterial, input: 
-00016000: 7064 2e53 6572 6965 730a 2020 2020 2920  pd.Series.    ) 
-00016010: 2d3e 2074 7570 6c65 5b62 6f6f 6c2c 2073  -> tuple[bool, s
-00016020: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
-00016030: 5661 6c69 6461 7465 206d 6963 726f 7374  Validate microst
-00016040: 7275 6374 7572 6520 7369 6d75 6c61 7469  ructure simulati
-00016050: 6f6e 2069 6e70 7574 2076 616c 7565 732e  on input values.
-00016060: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00016070: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00016080: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00016090: 696e 7075 7420 3a20 7064 2e53 6572 6965  input : pd.Serie
-000160a0: 730a 2020 2020 2020 2020 2020 2020 4d69  s.            Mi
-000160b0: 6372 6f73 7472 7563 7475 7265 2073 696d  crostructure sim
-000160c0: 756c 6174 696f 6e20 696e 7075 742e 0a0a  ulation input...
-000160d0: 2020 2020 2020 2020 6d61 6368 696e 6520          machine 
-000160e0: 3a20 4164 6469 7469 7665 4d61 6368 696e  : AdditiveMachin
-000160f0: 650a 2020 2020 2020 2020 2020 2020 4164  e.            Ad
-00016100: 6469 7469 7665 206d 6163 6869 6e65 206f  ditive machine o
-00016110: 626a 6563 7420 746f 2075 7365 2066 6f72  bject to use for
-00016120: 2076 616c 6964 6174 696e 6720 7468 6520   validating the 
-00016130: 6d69 6372 6f73 7472 7563 7475 7265 2069  microstructure i
-00016140: 6e70 7574 2e0a 0a20 2020 2020 2020 206d  nput...        m
-00016150: 6174 6572 6961 6c20 3a20 4164 6469 7469  aterial : Additi
-00016160: 7665 4d61 7465 7269 616c 0a20 2020 2020  veMaterial.     
-00016170: 2020 2020 2020 2041 6464 6974 6976 6520         Additive 
-00016180: 6d61 7465 7269 616c 206f 626a 6563 7420  material object 
-00016190: 746f 2075 7365 2066 6f72 2076 616c 6964  to use for valid
-000161a0: 6174 696e 6720 7468 6520 6d69 6372 6f73  ating the micros
-000161b0: 7472 7563 7475 7265 2069 6e70 7574 2e0a  tructure input..
-000161c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000161d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000161e0: 0a20 2020 2020 2020 2074 7570 6c65 5b62  .        tuple[b
-000161f0: 6f6f 6c2c 2073 7472 5d0a 2020 2020 2020  ool, str].      
-00016200: 2020 2020 2020 626f 6f6c 2c20 5472 7565        bool, True
-00016210: 2069 6620 7468 6520 6d69 6372 6f73 7472   if the microstr
-00016220: 7563 7475 7265 2069 6e70 7574 2069 7320  ucture input is 
-00016230: 7661 6c69 642c 2046 616c 7365 206f 7468  valid, False oth
-00016240: 6572 7769 7365 2e0a 2020 2020 2020 2020  erwise..        
-00016250: 2020 2020 7374 7269 6e67 2c20 4572 726f      string, Erro
-00016260: 7220 6d65 7373 6167 6520 6966 2074 6865  r message if the
-00016270: 206d 6963 726f 7374 7275 6374 7572 6520   microstructure 
-00016280: 696e 7075 7420 6973 2069 6e76 616c 6964  input is invalid
-00016290: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000162a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000162b0: 2020 2020 2020 2074 6573 745f 636f 6f6c         test_cool
-000162c0: 696e 675f 7261 7465 203d 2069 6e70 7574  ing_rate = input
-000162d0: 5b43 6f6c 756d 6e4e 616d 6573 2e43 4f4f  [ColumnNames.COO
-000162e0: 4c49 4e47 5f52 4154 455d 0a20 2020 2020  LING_RATE].     
-000162f0: 2020 2020 2020 2074 6573 745f 7468 6572         test_ther
-00016300: 6d61 6c5f 6772 6164 6965 6e74 203d 2069  mal_gradient = i
-00016310: 6e70 7574 5b43 6f6c 756d 6e4e 616d 6573  nput[ColumnNames
-00016320: 2e54 4845 524d 414c 5f47 5241 4449 454e  .THERMAL_GRADIEN
-00016330: 545d 0a20 2020 2020 2020 2020 2020 2074  T].            t
-00016340: 6573 745f 6d65 6c74 5f70 6f6f 6c5f 7769  est_melt_pool_wi
-00016350: 6474 6820 3d20 696e 7075 745b 436f 6c75  dth = input[Colu
-00016360: 6d6e 4e61 6d65 732e 4d49 4352 4f5f 4d45  mnNames.MICRO_ME
-00016370: 4c54 5f50 4f4f 4c5f 5749 4454 485d 0a20  LT_POOL_WIDTH]. 
-00016380: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-00016390: 6d65 6c74 5f70 6f6f 6c5f 6465 7074 6820  melt_pool_depth 
-000163a0: 3d20 696e 7075 745b 436f 6c75 6d6e 4e61  = input[ColumnNa
-000163b0: 6d65 732e 4d49 4352 4f5f 4d45 4c54 5f50  mes.MICRO_MELT_P
-000163c0: 4f4f 4c5f 4445 5054 485d 0a20 2020 2020  OOL_DEPTH].     
-000163d0: 2020 2020 2020 2074 6573 745f 7261 6e64         test_rand
-000163e0: 6f6d 5f73 6565 6420 3d20 696e 7075 745b  om_seed = input[
-000163f0: 436f 6c75 6d6e 4e61 6d65 732e 5241 4e44  ColumnNames.RAND
-00016400: 4f4d 5f53 4545 445d 0a0a 2020 2020 2020  OM_SEED]..      
-00016410: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00016420: 2020 2020 2020 2020 2020 206d 6174 682e             math.
-00016430: 6973 6e61 6e28 7465 7374 5f63 6f6f 6c69  isnan(test_cooli
-00016440: 6e67 5f72 6174 6529 0a20 2020 2020 2020  ng_rate).       
-00016450: 2020 2020 2020 2020 206f 7220 6d61 7468           or math
-00016460: 2e69 736e 616e 2874 6573 745f 7468 6572  .isnan(test_ther
-00016470: 6d61 6c5f 6772 6164 6965 6e74 290a 2020  mal_gradient).  
-00016480: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00016490: 206d 6174 682e 6973 6e61 6e28 7465 7374   math.isnan(test
-000164a0: 5f6d 656c 745f 706f 6f6c 5f77 6964 7468  _melt_pool_width
-000164b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000164c0: 2020 6f72 206d 6174 682e 6973 6e61 6e28    or math.isnan(
-000164d0: 7465 7374 5f6d 656c 745f 706f 6f6c 5f64  test_melt_pool_d
-000164e0: 6570 7468 290a 2020 2020 2020 2020 2020  epth).          
-000164f0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00016500: 2020 2020 2074 6573 745f 7573 655f 7072       test_use_pr
-00016510: 6f76 6964 6564 5f74 6865 726d 616c 5f70  ovided_thermal_p
-00016520: 6172 616d 6574 6572 7320 3d20 4661 6c73  arameters = Fals
-00016530: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-00016540: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016550: 2020 2020 7465 7374 5f75 7365 5f70 726f      test_use_pro
-00016560: 7669 6465 645f 7468 6572 6d61 6c5f 7061  vided_thermal_pa
-00016570: 7261 6d65 7465 7273 203d 2054 7275 650a  rameters = True.
-00016580: 0a20 2020 2020 2020 2020 2020 2074 6573  .            tes
-00016590: 745f 6d69 6372 6f73 7472 7563 7475 7265  t_microstructure
-000165a0: 5f69 6e70 7574 203d 204d 6963 726f 7374  _input = Microst
-000165b0: 7275 6374 7572 6549 6e70 7574 280a 2020  ructureInput(.  
-000165c0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000165d0: 6d70 6c65 5f6d 696e 5f78 3d69 6e70 7574  mple_min_x=input
-000165e0: 5b43 6f6c 756d 6e4e 616d 6573 2e4d 4943  [ColumnNames.MIC
-000165f0: 524f 5f4d 494e 5f58 5d2c 0a20 2020 2020  RO_MIN_X],.     
-00016600: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-00016610: 655f 6d69 6e5f 793d 696e 7075 745b 436f  e_min_y=input[Co
-00016620: 6c75 6d6e 4e61 6d65 732e 4d49 4352 4f5f  lumnNames.MICRO_
-00016630: 4d49 4e5f 595d 2c0a 2020 2020 2020 2020  MIN_Y],.        
-00016640: 2020 2020 2020 2020 7361 6d70 6c65 5f6d          sample_m
-00016650: 696e 5f7a 3d69 6e70 7574 5b43 6f6c 756d  in_z=input[Colum
-00016660: 6e4e 616d 6573 2e4d 4943 524f 5f4d 494e  nNames.MICRO_MIN
-00016670: 5f5a 5d2c 0a20 2020 2020 2020 2020 2020  _Z],.           
-00016680: 2020 2020 2073 616d 706c 655f 7369 7a65       sample_size
-00016690: 5f78 3d69 6e70 7574 5b43 6f6c 756d 6e4e  _x=input[ColumnN
-000166a0: 616d 6573 2e4d 4943 524f 5f53 495a 455f  ames.MICRO_SIZE_
-000166b0: 585d 2c0a 2020 2020 2020 2020 2020 2020  X],.            
-000166c0: 2020 2020 7361 6d70 6c65 5f73 697a 655f      sample_size_
-000166d0: 793d 696e 7075 745b 436f 6c75 6d6e 4e61  y=input[ColumnNa
-000166e0: 6d65 732e 4d49 4352 4f5f 5349 5a45 5f59  mes.MICRO_SIZE_Y
-000166f0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00016700: 2020 2073 616d 706c 655f 7369 7a65 5f7a     sample_size_z
-00016710: 3d69 6e70 7574 5b43 6f6c 756d 6e4e 616d  =input[ColumnNam
-00016720: 6573 2e4d 4943 524f 5f53 495a 455f 5a5d  es.MICRO_SIZE_Z]
-00016730: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016740: 2020 7365 6e73 6f72 5f64 696d 656e 7369    sensor_dimensi
-00016750: 6f6e 3d69 6e70 7574 5b43 6f6c 756d 6e4e  on=input[ColumnN
-00016760: 616d 6573 2e4d 4943 524f 5f53 454e 534f  ames.MICRO_SENSO
-00016770: 525f 4449 4d5d 2c0a 2020 2020 2020 2020  R_DIM],.        
-00016780: 2020 2020 2020 2020 7573 655f 7072 6f76          use_prov
-00016790: 6964 6564 5f74 6865 726d 616c 5f70 6172  ided_thermal_par
-000167a0: 616d 6574 6572 733d 7465 7374 5f75 7365  ameters=test_use
-000167b0: 5f70 726f 7669 6465 645f 7468 6572 6d61  _provided_therma
-000167c0: 6c5f 7061 7261 6d65 7465 7273 2c0a 2020  l_parameters,.  
-000167d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000167e0: 6f6c 696e 675f 7261 7465 3d4d 6963 726f  oling_rate=Micro
-000167f0: 7374 7275 6374 7572 6549 6e70 7574 2e44  structureInput.D
-00016800: 4546 4155 4c54 5f43 4f4f 4c49 4e47 5f52  EFAULT_COOLING_R
-00016810: 4154 450a 2020 2020 2020 2020 2020 2020  ATE.            
-00016820: 2020 2020 6966 2028 7465 7374 5f63 6f6f      if (test_coo
-00016830: 6c69 6e67 5f72 6174 6520 6973 204e 6f6e  ling_rate is Non
-00016840: 6520 6f72 206d 6174 682e 6973 6e61 6e28  e or math.isnan(
-00016850: 7465 7374 5f63 6f6f 6c69 6e67 5f72 6174  test_cooling_rat
-00016860: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00016870: 2020 2020 656c 7365 2074 6573 745f 636f      else test_co
-00016880: 6f6c 696e 675f 7261 7465 2c0a 2020 2020  oling_rate,.    
-00016890: 2020 2020 2020 2020 2020 2020 7468 6572              ther
-000168a0: 6d61 6c5f 6772 6164 6965 6e74 3d4d 6963  mal_gradient=Mic
-000168b0: 726f 7374 7275 6374 7572 6549 6e70 7574  rostructureInput
-000168c0: 2e44 4546 4155 4c54 5f54 4845 524d 414c  .DEFAULT_THERMAL
-000168d0: 5f47 5241 4449 454e 540a 2020 2020 2020  _GRADIENT.      
-000168e0: 2020 2020 2020 2020 2020 6966 2028 7465            if (te
-000168f0: 7374 5f74 6865 726d 616c 5f67 7261 6469  st_thermal_gradi
-00016900: 656e 7420 6973 204e 6f6e 6520 6f72 206d  ent is None or m
-00016910: 6174 682e 6973 6e61 6e28 7465 7374 5f74  ath.isnan(test_t
-00016920: 6865 726d 616c 5f67 7261 6469 656e 7429  hermal_gradient)
-00016930: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016940: 2020 656c 7365 2074 6573 745f 7468 6572    else test_ther
-00016950: 6d61 6c5f 6772 6164 6965 6e74 2c0a 2020  mal_gradient,.  
-00016960: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00016970: 6c74 5f70 6f6f 6c5f 7769 6474 683d 4d69  lt_pool_width=Mi
-00016980: 6372 6f73 7472 7563 7475 7265 496e 7075  crostructureInpu
-00016990: 742e 4445 4641 554c 545f 4d45 4c54 5f50  t.DEFAULT_MELT_P
-000169a0: 4f4f 4c5f 5749 4454 480a 2020 2020 2020  OOL_WIDTH.      
-000169b0: 2020 2020 2020 2020 2020 6966 2028 7465            if (te
-000169c0: 7374 5f6d 656c 745f 706f 6f6c 5f77 6964  st_melt_pool_wid
-000169d0: 7468 2069 7320 4e6f 6e65 206f 7220 6d61  th is None or ma
-000169e0: 7468 2e69 736e 616e 2874 6573 745f 6d65  th.isnan(test_me
-000169f0: 6c74 5f70 6f6f 6c5f 7769 6474 6829 290a  lt_pool_width)).
-00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a10: 656c 7365 2074 6573 745f 6d65 6c74 5f70  else test_melt_p
-00016a20: 6f6f 6c5f 7769 6474 682c 0a20 2020 2020  ool_width,.     
-00016a30: 2020 2020 2020 2020 2020 206d 656c 745f             melt_
-00016a40: 706f 6f6c 5f64 6570 7468 3d4d 6963 726f  pool_depth=Micro
-00016a50: 7374 7275 6374 7572 6549 6e70 7574 2e44  structureInput.D
-00016a60: 4546 4155 4c54 5f4d 454c 545f 504f 4f4c  EFAULT_MELT_POOL
-00016a70: 5f44 4550 5448 0a20 2020 2020 2020 2020  _DEPTH.         
-00016a80: 2020 2020 2020 2069 6620 2874 6573 745f         if (test_
-00016a90: 6d65 6c74 5f70 6f6f 6c5f 6465 7074 6820  melt_pool_depth 
-00016aa0: 6973 204e 6f6e 6520 6f72 206d 6174 682e  is None or math.
-00016ab0: 6973 6e61 6e28 7465 7374 5f6d 656c 745f  isnan(test_melt_
-00016ac0: 706f 6f6c 5f64 6570 7468 2929 0a20 2020  pool_depth)).   
-00016ad0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00016ae0: 6520 7465 7374 5f6d 656c 745f 706f 6f6c  e test_melt_pool
-00016af0: 5f64 6570 7468 2c0a 2020 2020 2020 2020  _depth,.        
-00016b00: 2020 2020 2020 2020 7261 6e64 6f6d 5f73          random_s
-00016b10: 6565 643d 7465 7374 5f72 616e 646f 6d5f  eed=test_random_
-00016b20: 7365 6564 2c0a 2020 2020 2020 2020 2020  seed,.          
-00016b30: 2020 2020 2020 6d61 6368 696e 653d 6d61        machine=ma
-00016b40: 6368 696e 652c 0a20 2020 2020 2020 2020  chine,.         
-00016b50: 2020 2020 2020 206d 6174 6572 6961 6c3d         material=
-00016b60: 6d61 7465 7269 616c 2c0a 2020 2020 2020  material,.      
-00016b70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00016b80: 2020 2020 7265 7475 726e 2028 5472 7565      return (True
-00016b90: 2c20 2222 290a 2020 2020 2020 2020 6578  , "").        ex
-00016ba0: 6365 7074 2056 616c 7565 4572 726f 7220  cept ValueError 
-00016bb0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00016bc0: 2020 7265 7475 726e 2028 4661 6c73 652c    return (False,
-00016bd0: 2028 6622 496e 7661 6c69 6420 7061 7261   (f"Invalid para
-00016be0: 6d65 7465 7220 636f 6d62 696e 6174 696f  meter combinatio
-00016bf0: 6e3a 207b 657d 2229 290a                 n: {e}")).
+000151f0: 6966 206e 702e 6973 6e61 6e28 696e 7075  if np.isnan(inpu
+00015200: 745b 436f 6c75 6d6e 4e61 6d65 732e 4841  t[ColumnNames.HA
+00015210: 5443 485f 5350 4143 494e 475d 293a 0a20  TCH_SPACING]):. 
+00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 2020 2069 6e70 7574 5b43 6f6c 756d 6e4e     input[ColumnN
+00015240: 616d 6573 2e48 4154 4348 5f53 5041 4349  ames.HATCH_SPACI
+00015250: 4e47 5d20 3d20 4d61 6368 696e 6543 6f6e  NG] = MachineCon
+00015260: 7374 616e 7473 2e44 4546 4155 4c54 5f48  stants.DEFAULT_H
+00015270: 4154 4348 5f53 5041 4349 4e47 0a20 2020  ATCH_SPACING.   
+00015280: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015290: 6e70 2e69 736e 616e 2869 6e70 7574 5b43  np.isnan(input[C
+000152a0: 6f6c 756d 6e4e 616d 6573 2e53 5452 4950  olumnNames.STRIP
+000152b0: 455f 5749 4454 485d 293a 0a20 2020 2020  E_WIDTH]):.     
+000152c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000152d0: 6e70 7574 5b43 6f6c 756d 6e4e 616d 6573  nput[ColumnNames
+000152e0: 2e53 5452 4950 455f 5749 4454 485d 203d  .STRIPE_WIDTH] =
+000152f0: 204d 6163 6869 6e65 436f 6e73 7461 6e74   MachineConstant
+00015300: 732e 4445 4641 554c 545f 534c 4943 494e  s.DEFAULT_SLICIN
+00015310: 475f 5354 5249 5045 5f57 4944 5448 0a0a  G_STRIPE_WIDTH..
+00015320: 2020 2020 2020 2020 2020 2020 6d61 6368              mach
+00015330: 696e 6520 3d20 4164 6469 7469 7665 4d61  ine = AdditiveMa
+00015340: 6368 696e 6528 0a20 2020 2020 2020 2020  chine(.         
+00015350: 2020 2020 2020 206c 6173 6572 5f70 6f77         laser_pow
+00015360: 6572 3d69 6e70 7574 5b43 6f6c 756d 6e4e  er=input[ColumnN
+00015370: 616d 6573 2e4c 4153 4552 5f50 4f57 4552  ames.LASER_POWER
+00015380: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00015390: 2020 2073 6361 6e5f 7370 6565 643d 696e     scan_speed=in
+000153a0: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
+000153b0: 5343 414e 5f53 5045 4544 5d2c 0a20 2020  SCAN_SPEED],.   
+000153c0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+000153d0: 7465 725f 7465 6d70 6572 6174 7572 653d  ter_temperature=
+000153e0: 696e 7075 745b 436f 6c75 6d6e 4e61 6d65  input[ColumnName
+000153f0: 732e 4845 4154 4552 5f54 454d 5045 5241  s.HEATER_TEMPERA
+00015400: 5455 5245 5d2c 0a20 2020 2020 2020 2020  TURE],.         
+00015410: 2020 2020 2020 206c 6179 6572 5f74 6869         layer_thi
+00015420: 636b 6e65 7373 3d69 6e70 7574 5b43 6f6c  ckness=input[Col
+00015430: 756d 6e4e 616d 6573 2e4c 4159 4552 5f54  umnNames.LAYER_T
+00015440: 4849 434b 4e45 5353 5d2c 0a20 2020 2020  HICKNESS],.     
+00015450: 2020 2020 2020 2020 2020 2062 6561 6d5f             beam_
+00015460: 6469 616d 6574 6572 3d69 6e70 7574 5b43  diameter=input[C
+00015470: 6f6c 756d 6e4e 616d 6573 2e42 4541 4d5f  olumnNames.BEAM_
+00015480: 4449 414d 4554 4552 5d2c 0a20 2020 2020  DIAMETER],.     
+00015490: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000154a0: 696e 675f 6c61 7965 725f 616e 676c 653d  ing_layer_angle=
+000154b0: 696e 7075 745b 436f 6c75 6d6e 4e61 6d65  input[ColumnName
+000154c0: 732e 5354 4152 545f 414e 474c 455d 2c0a  s.START_ANGLE],.
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 6c61 7965 725f 726f 7461 7469 6f6e 5f61  layer_rotation_a
+000154f0: 6e67 6c65 3d69 6e70 7574 5b43 6f6c 756d  ngle=input[Colum
+00015500: 6e4e 616d 6573 2e52 4f54 4154 494f 4e5f  nNames.ROTATION_
+00015510: 414e 474c 455d 2c0a 2020 2020 2020 2020  ANGLE],.        
+00015520: 2020 2020 2020 2020 6861 7463 685f 7370          hatch_sp
+00015530: 6163 696e 673d 696e 7075 745b 436f 6c75  acing=input[Colu
+00015540: 6d6e 4e61 6d65 732e 4841 5443 485f 5350  mnNames.HATCH_SP
+00015550: 4143 494e 475d 2c0a 2020 2020 2020 2020  ACING],.        
+00015560: 2020 2020 2020 2020 736c 6963 696e 675f          slicing_
+00015570: 7374 7269 7065 5f77 6964 7468 3d69 6e70  stripe_width=inp
+00015580: 7574 5b43 6f6c 756d 6e4e 616d 6573 2e53  ut[ColumnNames.S
+00015590: 5452 4950 455f 5749 4454 485d 2c0a 2020  TRIPE_WIDTH],.  
+000155a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000155b0: 2020 2020 2020 2020 206d 6174 6572 6961           materia
+000155c0: 6c20 3d20 4164 6469 7469 7665 4d61 7465  l = AdditiveMate
+000155d0: 7269 616c 286e 616d 653d 7374 7228 696e  rial(name=str(in
+000155e0: 7075 745b 436f 6c75 6d6e 4e61 6d65 732e  put[ColumnNames.
+000155f0: 4d41 5445 5249 414c 5d29 290a 0a20 2020  MATERIAL]))..   
+00015600: 2020 2020 2020 2020 2069 6620 696e 7075           if inpu
+00015610: 745b 436f 6c75 6d6e 4e61 6d65 732e 5459  t[ColumnNames.TY
+00015620: 5045 5d20 3d3d 2053 696d 756c 6174 696f  PE] == Simulatio
+00015630: 6e54 7970 652e 5349 4e47 4c45 5f42 4541  nType.SINGLE_BEA
+00015640: 443a 0a20 2020 2020 2020 2020 2020 2020  D:.             
+00015650: 2020 2076 616c 6964 2c20 6572 726f 7220     valid, error 
+00015660: 3d20 7365 6c66 2e5f 7661 6c69 6461 7465  = self._validate
+00015670: 5f73 696e 676c 655f 6265 6164 5f69 6e70  _single_bead_inp
+00015680: 7574 286d 6163 6869 6e65 2c20 6d61 7465  ut(machine, mate
+00015690: 7269 616c 2c20 696e 7075 7429 0a20 2020  rial, input).   
+000156a0: 2020 2020 2020 2020 2069 6620 696e 7075           if inpu
+000156b0: 745b 436f 6c75 6d6e 4e61 6d65 732e 5459  t[ColumnNames.TY
+000156c0: 5045 5d20 3d3d 2053 696d 756c 6174 696f  PE] == Simulatio
+000156d0: 6e54 7970 652e 504f 524f 5349 5459 3a0a  nType.POROSITY:.
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156f0: 7661 6c69 642c 2065 7272 6f72 203d 2073  valid, error = s
+00015700: 656c 662e 5f76 616c 6964 6174 655f 706f  elf._validate_po
+00015710: 726f 7369 7479 5f69 6e70 7574 286d 6163  rosity_input(mac
+00015720: 6869 6e65 2c20 6d61 7465 7269 616c 2c20  hine, material, 
+00015730: 696e 7075 7429 0a20 2020 2020 2020 2020  input).         
+00015740: 2020 2069 6620 696e 7075 745b 436f 6c75     if input[Colu
+00015750: 6d6e 4e61 6d65 732e 5459 5045 5d20 3d3d  mnNames.TYPE] ==
+00015760: 2053 696d 756c 6174 696f 6e54 7970 652e   SimulationType.
+00015770: 4d49 4352 4f53 5452 5543 5455 5245 3a0a  MICROSTRUCTURE:.
+00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015790: 7661 6c69 642c 2065 7272 6f72 203d 2073  valid, error = s
+000157a0: 656c 662e 5f76 616c 6964 6174 655f 6d69  elf._validate_mi
+000157b0: 6372 6f73 7472 7563 7475 7265 5f69 6e70  crostructure_inp
+000157c0: 7574 286d 6163 6869 6e65 2c20 6d61 7465  ut(machine, mate
+000157d0: 7269 616c 2c20 696e 7075 7429 0a20 2020  rial, input).   
+000157e0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000157f0: 7661 6c69 643a 0a20 2020 2020 2020 2020  valid:.         
+00015800: 2020 2020 2020 2072 6574 7572 6e20 2846         return (F
+00015810: 616c 7365 2c20 6572 726f 7229 0a20 2020  alse, error).   
+00015820: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015830: 2854 7275 652c 2022 2229 0a0a 2020 2020  (True, "")..    
+00015840: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+00015850: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+00015860: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00015870: 4661 6c73 652c 2028 6622 496e 7661 6c69  False, (f"Invali
+00015880: 6420 7061 7261 6d65 7465 7220 636f 6d62  d parameter comb
+00015890: 696e 6174 696f 6e3a 207b 657d 2229 290a  ination: {e}")).
+000158a0: 0a20 2020 2064 6566 205f 7661 6c69 6461  .    def _valida
+000158b0: 7465 5f73 696e 676c 655f 6265 6164 5f69  te_single_bead_i
+000158c0: 6e70 7574 280a 2020 2020 2020 2020 7365  nput(.        se
+000158d0: 6c66 2c20 6d61 6368 696e 653a 2041 6464  lf, machine: Add
+000158e0: 6974 6976 654d 6163 6869 6e65 2c20 6d61  itiveMachine, ma
+000158f0: 7465 7269 616c 3a20 4164 6469 7469 7665  terial: Additive
+00015900: 4d61 7465 7269 616c 2c20 696e 7075 743a  Material, input:
+00015910: 2070 642e 5365 7269 6573 0a20 2020 2029   pd.Series.    )
+00015920: 202d 3e20 7475 706c 655b 626f 6f6c 2c20   -> tuple[bool, 
+00015930: 7374 725d 3a0a 2020 2020 2020 2020 2222  str]:.        ""
+00015940: 2256 616c 6964 6174 6520 7369 6e67 6c65  "Validate single
+00015950: 2062 6561 6420 7369 6d75 6c61 7469 6f6e   bead simulation
+00015960: 2069 6e70 7574 2076 616c 7565 732e 0a0a   input values...
+00015970: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00015980: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00015990: 2d2d 2d2d 2d0a 2020 2020 2020 2020 696e  -----.        in
+000159a0: 7075 7420 3a20 7064 2e53 6572 6965 730a  put : pd.Series.
+000159b0: 2020 2020 2020 2020 2020 2020 5369 6e67              Sing
+000159c0: 6c65 2062 6561 6420 7369 6d75 6c61 7469  le bead simulati
+000159d0: 6f6e 2069 6e70 7574 2e0a 0a20 2020 2020  on input...     
+000159e0: 2020 206d 6163 6869 6e65 203a 2041 6464     machine : Add
+000159f0: 6974 6976 654d 6163 6869 6e65 0a20 2020  itiveMachine.   
+00015a00: 2020 2020 2020 2020 2041 6464 6974 6976           Additiv
+00015a10: 6520 6d61 6368 696e 6520 6f62 6a65 6374  e machine object
+00015a20: 2074 6f20 7573 6520 666f 7220 7661 6c69   to use for vali
+00015a30: 6461 7469 6e67 2074 6865 2073 696e 676c  dating the singl
+00015a40: 6520 6265 6164 2069 6e70 7574 2e0a 0a20  e bead input... 
+00015a50: 2020 2020 2020 206d 6174 6572 6961 6c20         material 
+00015a60: 3a20 4164 6469 7469 7665 4d61 7465 7269  : AdditiveMateri
+00015a70: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
+00015a80: 6464 6974 6976 6520 6d61 7465 7269 616c  dditive material
+00015a90: 206f 626a 6563 7420 746f 2075 7365 2066   object to use f
+00015aa0: 6f72 2076 616c 6964 6174 696e 6720 7468  or validating th
+00015ab0: 6520 7369 6e67 6c65 2062 6561 6420 696e  e single bead in
+00015ac0: 7075 742e 0a0a 2020 2020 2020 2020 5265  put...        Re
+00015ad0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00015ae0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7475  -----.        tu
+00015af0: 706c 655b 626f 6f6c 2c20 7374 725d 0a20  ple[bool, str]. 
+00015b00: 2020 2020 2020 2020 2020 2062 6f6f 6c2c             bool,
+00015b10: 2054 7275 6520 6966 2074 6865 2073 696e   True if the sin
+00015b20: 676c 6520 6265 6164 2069 6e70 7574 2069  gle bead input i
+00015b30: 7320 7661 6c69 642c 2046 616c 7365 206f  s valid, False o
+00015b40: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
+00015b50: 2020 2020 2020 7374 7269 6e67 2c20 4572        string, Er
+00015b60: 726f 7220 6d65 7373 6167 6520 6966 2074  ror message if t
+00015b70: 6865 2073 696e 676c 6520 6265 6164 2069  he single bead i
+00015b80: 6e70 7574 2069 7320 696e 7661 6c69 642e  nput is invalid.
+00015b90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015ba0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00015bb0: 2020 2020 2020 7465 7374 5f62 6561 645f        test_bead_
+00015bc0: 6c65 6e67 7468 203d 2069 6e70 7574 5b43  length = input[C
+00015bd0: 6f6c 756d 6e4e 616d 6573 2e53 494e 474c  olumnNames.SINGL
+00015be0: 455f 4245 4144 5f4c 454e 4754 485d 0a0a  E_BEAD_LENGTH]..
+00015bf0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+00015c00: 5f73 696e 676c 655f 6265 6164 5f69 6e70  _single_bead_inp
+00015c10: 7574 203d 2053 696e 676c 6542 6561 6449  ut = SingleBeadI
+00015c20: 6e70 7574 280a 2020 2020 2020 2020 2020  nput(.          
+00015c30: 2020 2020 2020 6265 6164 5f6c 656e 6774        bead_lengt
+00015c40: 683d 7465 7374 5f62 6561 645f 6c65 6e67  h=test_bead_leng
+00015c50: 7468 2c20 6d61 6368 696e 653d 6d61 6368  th, machine=mach
+00015c60: 696e 652c 206d 6174 6572 6961 6c3d 6d61  ine, material=ma
+00015c70: 7465 7269 616c 0a20 2020 2020 2020 2020  terial.         
+00015c80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00015c90: 2072 6574 7572 6e20 2854 7275 652c 2022   return (True, "
+00015ca0: 2229 0a20 2020 2020 2020 2065 7863 6570  ").        excep
+00015cb0: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
+00015cc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00015cd0: 6574 7572 6e20 2846 616c 7365 2c20 2866  eturn (False, (f
+00015ce0: 2249 6e76 616c 6964 2070 6172 616d 6574  "Invalid paramet
+00015cf0: 6572 2063 6f6d 6269 6e61 7469 6f6e 3a20  er combination: 
+00015d00: 7b65 7d22 2929 0a0a 2020 2020 6465 6620  {e}"))..    def 
+00015d10: 5f76 616c 6964 6174 655f 706f 726f 7369  _validate_porosi
+00015d20: 7479 5f69 6e70 7574 280a 2020 2020 2020  ty_input(.      
+00015d30: 2020 7365 6c66 2c20 6d61 6368 696e 653a    self, machine:
+00015d40: 2041 6464 6974 6976 654d 6163 6869 6e65   AdditiveMachine
+00015d50: 2c20 6d61 7465 7269 616c 3a20 4164 6469  , material: Addi
+00015d60: 7469 7665 4d61 7465 7269 616c 2c20 696e  tiveMaterial, in
+00015d70: 7075 743a 2070 642e 5365 7269 6573 0a20  put: pd.Series. 
+00015d80: 2020 2029 202d 3e20 7475 706c 655b 626f     ) -> tuple[bo
+00015d90: 6f6c 2c20 7374 725d 3a0a 2020 2020 2020  ol, str]:.      
+00015da0: 2020 2222 2256 616c 6964 6174 6520 706f    """Validate po
+00015db0: 726f 7369 7479 2073 696d 756c 6174 696f  rosity simulatio
+00015dc0: 6e20 696e 7075 7420 7661 6c75 6573 2e0a  n input values..
+00015dd0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00015de0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00015df0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
+00015e00: 6e70 7574 203a 2070 642e 5365 7269 6573  nput : pd.Series
+00015e10: 0a20 2020 2020 2020 2020 2020 2050 6f72  .            Por
+00015e20: 6f73 6974 7920 7369 6d75 6c61 7469 6f6e  osity simulation
+00015e30: 2069 6e70 7574 2e0a 0a20 2020 2020 2020   input...       
+00015e40: 206d 6163 6869 6e65 203a 2041 6464 6974   machine : Addit
+00015e50: 6976 654d 6163 6869 6e65 0a20 2020 2020  iveMachine.     
+00015e60: 2020 2020 2020 2041 6464 6974 6976 6520         Additive 
+00015e70: 6d61 6368 696e 6520 6f62 6a65 6374 2074  machine object t
+00015e80: 6f20 7573 6520 666f 7220 7661 6c69 6461  o use for valida
+00015e90: 7469 6e67 2074 6865 2070 6f72 6f73 6974  ting the porosit
+00015ea0: 7920 696e 7075 742e 0a0a 2020 2020 2020  y input...      
+00015eb0: 2020 6d61 7465 7269 616c 203a 2041 6464    material : Add
+00015ec0: 6974 6976 654d 6174 6572 6961 6c0a 2020  itiveMaterial.  
+00015ed0: 2020 2020 2020 2020 2020 4164 6469 7469            Additi
+00015ee0: 7665 206d 6174 6572 6961 6c20 6f62 6a65  ve material obje
+00015ef0: 6374 2074 6f20 7573 6520 666f 7220 7661  ct to use for va
+00015f00: 6c69 6461 7469 6e67 2074 6865 2070 6f72  lidating the por
+00015f10: 6f73 6974 7920 696e 7075 742e 0a0a 2020  osity input...  
+00015f20: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00015f30: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00015f40: 2020 2020 2020 7475 706c 655b 626f 6f6c        tuple[bool
+00015f50: 2c20 7374 725d 0a20 2020 2020 2020 2020  , str].         
+00015f60: 2020 2062 6f6f 6c2c 2054 7275 6520 6966     bool, True if
+00015f70: 2074 6865 2070 6f72 6f73 6974 7920 696e   the porosity in
+00015f80: 7075 7420 6973 2076 616c 6964 2c20 4661  put is valid, Fa
+00015f90: 6c73 6520 6f74 6865 7277 6973 652e 0a20  lse otherwise.. 
+00015fa0: 2020 2020 2020 2020 2020 2073 7472 696e             strin
+00015fb0: 672c 2045 7272 6f72 206d 6573 7361 6765  g, Error message
+00015fc0: 2069 6620 7468 6520 706f 726f 7369 7479   if the porosity
+00015fd0: 2069 6e70 7574 2069 7320 696e 7661 6c69   input is invali
+00015fe0: 642e 0a20 2020 2020 2020 2022 2222 0a0a  d..        """..
+00015ff0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00016000: 2020 2020 2020 2020 2074 6573 745f 706f           test_po
+00016010: 726f 7369 7479 5f69 6e70 7574 203d 2050  rosity_input = P
+00016020: 6f72 6f73 6974 7949 6e70 7574 280a 2020  orosityInput(.  
+00016030: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00016040: 7a65 5f78 3d69 6e70 7574 5b43 6f6c 756d  ze_x=input[Colum
+00016050: 6e4e 616d 6573 2e50 4f52 4f53 4954 595f  nNames.POROSITY_
+00016060: 5349 5a45 5f58 5d2c 0a20 2020 2020 2020  SIZE_X],.       
+00016070: 2020 2020 2020 2020 2073 697a 655f 793d           size_y=
+00016080: 696e 7075 745b 436f 6c75 6d6e 4e61 6d65  input[ColumnName
+00016090: 732e 504f 524f 5349 5459 5f53 495a 455f  s.POROSITY_SIZE_
+000160a0: 595d 2c0a 2020 2020 2020 2020 2020 2020  Y],.            
+000160b0: 2020 2020 7369 7a65 5f7a 3d69 6e70 7574      size_z=input
+000160c0: 5b43 6f6c 756d 6e4e 616d 6573 2e50 4f52  [ColumnNames.POR
+000160d0: 4f53 4954 595f 5349 5a45 5f5a 5d2c 0a20  OSITY_SIZE_Z],. 
+000160e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000160f0: 6163 6869 6e65 3d6d 6163 6869 6e65 2c0a  achine=machine,.
+00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016110: 6d61 7465 7269 616c 3d6d 6174 6572 6961  material=materia
+00016120: 6c2c 0a20 2020 2020 2020 2020 2020 2029  l,.            )
+00016130: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00016140: 7572 6e20 2854 7275 652c 2022 2229 0a20  urn (True, ""). 
+00016150: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+00016160: 6c75 6545 7272 6f72 2061 7320 653a 0a20  lueError as e:. 
+00016170: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016180: 6e20 2846 616c 7365 2c20 2866 2249 6e76  n (False, (f"Inv
+00016190: 616c 6964 2070 6172 616d 6574 6572 2063  alid parameter c
+000161a0: 6f6d 6269 6e61 7469 6f6e 3a20 7b65 7d22  ombination: {e}"
+000161b0: 2929 0a0a 2020 2020 6465 6620 5f76 616c  ))..    def _val
+000161c0: 6964 6174 655f 6d69 6372 6f73 7472 7563  idate_microstruc
+000161d0: 7475 7265 5f69 6e70 7574 280a 2020 2020  ture_input(.    
+000161e0: 2020 2020 7365 6c66 2c20 6d61 6368 696e      self, machin
+000161f0: 653a 2041 6464 6974 6976 654d 6163 6869  e: AdditiveMachi
+00016200: 6e65 2c20 6d61 7465 7269 616c 3a20 4164  ne, material: Ad
+00016210: 6469 7469 7665 4d61 7465 7269 616c 2c20  ditiveMaterial, 
+00016220: 696e 7075 743a 2070 642e 5365 7269 6573  input: pd.Series
+00016230: 0a20 2020 2029 202d 3e20 7475 706c 655b  .    ) -> tuple[
+00016240: 626f 6f6c 2c20 7374 725d 3a0a 2020 2020  bool, str]:.    
+00016250: 2020 2020 2222 2256 616c 6964 6174 6520      """Validate 
+00016260: 6d69 6372 6f73 7472 7563 7475 7265 2073  microstructure s
+00016270: 696d 756c 6174 696f 6e20 696e 7075 7420  imulation input 
+00016280: 7661 6c75 6573 2e0a 0a20 2020 2020 2020  values...       
+00016290: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000162a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000162b0: 2020 2020 2020 2069 6e70 7574 203a 2070         input : p
+000162c0: 642e 5365 7269 6573 0a20 2020 2020 2020  d.Series.       
+000162d0: 2020 2020 204d 6963 726f 7374 7275 6374       Microstruct
+000162e0: 7572 6520 7369 6d75 6c61 7469 6f6e 2069  ure simulation i
+000162f0: 6e70 7574 2e0a 0a20 2020 2020 2020 206d  nput...        m
+00016300: 6163 6869 6e65 203a 2041 6464 6974 6976  achine : Additiv
+00016310: 654d 6163 6869 6e65 0a20 2020 2020 2020  eMachine.       
+00016320: 2020 2020 2041 6464 6974 6976 6520 6d61       Additive ma
+00016330: 6368 696e 6520 6f62 6a65 6374 2074 6f20  chine object to 
+00016340: 7573 6520 666f 7220 7661 6c69 6461 7469  use for validati
+00016350: 6e67 2074 6865 206d 6963 726f 7374 7275  ng the microstru
+00016360: 6374 7572 6520 696e 7075 742e 0a0a 2020  cture input...  
+00016370: 2020 2020 2020 6d61 7465 7269 616c 203a        material :
+00016380: 2041 6464 6974 6976 654d 6174 6572 6961   AdditiveMateria
+00016390: 6c0a 2020 2020 2020 2020 2020 2020 4164  l.            Ad
+000163a0: 6469 7469 7665 206d 6174 6572 6961 6c20  ditive material 
+000163b0: 6f62 6a65 6374 2074 6f20 7573 6520 666f  object to use fo
+000163c0: 7220 7661 6c69 6461 7469 6e67 2074 6865  r validating the
+000163d0: 206d 6963 726f 7374 7275 6374 7572 6520   microstructure 
+000163e0: 696e 7075 742e 0a0a 2020 2020 2020 2020  input...        
+000163f0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00016400: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016410: 7475 706c 655b 626f 6f6c 2c20 7374 725d  tuple[bool, str]
+00016420: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
+00016430: 6c2c 2054 7275 6520 6966 2074 6865 206d  l, True if the m
+00016440: 6963 726f 7374 7275 6374 7572 6520 696e  icrostructure in
+00016450: 7075 7420 6973 2076 616c 6964 2c20 4661  put is valid, Fa
+00016460: 6c73 6520 6f74 6865 7277 6973 652e 0a20  lse otherwise.. 
+00016470: 2020 2020 2020 2020 2020 2073 7472 696e             strin
+00016480: 672c 2045 7272 6f72 206d 6573 7361 6765  g, Error message
+00016490: 2069 6620 7468 6520 6d69 6372 6f73 7472   if the microstr
+000164a0: 7563 7475 7265 2069 6e70 7574 2069 7320  ucture input is 
+000164b0: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
+000164c0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
+000164d0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+000164e0: 7374 5f63 6f6f 6c69 6e67 5f72 6174 6520  st_cooling_rate 
+000164f0: 3d20 696e 7075 745b 436f 6c75 6d6e 4e61  = input[ColumnNa
+00016500: 6d65 732e 434f 4f4c 494e 475f 5241 5445  mes.COOLING_RATE
+00016510: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+00016520: 7374 5f74 6865 726d 616c 5f67 7261 6469  st_thermal_gradi
+00016530: 656e 7420 3d20 696e 7075 745b 436f 6c75  ent = input[Colu
+00016540: 6d6e 4e61 6d65 732e 5448 4552 4d41 4c5f  mnNames.THERMAL_
+00016550: 4752 4144 4945 4e54 5d0a 2020 2020 2020  GRADIENT].      
+00016560: 2020 2020 2020 7465 7374 5f6d 656c 745f        test_melt_
+00016570: 706f 6f6c 5f77 6964 7468 203d 2069 6e70  pool_width = inp
+00016580: 7574 5b43 6f6c 756d 6e4e 616d 6573 2e4d  ut[ColumnNames.M
+00016590: 4943 524f 5f4d 454c 545f 504f 4f4c 5f57  ICRO_MELT_POOL_W
+000165a0: 4944 5448 5d0a 2020 2020 2020 2020 2020  IDTH].          
+000165b0: 2020 7465 7374 5f6d 656c 745f 706f 6f6c    test_melt_pool
+000165c0: 5f64 6570 7468 203d 2069 6e70 7574 5b43  _depth = input[C
+000165d0: 6f6c 756d 6e4e 616d 6573 2e4d 4943 524f  olumnNames.MICRO
+000165e0: 5f4d 454c 545f 504f 4f4c 5f44 4550 5448  _MELT_POOL_DEPTH
+000165f0: 5d0a 2020 2020 2020 2020 2020 2020 7465  ].            te
+00016600: 7374 5f72 616e 646f 6d5f 7365 6564 203d  st_random_seed =
+00016610: 2069 6e70 7574 5b43 6f6c 756d 6e4e 616d   input[ColumnNam
+00016620: 6573 2e52 414e 444f 4d5f 5345 4544 5d0a  es.RANDOM_SEED].
+00016630: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016640: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00016650: 2020 6d61 7468 2e69 736e 616e 2874 6573    math.isnan(tes
+00016660: 745f 636f 6f6c 696e 675f 7261 7465 290a  t_cooling_rate).
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 6f72 206d 6174 682e 6973 6e61 6e28 7465  or math.isnan(te
+00016690: 7374 5f74 6865 726d 616c 5f67 7261 6469  st_thermal_gradi
+000166a0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+000166b0: 2020 2020 206f 7220 6d61 7468 2e69 736e       or math.isn
+000166c0: 616e 2874 6573 745f 6d65 6c74 5f70 6f6f  an(test_melt_poo
+000166d0: 6c5f 7769 6474 6829 0a20 2020 2020 2020  l_width).       
+000166e0: 2020 2020 2020 2020 206f 7220 6d61 7468           or math
+000166f0: 2e69 736e 616e 2874 6573 745f 6d65 6c74  .isnan(test_melt
+00016700: 5f70 6f6f 6c5f 6465 7074 6829 0a20 2020  _pool_depth).   
+00016710: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00016720: 2020 2020 2020 2020 2020 2020 7465 7374              test
+00016730: 5f75 7365 5f70 726f 7669 6465 645f 7468  _use_provided_th
+00016740: 6572 6d61 6c5f 7061 7261 6d65 7465 7273  ermal_parameters
+00016750: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00016760: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016770: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00016780: 7573 655f 7072 6f76 6964 6564 5f74 6865  use_provided_the
+00016790: 726d 616c 5f70 6172 616d 6574 6572 7320  rmal_parameters 
+000167a0: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
+000167b0: 2020 2020 7465 7374 5f6d 6963 726f 7374      test_microst
+000167c0: 7275 6374 7572 655f 696e 7075 7420 3d20  ructure_input = 
+000167d0: 4d69 6372 6f73 7472 7563 7475 7265 496e  MicrostructureIn
+000167e0: 7075 7428 0a20 2020 2020 2020 2020 2020  put(.           
+000167f0: 2020 2020 2073 616d 706c 655f 6d69 6e5f       sample_min_
+00016800: 783d 696e 7075 745b 436f 6c75 6d6e 4e61  x=input[ColumnNa
+00016810: 6d65 732e 4d49 4352 4f5f 4d49 4e5f 585d  mes.MICRO_MIN_X]
+00016820: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016830: 2020 7361 6d70 6c65 5f6d 696e 5f79 3d69    sample_min_y=i
+00016840: 6e70 7574 5b43 6f6c 756d 6e4e 616d 6573  nput[ColumnNames
+00016850: 2e4d 4943 524f 5f4d 494e 5f59 5d2c 0a20  .MICRO_MIN_Y],. 
+00016860: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016870: 616d 706c 655f 6d69 6e5f 7a3d 696e 7075  ample_min_z=inpu
+00016880: 745b 436f 6c75 6d6e 4e61 6d65 732e 4d49  t[ColumnNames.MI
+00016890: 4352 4f5f 4d49 4e5f 5a5d 2c0a 2020 2020  CRO_MIN_Z],.    
+000168a0: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+000168b0: 6c65 5f73 697a 655f 783d 696e 7075 745b  le_size_x=input[
+000168c0: 436f 6c75 6d6e 4e61 6d65 732e 4d49 4352  ColumnNames.MICR
+000168d0: 4f5f 5349 5a45 5f58 5d2c 0a20 2020 2020  O_SIZE_X],.     
+000168e0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
+000168f0: 655f 7369 7a65 5f79 3d69 6e70 7574 5b43  e_size_y=input[C
+00016900: 6f6c 756d 6e4e 616d 6573 2e4d 4943 524f  olumnNames.MICRO
+00016910: 5f53 495a 455f 595d 2c0a 2020 2020 2020  _SIZE_Y],.      
+00016920: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+00016930: 5f73 697a 655f 7a3d 696e 7075 745b 436f  _size_z=input[Co
+00016940: 6c75 6d6e 4e61 6d65 732e 4d49 4352 4f5f  lumnNames.MICRO_
+00016950: 5349 5a45 5f5a 5d2c 0a20 2020 2020 2020  SIZE_Z],.       
+00016960: 2020 2020 2020 2020 2073 656e 736f 725f           sensor_
+00016970: 6469 6d65 6e73 696f 6e3d 696e 7075 745b  dimension=input[
+00016980: 436f 6c75 6d6e 4e61 6d65 732e 4d49 4352  ColumnNames.MICR
+00016990: 4f5f 5345 4e53 4f52 5f44 494d 5d2c 0a20  O_SENSOR_DIM],. 
+000169a0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000169b0: 7365 5f70 726f 7669 6465 645f 7468 6572  se_provided_ther
+000169c0: 6d61 6c5f 7061 7261 6d65 7465 7273 3d74  mal_parameters=t
+000169d0: 6573 745f 7573 655f 7072 6f76 6964 6564  est_use_provided
+000169e0: 5f74 6865 726d 616c 5f70 6172 616d 6574  _thermal_paramet
+000169f0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+00016a00: 2020 2020 2063 6f6f 6c69 6e67 5f72 6174       cooling_rat
+00016a10: 653d 4d69 6372 6f73 7472 7563 7475 7265  e=Microstructure
+00016a20: 496e 7075 742e 4445 4641 554c 545f 434f  Input.DEFAULT_CO
+00016a30: 4f4c 494e 475f 5241 5445 0a20 2020 2020  OLING_RATE.     
+00016a40: 2020 2020 2020 2020 2020 2069 6620 2874             if (t
+00016a50: 6573 745f 636f 6f6c 696e 675f 7261 7465  est_cooling_rate
+00016a60: 2069 7320 4e6f 6e65 206f 7220 6d61 7468   is None or math
+00016a70: 2e69 736e 616e 2874 6573 745f 636f 6f6c  .isnan(test_cool
+00016a80: 696e 675f 7261 7465 2929 0a20 2020 2020  ing_rate)).     
+00016a90: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00016aa0: 7465 7374 5f63 6f6f 6c69 6e67 5f72 6174  test_cooling_rat
+00016ab0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00016ac0: 2020 2074 6865 726d 616c 5f67 7261 6469     thermal_gradi
+00016ad0: 656e 743d 4d69 6372 6f73 7472 7563 7475  ent=Microstructu
+00016ae0: 7265 496e 7075 742e 4445 4641 554c 545f  reInput.DEFAULT_
+00016af0: 5448 4552 4d41 4c5f 4752 4144 4945 4e54  THERMAL_GRADIENT
+00016b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b10: 2069 6620 2874 6573 745f 7468 6572 6d61   if (test_therma
+00016b20: 6c5f 6772 6164 6965 6e74 2069 7320 4e6f  l_gradient is No
+00016b30: 6e65 206f 7220 6d61 7468 2e69 736e 616e  ne or math.isnan
+00016b40: 2874 6573 745f 7468 6572 6d61 6c5f 6772  (test_thermal_gr
+00016b50: 6164 6965 6e74 2929 0a20 2020 2020 2020  adient)).       
+00016b60: 2020 2020 2020 2020 2065 6c73 6520 7465           else te
+00016b70: 7374 5f74 6865 726d 616c 5f67 7261 6469  st_thermal_gradi
+00016b80: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
+00016b90: 2020 2020 206d 656c 745f 706f 6f6c 5f77       melt_pool_w
+00016ba0: 6964 7468 3d4d 6963 726f 7374 7275 6374  idth=Microstruct
+00016bb0: 7572 6549 6e70 7574 2e44 4546 4155 4c54  ureInput.DEFAULT
+00016bc0: 5f4d 454c 545f 504f 4f4c 5f57 4944 5448  _MELT_POOL_WIDTH
+00016bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016be0: 2069 6620 2874 6573 745f 6d65 6c74 5f70   if (test_melt_p
+00016bf0: 6f6f 6c5f 7769 6474 6820 6973 204e 6f6e  ool_width is Non
+00016c00: 6520 6f72 206d 6174 682e 6973 6e61 6e28  e or math.isnan(
+00016c10: 7465 7374 5f6d 656c 745f 706f 6f6c 5f77  test_melt_pool_w
+00016c20: 6964 7468 2929 0a20 2020 2020 2020 2020  idth)).         
+00016c30: 2020 2020 2020 2065 6c73 6520 7465 7374         else test
+00016c40: 5f6d 656c 745f 706f 6f6c 5f77 6964 7468  _melt_pool_width
+00016c50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016c60: 2020 6d65 6c74 5f70 6f6f 6c5f 6465 7074    melt_pool_dept
+00016c70: 683d 4d69 6372 6f73 7472 7563 7475 7265  h=Microstructure
+00016c80: 496e 7075 742e 4445 4641 554c 545f 4d45  Input.DEFAULT_ME
+00016c90: 4c54 5f50 4f4f 4c5f 4445 5054 480a 2020  LT_POOL_DEPTH.  
+00016ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016cb0: 2028 7465 7374 5f6d 656c 745f 706f 6f6c   (test_melt_pool
+00016cc0: 5f64 6570 7468 2069 7320 4e6f 6e65 206f  _depth is None o
+00016cd0: 7220 6d61 7468 2e69 736e 616e 2874 6573  r math.isnan(tes
+00016ce0: 745f 6d65 6c74 5f70 6f6f 6c5f 6465 7074  t_melt_pool_dept
+00016cf0: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+00016d00: 2020 2020 656c 7365 2074 6573 745f 6d65      else test_me
+00016d10: 6c74 5f70 6f6f 6c5f 6465 7074 682c 0a20  lt_pool_depth,. 
+00016d20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016d30: 616e 646f 6d5f 7365 6564 3d74 6573 745f  andom_seed=test_
+00016d40: 7261 6e64 6f6d 5f73 6565 642c 0a20 2020  random_seed,.   
+00016d50: 2020 2020 2020 2020 2020 2020 206d 6163               mac
+00016d60: 6869 6e65 3d6d 6163 6869 6e65 2c0a 2020  hine=machine,.  
+00016d70: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00016d80: 7465 7269 616c 3d6d 6174 6572 6961 6c2c  terial=material,
+00016d90: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00016da0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016db0: 6e20 2854 7275 652c 2022 2229 0a20 2020  n (True, "").   
+00016dc0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00016dd0: 6545 7272 6f72 2061 7320 653a 0a20 2020  eError as e:.   
+00016de0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016df0: 2846 616c 7365 2c20 2866 2249 6e76 616c  (False, (f"Inval
+00016e00: 6964 2070 6172 616d 6574 6572 2063 6f6d  id parameter com
+00016e10: 6269 6e61 7469 6f6e 3a20 7b65 7d22 2929  bination: {e}"))
+00016e20: 0a                                       .
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/parametric_study/parametric_utils.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/parametric_study/parametric_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/porosity.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/porosity.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/progress_handler.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/progress_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/__init__.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/local_server.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/local_server.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/network_utils.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/network_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/server_connection/server_connection.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/server_connection/server_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     @property
     def channel_str(self) -> str:
         """GRPC channel target.
 
         The form is generally ``"ip:port"``. For example, ``"127.0.0.1:50052"``.
         """
         if self._channel is not None:
-            return self._channel._channel.target().decode()
+            return self._channel._channel.target().decode().removeprefix("dns:///")
         return ""
 
     @property
     def materials_stub(self) -> MaterialsServiceStub:
         """Materials service stub."""
         return self._materials_stub
```

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/simulation.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/simulation.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/single_bead.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/single_bead.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/src/ansys/additive/core/thermal_history.py` & `ansys_additive_core-0.18.0b5/src/ansys/additive/core/thermal_history.py`

 * *Files identical despite different names*

### Comparing `ansys_additive_core-0.18.0b4/PKG-INFO` & `ansys_additive_core-0.18.0b5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-additive-core
-Version: 0.18.0b4
+Version: 0.18.0b5
 Summary: A Python client for the Ansys Additive service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Manufacturing
@@ -21,33 +21,28 @@
 Requires-Dist: google-api-python-client>=1.7.11
 Requires-Dist: googleapis-common-protos>=1.52.0
 Requires-Dist: grpcio>=1.35.0
 Requires-Dist: grpcio-health-checking>=1.45.0
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: pandas>=1.3.2
-Requires-Dist: panel>=1.2.1
 Requires-Dist: platformdirs>=3.8.0
-Requires-Dist: plotly>=5.16.1
 Requires-Dist: protobuf>=3.20.2,<5
 Requires-Dist: six>=1.16.0
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: pydantic>=2.6.3
-Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
 Requires-Dist: enum-tools==0.12.0 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.8.4 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
-Requires-Dist: panel==1.4.2 ; extra == "doc"
 Requires-Dist: phantomjs==1.4.1 ; extra == "doc"
 Requires-Dist: pypandoc==1.13 ; extra == "doc"
-Requires-Dist: pyvista==0.43.6 ; extra == "doc"
-Requires-Dist: selenium==4.20.0 ; extra == "doc"
+Requires-Dist: pyvista==0.43.7 ; extra == "doc"
 Requires-Dist: sphinx==7.3.7 ; extra == "doc"
-Requires-Dist: sphinx-autoapi==3.0.0 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==2.1.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-design==0.5.0 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.16.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==1.0.0 ; extra == "doc"
 Requires-Dist: sphinx-toolbox==3.5.0 ; extra == "doc"
@@ -56,20 +51,18 @@
 Requires-Dist: dill==0.3.8 ; extra == "tests"
 Requires-Dist: google-api-python-client==2.122.0 ; extra == "tests"
 Requires-Dist: googleapis-common-protos==1.63.0 ; extra == "tests"
 Requires-Dist: grpcio==1.60.0 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.48.2 ; extra == "tests"
 Requires-Dist: numpy==1.26.4 ; extra == "tests"
 Requires-Dist: pandas==2.2.2 ; extra == "tests"
-Requires-Dist: panel==1.4.2 ; extra == "tests"
 Requires-Dist: platformdirs==4.2.1 ; extra == "tests"
-Requires-Dist: plotly==5.21.0 ; extra == "tests"
 Requires-Dist: protobuf==4.25.3 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
-Requires-Dist: tqdm==4.66.2 ; extra == "tests"
+Requires-Dist: tqdm==4.66.4 ; extra == "tests"
 Requires-Dist: pydantic==2.7.1 ; extra == "tests"
 Requires-Dist: pytest==8.2.0 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Discussions, https://github.com/ansys/pyadditive/discussions
 Project-URL: Documentation, https://additive.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyadditive/issues
 Project-URL: Releases, https://github.com/ansys/pyadditive/releases
```

