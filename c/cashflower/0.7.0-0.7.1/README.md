# Comparing `tmp/cashflower-0.7.0.tar.gz` & `tmp/cashflower-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.7.0.tar", last modified: Thu Dec  7 17:07:58 2023, max compression
+gzip compressed data, was "cashflower-0.7.1.tar", last modified: Wed May 15 07:56:38 2024, max compression
```

## Comparing `cashflower-0.7.0.tar` & `cashflower-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:58.935013 cashflower-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-07 17:07:52.000000 cashflower-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-07 17:07:52.000000 cashflower-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-12-07 17:07:58.935013 cashflower-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-07 17:07:52.000000 cashflower-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:58.935013 cashflower-0.7.0/cashflower/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21810 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:58.935013 cashflower-0.7.0/cashflower/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   400151 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower/cython/discount.c
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/cython/discount.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:58.935013 cashflower-0.7.0/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/model_tpl/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/model_tpl/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-12-07 17:07:52.000000 cashflower-0.7.0/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 17:07:58.935013 cashflower-0.7.0/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-07 17:07:58.000000 cashflower-0.7.0/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-07 17:07:52.000000 cashflower-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 17:07:58.935013 cashflower-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-12-07 17:07:52.000000 cashflower-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:38.113207 cashflower-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-15 07:56:31.000000 cashflower-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 07:56:31.000000 cashflower-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-15 07:56:38.109207 cashflower-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-15 07:56:31.000000 cashflower-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:38.109207 cashflower-0.7.1/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:38.109207 cashflower-0.7.1/cashflower/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   400319 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower/cython/discount.c
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/cython/discount.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:38.109207 cashflower-0.7.1/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/model_tpl/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/model_tpl/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-15 07:56:31.000000 cashflower-0.7.1/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:56:38.109207 cashflower-0.7.1/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 07:56:38.000000 cashflower-0.7.1/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 07:56:31.000000 cashflower-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:56:38.113207 cashflower-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-15 07:56:31.000000 cashflower-0.7.1/setup.py
```

### Comparing `cashflower-0.7.0/LICENSE` & `cashflower-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.7.0/PKG-INFO` & `cashflower-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.7.0
+Version: 0.7.1
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 License: UNKNOWN
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
@@ -34,14 +34,15 @@
 ```
 pip install cashflower
 ```
 
 ## Create model
 
 *python console*
+
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
 Creates:
```

### Comparing `cashflower-0.7.0/README.md` & `cashflower-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ```
 pip install cashflower
 ```
 
 ## Create model
 
 *python console*
+
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
 Creates:
```

### Comparing `cashflower-0.7.0/cashflower/core.py` & `cashflower-0.7.1/cashflower/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,84 @@
 import time
 import multiprocessing
 import numpy as np
 import pandas as pd
 import psutil
 
 from .error import CashflowModelError
-from .utils import get_first_indexes, get_object_by_name, print_log, split_to_ranges, updt
+from .utils import get_first_indexes, get_object_by_name, log_message, split_to_ranges, update_progressbar
 
 
 def get_variable_type(v):
+    """
+    Returns the type of the given variable.
+
+    Args:
+        v (object): The variable to check.
+
+    Returns:
+        str: The type of the variable. Possible values are "constant", "array", "stochastic", and "default".
+    """
     if isinstance(v, ConstantVariable):
         return "constant"
     elif isinstance(v, ArrayVariable):
         return "array"
     elif isinstance(v, StochasticVariable):
         return "stochastic"
     else:
         return "default"
 
 
 def check_arguments(func, array):
-    """Check if variable definition has correct argument(s): def my_var(...)"""
-    # Variable has maximally 2 parameters ("t" and "stoch")
+    """
+    Check if the input function has the correct arguments.
+
+    The function should have at most two parameters, 't' and 'stoch'. If the function has two parameters,
+    the first one should be named 't' and the second one should be named 'stoch'.
+    If the function has only one parameter, it should be named 't'. Additionally, if the input 'array' is True,
+    the function should not have any parameters.
+
+    Parameters:
+        func (function): The function to check.
+        array (bool): Whether the function is an array variable.
+
+    Raises:
+        CashflowModelError: If the function does not meet the required criteria.
+    """
+    # Variable has at most 2 parameters ("t" and "stoch")
     if func.__code__.co_argcount > 2:
         msg = f"Error in '{func.__name__}': The model variable should have at most two parameters ('t' and 'stoch')."
         raise CashflowModelError(msg)
 
-    # First parameter must be named "t" and second "stoch"
+    # The first parameter must be named "t" and second "stoch"
     if func.__code__.co_argcount == 2:
         if not func.__code__.co_varnames[0] == 't':
             msg = f"Error in '{func.__name__}': The first parameter should be named 't'."
             raise CashflowModelError(msg)
 
         if not func.__code__.co_varnames[1] == 'stoch':
             msg = f"Error in '{func.__name__}': The second parameter should be named 'stoch'."
             raise CashflowModelError(msg)
 
-    # Only parameter must be named "t"
+    # The only parameter must be named "t"
     if func.__code__.co_argcount == 1:
         if not func.__code__.co_varnames[0] == 't':
             msg = f"Error in '{func.__name__}': The parameter should be named 't'."
             raise CashflowModelError(msg)
 
-    # Array variables don't have parameters
+    # Array variables should not have any parameters
     if array and not func.__code__.co_argcount == 0:
         msg = f"Error in '{func.__name__}': Array variables cannot have parameters."
         raise CashflowModelError(msg)
 
     return None
 
 
 def variable(array=False, aggregation_type="sum"):
-    """Transform a function with decorator into an object of class Variable"""
+    """A decorator that transforms a function into an object of class Variable."""
     def wrapper(func):
         check_arguments(func, array)
 
         # Create a variable
         if array:
             v = ArrayVariable(func, aggregation_type)
         elif func.__code__.co_argcount == 0:
@@ -67,19 +90,31 @@
             v = Variable(func, aggregation_type)
 
         return v
     return wrapper
 
 
 class Variable:
-    """Default variable type.
+    """
+    Represents a variable in a cashflow model.
 
     @variable()
     def my_var(t):
         ...
+
+    Attributes:
+        func (function): The function that calculates the variable's value.
+        aggregation_type (str): The type of aggregation to apply to the variable's values.
+        name (str): The name of the variable.
+        calc_direction (int): The direction of calculation (0: normal, 1: forward, -1: backward).
+        calc_order (int): The order in which the variable is calculated.
+        cycle (bool): Whether the variable is part of a cycle.
+        cycle_order (int): The order of the variable in its cycle.
+        result (list): The calculated values of the variable.
+        runtime (float): The time it took to calculate the variable's values.
     """
     def __init__(self, func, aggregation_type):
         self.func = func
         self.aggregation_type = aggregation_type
         self.name = None
         self.calc_direction = None
         self.calc_order = None
@@ -87,23 +122,29 @@
         self.cycle_order = 0
         self.result = None
         self.runtime = 0.0
 
     def __repr__(self):
         return f"V: {self.func.__name__}"
 
+    def __lt__(self, other):
+        return self.name < other.name
+
     def __call__(self, t=None):
         if t is None:
             return self.result
 
+        # Python allows negative indexing, which would wrap around to the end of the list.
+        # To prevent this and ensure t is within the valid range, we explicitly check for t < 0.
         if t < 0:
             msg = (f"\n\nVariable '{self.name}' has been called for period '{t}' "
                    f"which is outside of the calculation range.")
             raise CashflowModelError(msg)
 
+        # Easier to ask forgiveness
         try:
             return self.result[t]
         except IndexError as e:
             if t > len(self.result):
                 msg = (f"\n\nVariable '{self.name}' has been called for period '{t}' "
                        f"which is outside of the calculation range.")
                 raise CashflowModelError(msg)
@@ -113,15 +154,15 @@
     def calculate_t(self, t):
         """For cycle calculations"""
         self.result[t] = self.func(t)
 
     def calculate(self):
         t_max = len(self.result)
         if self.calc_direction == 0:
-            self.result = np.array([*map(self.func, range(t_max))], dtype=np.float64)
+            self.result = np.array([self.func(t) for t in range(t_max)], dtype=np.float64)
         elif self.calc_direction == 1:
             for t in range(t_max):
                 self.result[t] = self.func(t)
         elif self.calc_direction == -1:
             for t in range(t_max-1, -1, -1):
                 self.result[t] = self.func(t)
         else:
@@ -186,32 +227,32 @@
 
     def __call__(self, t, stoch):
         return self.result_stoch[stoch-1, t]
 
     def calculate_t(self, t):
         """For cycle calculations"""
         stoch_scenarios_count = self.result_stoch.shape[0]
-        for stoch in range(1, stoch_scenarios_count+1):
-            self.result_stoch[stoch-1, t] = self.func(t, stoch)
+        stoch_range = np.arange(1, stoch_scenarios_count + 1)
+        self.result_stoch[:, t] = self.func(t, stoch_range)
 
     def calculate(self):
         stoch_scenarios_count, t_max = self.result_stoch.shape
 
-        for stoch in range(1, stoch_scenarios_count+1):
-            if self.calc_direction == 0:
+        if self.calc_direction == 0:
+            for stoch in range(1, stoch_scenarios_count + 1):
                 func_with_stoch = functools.partial(self.func, stoch=stoch)
-                self.result_stoch[stoch-1, :] = np.array([*map(func_with_stoch, range(t_max))], dtype=np.float64)
-            elif self.calc_direction == 1:
-                for t in range(t_max):
-                    self.result_stoch[stoch-1, t] = self.func(t, stoch)
-            elif self.calc_direction == -1:
-                for t in range(t_max-1, -1, -1):
-                    self.result_stoch[stoch-1, t] = self.func(t, stoch)
-            else:
-                raise CashflowModelError(f"\n\nIncorrect calculation direction '{self.calc_direction}'.")
+                self.result_stoch[stoch-1, :] = np.array([func_with_stoch(t) for t in range(t_max)], dtype=np.float64)
+        elif self.calc_direction == 1:
+            for t in range(t_max):
+                self.result_stoch[:, t] = [self.func(t, stoch) for stoch in range(1, stoch_scenarios_count + 1)]
+        elif self.calc_direction == -1:
+            for t in range(t_max-1, -1, -1):
+                self.result_stoch[:, t] = [self.func(t, stoch) for stoch in range(1, stoch_scenarios_count + 1)]
+        else:
+            raise CashflowModelError(f"\n\nIncorrect calculation direction '{self.calc_direction}'.")
 
     def average_result_stoch(self):
         self.result = np.mean(self.result_stoch, axis=0)
 
 
 class Runplan:
     """Runplan of the cash flow model.
@@ -251,23 +292,22 @@
 
         # Version must be unique
         if not self.data["version"].is_unique:
             msg = "Runplan must have unique values in the 'version' column."
             raise CashflowModelError(msg)
 
     def set_index(self, version):
-        """Version in original form stays as a column, version as a string becomes an index."""
-        self.data["version_duplicate"] = self.data["version"]
-        self.data["version"] = self.data["version"].astype(str)
-        self.data = self.data.set_index("version")
-        self.data["version"] = self.data["version_duplicate"]
-        self.data = self.data.drop(columns=["version_duplicate"])
-        if version is None:  # user has not specified version
+        # Converts the 'version' column to string and sets it as the index,
+        # while keeping the original 'version' column intact.
+        self.data = self.data.set_index(self.data["version"].astype(str))
+
+        # Set version (first one if not chosen by the user)
+        if version is None:
             self.version = str(self.data["version"].iloc[0])
-        else:  # user has specified version
+        else:
             self.version = str(version)
 
 
 class ModelPointSet:
     """Set of model points."""
 
     def __init__(self, data, name=None, settings=None):
@@ -279,204 +319,278 @@
 
     def __repr__(self):
         return f"MPS: {self.name}"
 
     def __len__(self):
         return self.data.shape[0]
 
+    def initialize(self):
+        """Additional initialization (beyond __init__) is required
+        since 'name' and 'settings' are not available during object creation."""
+        self.perform_checks()
+        self.set_index()
+        self.id = self.data.iloc[0][self.settings["ID_COLUMN"]]
+
     @functools.lru_cache()
     def get(self, attribute, record_num=0):
-        # Model point sets other than main may not have rows for all IDs
+        # Note: Only the 'main' model point set is guaranteed to have all IDs;
+        # other model point sets may not have rows for every ID
         if self.id is None:
             return None
 
         return self.model_point_data.iloc[record_num][attribute]
 
     @property
     def id(self):
-        """Current model point's id."""
+        """Get the current model point's ID."""
         return self._id
 
     @id.setter
     def id(self, new_id):
-        """Set model point's id and corresponding attributes."""
+        """Set the model point's ID and update corresponding attributes."""
         new_id = str(new_id)
         if new_id in self.data.index:
             self._id = new_id
             self.model_point_data = self.data.loc[[new_id]]
         else:
             self._id = None
         self.get.cache_clear()
 
-    def initialize(self):
-        """Name and settings are not present while creating object, so additional initialization is needed."""
-        self.perform_checks()
-        self.set_index()
-        self.id = self.data.iloc[0][self.settings["ID_COLUMN"]]
+    def set_id(self, new_id):
+        self.id = new_id
 
     def perform_checks(self):
-        # Model point set must have id_column
-        id_column = self.settings["ID_COLUMN"]
-        if id_column not in self.data.columns:
-            raise CashflowModelError(f"\nThere is no column '{id_column}' in model_point_set '{self.name}'.")
+        id_column_name = self.settings["ID_COLUMN"]
+
+        # Model point set must have ID_COLUMN
+        if id_column_name not in self.data.columns:
+            raise CashflowModelError(f"\nModel point set '{self.name}' is missing the required column '{id_column_name}'.")
 
         # ID must be unique in the 'main' model point set
-        id_column = self.settings["ID_COLUMN"]
         if self.name == "main":
-            if not self.data[id_column].is_unique:
-                msg = f"\nThe 'main' model point set must have unique values in '{id_column}' column."
-                raise CashflowModelError(msg)
+            if not self.data[id_column_name].is_unique:
+                raise CashflowModelError(f"\nThe 'main' model point set must have unique values in '{id_column_name}' column.")
 
     def set_index(self):
-        """ID column in original form stays as a column, ID column as a string becomes an index."""
-        id_column = self.settings["ID_COLUMN"]
-        self.data[id_column + "_duplicate"] = self.data[id_column]
-        self.data[id_column] = self.data[id_column].astype(str)
-        self.data = self.data.set_index(id_column)
-        self.data[id_column] = self.data[id_column + "_duplicate"]
-        self.data = self.data.drop(columns=[id_column + "_duplicate"])
+        """Convert ID column to string and use it as index, while preserving the original ID column."""
+        id_column_name = self.settings["ID_COLUMN"]
+        self.data = self.data.set_index(self.data[id_column_name].astype(str))
 
 
 class Model:
     """Actuarial cash flow model.
     Model combines model variables and model point sets."""
     def __init__(self, variables, model_point_sets, settings):
         self.variables = variables
         self.model_point_sets = model_point_sets
         self.settings = settings
 
     def run(self, part=None):
         """Orchestrate all steps of the cash flow model run."""
-        one_core = part == 0 or part is None  # single or first part
-        main = get_object_by_name(self.model_point_sets, "main")
+        # Get the start and end indices of the model points to be calculated
+        calculation_range = self.get_calculation_range(part)
+        if calculation_range is None:
+            return None
+        range_start, range_end = calculation_range
 
-        # Set calculation ranges
+        # Perform calculations
+        one_core = part == 0 or part is None  # single core or first part of multiprocessing calculation
+        log_message("Starting calculations...", show_time=True, print_and_save=one_core)
+        if self.settings["AGGREGATE"]:
+            output = self.compute_aggregated_results(range_start, range_end, one_core)
+        else:
+            output = self.compute_individual_results(range_start, range_end, one_core)
+
+        # Create a diagnostic file
+        diagnostic = self.create_diagnostic_data()
+
+        return output, diagnostic
+
+    def get_calculation_range(self, part):
+        main = get_object_by_name(self.model_point_sets, "main")
         range_start, range_end = 0, len(main)
         if self.settings["MULTIPROCESSING"]:
             main_ranges = split_to_ranges(len(main), multiprocessing.cpu_count())
             # Number of model points is lower than the number of CPUs, only calculate on the 1st core
             if part >= len(main_ranges):
                 return None
             range_start, range_end = main_ranges[part]
+        return range_start, range_end
 
-        # Perform calculations
-        print_log("Starting calculations...", show_time=True, visible=one_core)
-        if self.settings["AGGREGATE"]:
-            output = self.compute_aggregated_results(range_start, range_end, one_core)
-        else:
-            output = self.compute_individual_results(range_start, range_end, one_core)
-
-        # Create a diagnostic file
-        diagnostic = None
+    def create_diagnostic_data(self):
         if self.settings["SAVE_DIAGNOSTIC"]:
             diagnostic = pd.DataFrame({
                 "variable": [v.name for v in self.variables],
                 "calc_order": [v.calc_order for v in self.variables],
                 "calc_direction": [v.calc_direction for v in self.variables],
                 "cycle": [v.cycle for v in self.variables],
                 "cycle_order": [v.cycle_order for v in self.variables],
                 "variable_type": [get_variable_type(v) for v in self.variables],
                 "aggregation_type": [v.aggregation_type for v in self.variables],
                 "runtime": [v.runtime for v in self.variables]
             })
-
-        return output, diagnostic
+        else:
+            diagnostic = None
+        return diagnostic
 
     def compute_aggregated_results(self, range_start, range_end, one_core):
-        p = functools.partial(self.calculate_model_point, one_core=one_core, progressbar_max=range_end)
+        calculate_model_point_partial = functools.partial(
+            self.calculate_model_point, one_core=one_core, progressbar_max=range_end
+        )
+        output_columns = self.prepare_output_columns()
+        num_output_columns = len(output_columns)
+
+        # Define the initial batch size to process, to prevent excessive memory usage
+        batch_size = self.agg_calculate_batch_size(num_output_columns)
+        batch_start, batch_end = range_start, min(range_start + batch_size, range_end)
 
-        # Multiplier that takes into account aggregation type
+        # Create an array of multipliers based on the aggregation type of each variable
         multiplier = np.array([1 if v.aggregation_type == "sum" else 0 for v in self.variables])
 
-        # Prepare output columns
+        # Calculate aggregated results for all model points without grouping
+        if self.settings["GROUP_BY_COLUMN"] is None:
+            results = self.agg_calculate_without_grouping(calculate_model_point_partial, batch_start, batch_end,
+                                                          batch_size, range_end, multiplier)
+            output = self.agg_prepare_output_without_grouping(results, output_columns, one_core)
+
+        # Calculate aggregated results for all model points, grouped by the specified column
+        else:
+            group_sums = self.agg_calculate_with_grouping(calculate_model_point_partial, batch_start, batch_end,
+                                                          batch_size, range_end, multiplier, num_output_columns)
+            output = self.agg_prepare_output_with_grouping(group_sums, output_columns, one_core)
+        return output
+
+    def prepare_output_columns(self):
         if len(self.settings["OUTPUT_COLUMNS"]) == 0:
             output_columns = [v.name for v in self.variables]
         else:
             output_columns = self.settings["OUTPUT_COLUMNS"]
 
-        # Calculate batch_size based on available memory
+        return output_columns
+
+    def agg_calculate_batch_size(self, num_output_columns):
+        """
+        Calculate the batch size based on available memory.
+
+        The batch size is calculated to avoid memory errors when processing model points.
+        Each model point outputs a numpy array with "t" rows and "num_output_columns" columns.
+        The calculation takes into account whether the processing is done on one core or multiple cores (multiprocessing).
+
+        Args:
+            num_output_columns (int): The number of output columns.
+
+        Returns:
+            int: The batch size.
+        """
         t = self.settings["T_MAX_OUTPUT"] + 1
-        v = len(output_columns)
         float_size = np.dtype(np.float64).itemsize
         num_cores = 1 if not self.settings["MULTIPROCESSING"] else multiprocessing.cpu_count()
-        batch_size = int((psutil.virtual_memory().available * 0.95) // ((t * v) * float_size) // num_cores)
+        available_memory = psutil.virtual_memory().available * 0.95
+        memory_per_model_point = (t * num_output_columns) * float_size
+        batch_size = int(available_memory // (memory_per_model_point // num_cores))
+        batch_size = max(batch_size, 1)
+        return batch_size
+
+    def agg_calculate_without_grouping(self, calculate_model_point_partial, batch_start, batch_end, batch_size, range_end,
+                                   multiplier):
+        # Initialize the results with the output of the first model point calculation
+        if batch_start == 0:
+            results = calculate_model_point_partial(0)
+            batch_start += 1
+        else:
+            results = 0
 
-        # Initial calculation batch
-        batch_start, batch_end = range_start, min(range_start + batch_size, range_end)
+        # Calculate the results for each batch of model points iteratively, aggregating the results
+        while batch_start < range_end:
+            # batch_results_list is a list of model point results (each result is a 2D array)
+            batch_results_list = [*map(calculate_model_point_partial, range(batch_start, batch_end))]
+            batch_results = sum(batch_results_list)
+            results += batch_results * multiplier[:, None]
+            batch_start = batch_end
+            batch_end = min(batch_end + batch_size, range_end)
 
-        # Aggregate all model points (without grouping)
-        if self.settings["GROUP_BY_COLUMN"] is None:
-            # Initiate with results of the first model point
-            if batch_start == 0:
-                results = p(0)
-                batch_start += 1
-            else:
-                results = 0
+        return results
 
-            # Calculate batches iteratively
-            while batch_start < range_end:
-                lst = [*map(p, range(batch_start, batch_end))]  # list of mp_results (arrays of arrays)
-                batch_results = functools.reduce(lambda a, b: a + b, lst)
-                results += batch_results * multiplier[:, None]
-                batch_start = batch_end
-                batch_end = min(batch_end+batch_size, range_end)
-
-            # Prepare the 'output' data frame
-            print_log("Preparing output...", show_time=True, visible=one_core)
-            results = np.transpose(results)
-            output = pd.DataFrame(data=results, columns=output_columns)
-
-        # Aggregate by groups
-        else:
-            main = get_object_by_name(self.model_point_sets, "main")
-            group_by_column = self.settings["GROUP_BY_COLUMN"]
-            if group_by_column not in main.data.columns:
-                msg = (f"There is no column '{group_by_column}' in the 'main' model point set. "
-                       f"Please review the 'GROUP_BY_COLUMN' setting.")
-                raise CashflowModelError(msg)
-            unique_groups = main.data[group_by_column].unique()
+    def agg_prepare_output_without_grouping(self, results, output_columns, one_core):
+        # Prepare the 'output' data frame
+        log_message("Preparing output...", show_time=True, print_and_save=one_core)
+        results = np.transpose(results)
+        output = pd.DataFrame(data=results, columns=output_columns)
+        return output
+
+    def agg_calculate_with_grouping(self, calculate_model_point_partial, batch_start, batch_end, batch_size, range_end,
+                                multiplier, num_output_columns):
+        max_output = self.settings["T_MAX_OUTPUT"] + 1
+        group_by_column = self.settings["GROUP_BY_COLUMN"]
+        main = get_object_by_name(self.model_point_sets, "main")
+
+        # Check that the grouping column exists in the main model point set
+        if group_by_column not in main.data.columns:
+            msg = (f"There is no column '{group_by_column}' in the 'main' model point set. "
+                   f"Please review the 'GROUP_BY_COLUMN' setting.")
+            raise CashflowModelError(msg)
+
+        # Get the indices of the first element from each group
+        unique_groups = main.data[group_by_column].unique()
+        first_indexes = get_first_indexes(main.data[group_by_column])
+
+        # Initialize empty results for each group
+        group_sums = {group: np.zeros((num_output_columns, max_output)) for group in unique_groups}
+
+        # Process batches iteratively to calculate the results
+        while batch_start < range_end:
+            # batch_results_list is a list of model point results (each result is a 2D array)
+            batch_results_list = [calculate_model_point_partial(i) for i in range(batch_start, batch_end)]
+            groups = main.data.iloc[batch_start:batch_end][group_by_column].tolist()
+            if_firsts = np.isin(range(batch_start, batch_end), first_indexes)
+
+            for mp_result, group, if_first in zip(batch_results_list, groups, if_firsts):
+                if if_first:
+                    group_sums[group] += mp_result
+                else:
+                    group_sums[group] += mp_result * multiplier[:, None]
+
+            batch_start = batch_end
+            batch_end = min(batch_end + batch_size, range_end)
 
-            # Indexes of the first element from each group
-            first_indexes = get_first_indexes(main.data[group_by_column])
+        return group_sums
 
-            # Initiate empty results
-            group_sums = {group: np.array([np.zeros(t) for _ in range(v)]) for group in unique_groups}
+    def agg_prepare_output_with_grouping(self, group_sums, output_columns, one_core):
+        group_by_column = self.settings["GROUP_BY_COLUMN"]
 
-            # Calculate batches iteratively
-            while batch_start < range_end:
-                lst = [*map(p, range(batch_start, batch_end))]  # list of mp_results
-                groups = main.data.iloc[batch_start:batch_end][group_by_column].tolist()
-                if_firsts = [i in first_indexes for i in range(batch_start, batch_end)]
-
-                for mp_result, group, if_first in zip(lst, groups, if_firsts):
-                    if if_first:
-                        group_sums[group] += mp_result
-                    else:
-                        group_sums[group] += mp_result * multiplier[:, None]
-                batch_start = batch_end
-                batch_end = min(batch_end+batch_size, range_end)
-
-            # Prepare the 'output' data frame
-            print_log("Preparing output...", show_time=True, visible=one_core)
-            lst_dfs = []
-            for group, data in group_sums.items():
-                group_df = pd.DataFrame(data=np.transpose(data), columns=output_columns)
-                group_df.insert(0, group_by_column, group)
-                lst_dfs.append(group_df)
-            output = pd.concat(lst_dfs, ignore_index=True)
+        log_message("Preparing output...", show_time=True, print_and_save=one_core)
 
+        lst_dfs = []
+        for group, data in group_sums.items():
+            group_df = pd.DataFrame(data=np.transpose(data), columns=output_columns)
+            group_df.insert(0, group_by_column, group)
+            lst_dfs.append(group_df)
+
+        output = pd.concat(lst_dfs, ignore_index=True)
         return output
 
     def compute_individual_results(self, range_start, range_end, one_core):
-        p = functools.partial(self.calculate_model_point, one_core=one_core, progressbar_max=range_end)
+        calculate_model_point_partial = functools.partial(
+            self.calculate_model_point, one_core=one_core, progressbar_max=range_end
+        )
 
+        mp = range_end - range_start
+        results = self.ind_allocate_memory_for_results(mp)
+        results = [*map(calculate_model_point_partial, range(range_start, range_end))]
+
+        output_columns = self.prepare_output_columns()
+        output = self.ind_prepare_output(results, output_columns, one_core)
+
+        return output
+
+    def ind_allocate_memory_for_results(self, mp):
         # Allocate memory for results
         t = self.settings["T_MAX_OUTPUT"] + 1
         v = len(self.variables) if len(self.settings["OUTPUT_COLUMNS"]) == 0 else len(self.settings["OUTPUT_COLUMNS"])
-        mp = range_end - range_start
+
         float_size = np.dtype(np.float64).itemsize
         results_size = t * v * mp * float_size
         results_size_mb = results_size / (1024 ** 2)
         num_cores = 1 if not self.settings["MULTIPROCESSING"] else multiprocessing.cpu_count()
 
         # Results may require a lot of memory
         msg = (f"Failed to allocate memory for the output with {t} periods, {v} variables, and {mp} model points "
@@ -488,43 +602,37 @@
             raise CashflowModelError(msg)
 
         # Allocate results to available RAM memory
         try:
             results = [np.empty((v, t), dtype=float) for _ in range(mp)]
         except MemoryError:
             raise CashflowModelError(msg)
-        else:
-            results = [*map(p, range(range_start, range_end))]
 
-        # Prepare output columns
-        if len(self.settings["OUTPUT_COLUMNS"]) == 0:
-            output_columns = [v.name for v in self.variables]
-        else:
-            output_columns = self.settings["OUTPUT_COLUMNS"]
+        return results
 
+    def ind_prepare_output(self, results, output_columns, one_core):
         # Prepare the 'output' data frame
-        print_log("Preparing output...", show_time=True, visible=one_core)
+        log_message("Preparing output...", show_time=True, print_and_save=one_core)
         total_data = [pd.DataFrame(np.transpose(arr)) for arr in results]
         output = pd.concat(total_data)
         output.columns = output_columns
-
         return output
 
     def calculate_model_point(self, row, one_core, progressbar_max):
         """Returns array of arrays:
         [[v1_t0, v1_t1, v1_t2, ... v1_tm],
          [v2_t0, v2_t1, v2_t2, ... v2_tm],
          ...
          [vn_t0, vn_t1, vn_t2, ... v2_tm]]"""
         main = get_object_by_name(self.model_point_sets, "main")
 
         # Set model point's id
         model_point_id = main.data.index[row]
         for model_point_set in self.model_point_sets:
-            model_point_set.id = model_point_id
+            model_point_set.set_id(model_point_id)
 
         # Perform calculations
         max_calc_order = self.variables[-1].calc_order
         for calc_order in range(1, max_calc_order + 1):
             # Either a single variable or a cycle
             variables = [v for v in self.variables if v.calc_order == calc_order]
 
@@ -532,39 +640,45 @@
             if len(variables) == 1:
                 v = variables[0]
                 start = time.time()
                 v.calculate()
                 v.runtime += time.time() - start
             # Cycle
             else:
-                start = time.time()
-                first_variable = variables[0]
-                calc_direction = first_variable.calc_direction
-                if calc_direction in (0, 1):
-                    for t in range(self.settings["T_MAX_CALCULATION"] + 1):
-                        for v in variables:
-                            v.calculate_t(t)
-                else:
-                    for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
-                        for v in variables:
-                            v.calculate_t(t)
-                end = time.time()
-                avg_runtime = (end-start)/len(variables)
-                for v in variables:
-                    v.runtime += avg_runtime
+                self.calculate_cycle(variables)
 
         # Average stochastic results
         for v in self.variables:
             if isinstance(v, StochasticVariable):
                 v.average_result_stoch()
 
         # Get results and trim for T_MAX_OUTPUT,results may contain subset of columns
         if len(self.settings["OUTPUT_COLUMNS"]) > 0:
             mp_results = np.array([v.result[:self.settings["T_MAX_OUTPUT"]+1] for v in self.variables if v.name in self.settings["OUTPUT_COLUMNS"]])
         else:
             mp_results = np.array([v.result[:self.settings["T_MAX_OUTPUT"]+1] for v in self.variables])
 
         # Update progressbar
         if one_core:
-            updt(progressbar_max, row + 1)
+            update_progressbar(progressbar_max, row + 1)
 
         return mp_results
+
+    def calculate_cycle(self, variables):
+        start = time.time()
+        first_variable = variables[0]
+        calc_direction = first_variable.calc_direction
+        t_max_calculation = self.settings["T_MAX_CALCULATION"]
+
+        if calc_direction in (0, 1):
+            for t in range(t_max_calculation + 1):
+                for v in variables:
+                    v.calculate_t(t)
+        else:
+            for t in range(t_max_calculation, -1, -1):
+                for v in variables:
+                    v.calculate_t(t)
+
+        end = time.time()
+        avg_runtime = (end-start)/len(variables)
+        for v in variables:
+            v.runtime += avg_runtime
```

### Comparing `cashflower-0.7.0/cashflower/cython/discount.c` & `cashflower-0.7.1/cashflower/cython/discount.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.6 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/.local/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
             "/home/runner/.local/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
@@ -42,18 +42,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_6" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030006F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -137,14 +137,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -198,14 +200,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -259,60 +263,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -395,14 +422,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -587,22 +617,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -652,15 +682,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -738,16 +768,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1091,15 +1126,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1178,15 +1213,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1291,32 +1326,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1358,15 +1376,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -2103,16 +2121,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2120,16 +2138,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2159,30 +2178,30 @@
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_6
-#define __PYX_HAVE_RT_ImportType_proto_3_0_6
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_6(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_6(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_6 {
-   __Pyx_ImportType_CheckSize_Error_3_0_6 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_6 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_6 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_6(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_6 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2284,15 +2303,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -4840,41 +4859,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_6(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_6); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_6(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_6(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_6); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5080,15 +5099,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("discount", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to discount pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "discount" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -6876,19 +6895,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -6993,15 +7012,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -7012,15 +7031,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -7044,15 +7063,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -7126,18 +7145,18 @@
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_6
-#define __PYX_HAVE_RT_ImportType_3_0_6
-static PyTypeObject *__Pyx_ImportType_3_0_6(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_6 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -7183,23 +7202,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_6 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_6 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8450,15 +8469,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -8909,15 +8928,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `cashflower-0.7.0/cashflower/cython/discount.pyx` & `cashflower-0.7.1/cashflower/cython/discount.pyx`

 * *Files identical despite different names*

### Comparing `cashflower-0.7.0/cashflower/reader.py` & `cashflower-0.7.1/cashflower/reader.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.7.0/cashflower/start.py` & `cashflower-0.7.1/cashflower/start.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,25 +10,47 @@
 import os
 import pandas as pd
 import shutil
 
 from .core import ArrayVariable, Model, ModelPointSet, Runplan, StochasticVariable, Variable
 from .error import CashflowModelError
 from .graph import create_directed_graph, filter_variables_and_graph, get_calls, get_predecessors, set_calc_direction
-from .utils import get_git_commit_info, get_object_by_name, print_log, save_log_to_file
+from .utils import get_git_commit_info, get_object_by_name, log_message, save_log_to_file
 
 
 def create_model(model):
-    """Create a folder structure for a model."""
+    """Create a folder structure for a model.
+
+    Args:
+        model (str): The path where the folder structure should be created.
+
+    Returns:
+        None
+    """
     template_path = os.path.join(os.path.dirname(__file__), "model_tpl")
-    shutil.copytree(template_path, model)
+
+    try:
+        shutil.copytree(template_path, model)
+    except OSError as e:
+        print(f"Error: {e.filename} - {e.strerror}.")
 
 
 def load_settings(settings=None):
-    """Add missing settings."""
+    """
+    Load settings for the model.
+
+    If T_MAX_OUTPUT exceeds T_MAX_CALCULATION, T_MAX_OUTPUT is adjusted to match T_MAX_CALCULATION
+    and a log message is generated.
+
+    Args:
+        settings (dict, optional): A dictionary of user's settings. Defaults to None.
+
+    Returns:
+        dict: A dictionary of settings.
+    """
     initial_settings = {
         "AGGREGATE": True,
         "GROUP_BY_COLUMN": None,
         "ID_COLUMN": "id",
         "MULTIPROCESSING": False,
         "NUM_STOCHASTIC_SCENARIOS": None,
         "OUTPUT_COLUMNS": [],
@@ -39,69 +61,104 @@
         "T_MAX_OUTPUT": 720,
     }
 
     if settings is None:
         return initial_settings
 
     # Update with the user settings
-    for key, value in settings.items():
-        initial_settings[key] = value
+    initial_settings.update(settings)
 
     # Maximal output t can't exceed maximal calculation t
-    if initial_settings["T_MAX_CALCULATION"] < initial_settings["T_MAX_OUTPUT"]:
-        out = initial_settings["T_MAX_OUTPUT"]
-        cal = initial_settings["T_MAX_CALCULATION"]
+    out = initial_settings["T_MAX_OUTPUT"]
+    cal = initial_settings["T_MAX_CALCULATION"]
+
+    if cal < out:
         msg = (f"T_MAX_OUTPUT ('{out}') exceeds T_MAX_CALCULATION ('{cal}'); "
                f"T_MAX_OUTPUT adjusted to match T_MAX_CALCULATION.")
-        print_log(msg)
-        initial_settings["T_MAX_OUTPUT"] = initial_settings["T_MAX_CALCULATION"]
+        log_message(msg)
+        initial_settings["T_MAX_OUTPUT"] = cal
 
     return initial_settings
 
 
 def get_runplan(input_members, args):
-    """Get runplan object from input.py script. Assign version if provided in the CLI command."""
+    """
+    Get runplan object from input.py script. Assign version if provided in the CLI command.
+
+    Args:
+        input_members (list): A list of tuples containing the name and instance of each input member.
+        args (obj): An object containing the CLI command arguments.
+
+    Returns:
+        obj: The first Runplan object found in the input_members list, or None if no Runplan object is found.
+    """
     runplan = None
     for name, item in input_members:
         if isinstance(item, Runplan):
             runplan = item
             break
 
     if runplan is not None and args.version is not None:
         runplan.version = args.version
 
     return runplan
 
 
 def get_model_point_sets(input_members, settings, args):
-    """Get model point set objects from input.py script."""
-    model_point_set_members = [m for m in input_members if isinstance(m[1], ModelPointSet)]
+    """
+    Get model point set objects from the input.py script.
+
+    Args:
+        input_members (list): List of tuples containing member names and their corresponding values.
+        settings (object): Settings object containing configuration for the model point sets.
+        args (object): Arguments object containing command line arguments.
+
+    Returns:
+        list: A list of initialized ModelPointSet objects.
+
+    Raises:
+        CashflowModelError: If a model point set named 'main' is not found in the input_members.
+    """
+    model_point_set_members = [member for member in input_members if isinstance(member[1], ModelPointSet)]
 
     main = None
     model_point_sets = []
     for name, model_point_set in model_point_set_members:
         model_point_set.name = name
         model_point_set.settings = settings
         model_point_set.initialize()
         model_point_sets.append(model_point_set)
         if name == "main":
             main = model_point_set
 
     if main is None:
-        raise CashflowModelError("\nA model must have a model point set named 'main'.")
+        raise CashflowModelError("\nA model must have a model point set named 'main'. "
+                                 "Please check your input.py script.")
 
     if args.id is not None:
         chosen_id = str(args.id)
         main.data = main.data.loc[chosen_id]
 
     return model_point_sets
 
 
 def get_variables(model_members, settings):
-    """Get model variables from model.py script."""
+    """
+   Get model variables from model.py script.
+
+   Args:
+       model_members (list): A list of tuples containing the names and values of the model members.
+       settings (dict): A dictionary of settings for the model.
+
+   Returns:
+       list: A list of Variable objects.
+
+   Raises:
+       CashflowModelError: If a variable is named 't' or if a stochastic variable is used without setting the number of stochastic scenarios.
+   """
     variable_members = [m for m in model_members if isinstance(m[1], Variable)]
     variables = []
 
     for name, variable in variable_members:
         # Set name
         if name == "t":
             msg = f"\nA variable can not be named '{name}' because it is a system variable. Please rename it."
@@ -119,15 +176,28 @@
             variable.result_stoch = np.empty((settings["NUM_STOCHASTIC_SCENARIOS"], settings["T_MAX_CALCULATION"]+1))
 
         variables.append(variable)
     return variables
 
 
 def prepare_model_input(settings, args):
-    """Get input for the cash flow model."""
+    """
+    Prepare the input for the cash flow model.
+
+    Args:
+        settings (dict): A dictionary of settings for the model.
+        args (dict): A dictionary of arguments for the model.
+
+    Returns:
+        tuple: A tuple containing the runplan, model point sets, and variables for the cash flow model.
+
+    Notes:
+        This function imports the input and model modules, gets the members of these modules,
+        and then uses these members to get the runplan, model point sets, and variables for the cash flow model.
+    """
     input_module = importlib.import_module("input")
     model_module = importlib.import_module("model")
 
     # input.py contains runplan and model point sets
     input_members = inspect.getmembers(input_module)
     runplan = get_runplan(input_members, args)
     model_point_sets = get_model_point_sets(input_members, settings, args)
@@ -135,80 +205,126 @@
     # model.py contains model variables
     model_members = inspect.getmembers(model_module)
     variables = get_variables(model_members, settings)
 
     return runplan, model_point_sets, variables
 
 
+def check_for_array_variables_in_cycle(cycle):
+    for variable in cycle:
+        if isinstance(variable, ArrayVariable):
+            msg = (f"Variable '{variable.name}' is part of a cycle so it can't be modelled as an array variable."
+                   f"\nCycle: {cycle}"
+                   f"\nPlease remove 'array=True' from the decorator and recode the variable.")
+            raise CashflowModelError(msg)
+
+
+def set_cycle_order(dg_cycle):
+    cycle_order = 0
+    while dg_cycle.nodes:
+        cycle_nodes_without_predecessors = [cn for cn in dg_cycle.nodes if len(list(dg_cycle.predecessors(cn))) == 0]
+        if len(cycle_nodes_without_predecessors) > 0:
+            for node in cycle_nodes_without_predecessors:
+                cycle_order += 1
+                node.cycle_order = cycle_order
+            dg_cycle.remove_nodes_from(cycle_nodes_without_predecessors)
+        else:
+            cycle_variable_nodes = [node.name for node in dg_cycle.nodes]
+            msg = (f"Circular relationship without time step difference is not allowed. "
+                   f"Please review variables: {cycle_variable_nodes}."
+                   f"\nIf circular relationship without time step difference is necessary in your project, "
+                   f"please raise it on: github.com/acturtle/cashflower")
+            raise CashflowModelError(msg)
+
+
 def resolve_calculation_order(variables, output_columns):
-    """Determines a safe execution order for variables to avoid recursion errors."""
+    """
+    Determines a safe execution order for variables to avoid recursion errors.
+
+    This function takes a list of variables and an optional list of output columns as input.
+    It first creates a dictionary of called functions for each variable, then creates a directed graph representing
+    the relationships between variables. If output columns are specified, it filters the variables and graph
+    to only include the necessary variables. It then sets the calculation order of the variables,
+    handling both acyclic and cyclic relationships.
+    Finally, it sorts the variables by calculation order and sets the calculation direction.
+
+    Parameters:
+    variables (list): A list of variable objects.
+    output_columns (list, optional): A list of output column names. If specified, only variables that are needed for
+        these columns will be included in the calculation order.
+
+    Returns:
+    list: A list of variable objects, sorted by calculation order and with their calculation direction set.
+    """
     # [1] Dictionary of called functions (key = variable; value = other variables called by it)
     calls = {}
     for variable in variables:
         calls[variable] = get_calls(variable, variables)
 
     # [2] Create directed graph for all variables
     dg = create_directed_graph(variables, calls)
 
-    # [3] User has chosen output so remove unneeded variables
+    # Debug
+    # import matplotlib.pyplot as plt
+    # nx.draw(dg, with_labels=True)
+    # plt.show()
+
+    # [3] User has chosen output columns so remove unneeded variables
     if output_columns is not None:
         variables, dg = filter_variables_and_graph(output_columns, variables, dg)
 
     # [4] Set calculation order of variables ('calc_order')
     calc_order = 0
     while dg.nodes:
         nodes_without_predecessors = [n for n in dg.nodes if len(list(dg.predecessors(n))) == 0]
 
-        # [4a] There are variables without any predecessors
+        # [4a] Acyclic - there are variables without any predecessors
         if len(nodes_without_predecessors) > 0:
             for node in nodes_without_predecessors:
                 calc_order += 1
                 node.calc_order = calc_order
             dg.remove_nodes_from(nodes_without_predecessors)
 
-        # [4b] There is a cyclic relationship between variables
+        # [4b] Cyclic - there is a cyclic relationship between variables
         else:
             cycles = list(nx.simple_cycles(dg))
+
             cycles_without_predecessors = [c for c in cycles if len(get_predecessors(c[0], dg)) == len(c)]
 
+            # Graph contains strongly connected components (SCC)
+            if len(cycles_without_predecessors) == 0:
+                # Find strongly connected components
+                sccs = list(nx.strongly_connected_components(dg))
+
+                # Find source SCC
+                for scc in sccs:
+                    has_incoming_edge = False
+                    for node in scc:
+                        for edge in dg.in_edges(node):
+                            if edge[0] not in scc:
+                                has_incoming_edge = True
+                                break
+                        if has_incoming_edge:
+                            break
+                    if not has_incoming_edge:
+                        scc = sorted(list(scc))
+                        cycles_without_predecessors = [scc]
+
             for cycle in cycles_without_predecessors:
-                # [4b_1] Ensure that there are no ArrayVariables in cycles
-                for variable in cycle:
-                    if isinstance(variable, ArrayVariable):
-                        msg = (f"Variable '{variable.name}' is part of a cycle so it can't be modelled as an array variable."
-                               f"\nCycle: {cycle}"
-                               f"\nPlease remove 'array=True' from the decorator and recode the variable.")
-                        raise CashflowModelError(msg)
+                # Ensure that there are no ArrayVariables in cycles
+                check_for_array_variables_in_cycle(cycle)
 
-                # [4b_2] Set the calculation order within the cycle
+                # Set the calculation order within the cycle ('cycle_order')
                 calls_t = {}  # dictionary of called functions but only for the same time period ("t")
                 for variable in cycle:
                     calls_t[variable] = get_calls(variable, cycle, argument_t_only=True)
-
-                # Create directed graph for cycle variables
                 dg_cycle = create_directed_graph(cycle, calls_t)
+                set_cycle_order(dg_cycle)
 
-                # Set 'cycle_order'
-                cycle_order = 0
-                while dg_cycle.nodes:
-                    cycle_nodes_without_predecessors = [cn for cn in dg_cycle.nodes if len(list(dg_cycle.predecessors(cn))) == 0]
-                    if len(cycle_nodes_without_predecessors) > 0:
-                        for node in cycle_nodes_without_predecessors:
-                            cycle_order += 1
-                            node.cycle_order = cycle_order
-                        dg_cycle.remove_nodes_from(cycle_nodes_without_predecessors)
-                    else:
-                        cycle_variable_nodes = [node.name for node in dg_cycle.nodes]
-                        msg = (f"Circular relationship without time step difference is not allowed. "
-                               f"Please review variables: {cycle_variable_nodes}."
-                               f"\nIf circular relationship without time step difference is necessary in your project, "
-                               f"please raise it on: github.com/acturtle/cashflower")
-                        raise CashflowModelError(msg)
-
-                # [4b_3] All the variables from a cycle have the same 'calc_order' value
+                # All the variables from a cycle have the same 'calc_order' value
                 calc_order += 1
                 for node in cycle:
                     node.calc_order = calc_order
                     node.cycle = True
                 dg.remove_nodes_from(cycle)
 
     # [5] Sort variables for calculation order
@@ -217,67 +333,95 @@
     # [6] Set calculation direction of calculation ('calc_direction' attribute)
     variables = set_calc_direction(variables)
 
     return variables
 
 
 def start_single_core(settings, args):
-    """Create and run a cash flow model."""
+    """
+    Create and run a cash flow model on a single core.
+
+    Args:
+        settings (dict): Model settings.
+        args (dict): Additional arguments.
+
+    Returns:
+        tuple: A tuple containing the model output and runtime.
+    """
     # Prepare model components
-    print_log("Reading model components...", show_time=True)
+    log_message("Reading model components...", show_time=True)
     runplan, model_point_sets, variables = prepare_model_input(settings, args)
     output_columns = None if len(settings["OUTPUT_COLUMNS"]) == 0 else settings["OUTPUT_COLUMNS"]
     variables = resolve_calculation_order(variables, output_columns)
 
     # Log runplan version and number of model points
     if runplan is not None:
-        print_log(f"Runplan version: {runplan.version}")
+        log_message(f"Runplan version: {runplan.version}")
     main = get_object_by_name(model_point_sets, "main")
-    print_log(f"Number of model points: {len(main)}")
+    log_message(f"Number of model points: {len(main)}")
 
     # Run model on single core
     model = Model(variables, model_point_sets, settings)
     output, runtime = model.run()
     return output, runtime
 
 
 def start_multiprocessing(part, settings, args):
-    """Run subset of the model points using multiprocessing."""
+    """
+    Run subset of the model points using multiprocessing.
+
+    Args:
+        part (int): The part of the model points to run.
+        settings (dict): The model settings.
+        args (object): The command line arguments.
+
+    Returns:
+        tuple: A tuple containing the output and runtime of the model run.
+    """
     cpu_count = multiprocessing.cpu_count()
     one_core = part == 0
 
     # Prepare model components
-    print_log("Reading model components...", show_time=True, visible=one_core)
+    log_message("Reading model components...", show_time=True, print_and_save=one_core)
     runplan, model_point_sets, variables = prepare_model_input(settings, args)
     output_columns = None if len(settings["OUTPUT_COLUMNS"]) == 0 else settings["OUTPUT_COLUMNS"]
     variables = resolve_calculation_order(variables, output_columns)
 
     # Log runplan version and number of model points
     if runplan is not None:
-        print_log(f"Runplan version: {runplan.version}", visible=one_core)
+        log_message(f"Runplan version: {runplan.version}", print_and_save=one_core)
     main = get_object_by_name(model_point_sets, "main")
-    print_log(f"Number of model points: {len(main)}", visible=one_core)
-    print_log(f"Multiprocessing on {cpu_count} cores", visible=one_core)
-    print_log(f"Calculation of ca. {len(main) // cpu_count} model points per core", visible=one_core)
+    log_message(f"Number of model points: {len(main)}", print_and_save=one_core)
+    log_message(f"Multiprocessing on {cpu_count} cores", print_and_save=one_core)
+    log_message(f"Calculation of ca. {len(main) // cpu_count} model points per core", print_and_save=one_core)
 
     # Run model on multiple cores
     model = Model(variables, model_point_sets, settings)
     model_run = model.run(part)
 
     if model_run is None:
         part_output, part_runtime = None, None
     else:
         part_output, part_runtime = model_run
     return part_output, part_runtime
 
 
 def merge_part_outputs(part_outputs, settings):
-    """Merge outputs from multiprocessing and save to files."""
+    """
+    Merge outputs from multiprocessing.
+
+    Args:
+        part_outputs (list): A list of outputs from multiprocessing.
+        settings (dict): A dictionary of settings.
+
+    Returns:
+        pandas.DataFrame: The merged output.
+    """
     # Nones are returned, when number of policies < number of cpus
-    part_outputs = [po for po in part_outputs if po is not None]
+    part_outputs = [part_output for part_output in part_outputs if part_output is not None]
 
     # Merge or concatenate outputs into one
     if settings["AGGREGATE"]:
         output = functools.reduce(lambda x, y: x.add(y, fill_value=0), part_outputs)
         if settings["GROUP_BY_COLUMN"] is not None:
             # group_by_column should not be added up
             output[settings["GROUP_BY_COLUMN"]] = part_outputs[0][settings["GROUP_BY_COLUMN"]]
@@ -292,93 +436,161 @@
     part_diagnostic = [item for item in part_diagnostic if item is not None]
     total_runtimes = sum([item["runtime"] for item in part_diagnostic])
     diagnostic = part_diagnostic[0]
     diagnostic["runtime"] = total_runtimes
     return diagnostic
 
 
-def run(settings=None, path=None):
-    timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    settings = load_settings(settings)
-    output, diagnostic = None, None
-
-    # Parse arguments
+def parse_arguments():
+    """
+    Parse command line arguments.
+
+    Returns:
+        args: The parsed arguments.
+    """
     parser = argparse.ArgumentParser()
-    parser.add_argument("--id", "-i")
-    parser.add_argument("--version", "-v")
-    args = parser.parse_args()
 
-    # Start log
+    parser.add_argument("--id", "-i", help="Run a specific model point.")
+    parser.add_argument("--version", "-v", help="Run a specific version.")
+
+    return parser.parse_args()
+
+
+def run_multi_core(settings, args):
+    """
+    Run the model on multiple cores.
+
+    Args:
+        settings (dict): A dictionary containing the settings for the model.
+        args (argparse.Namespace): The arguments passed to the script.
+
+    Returns:
+        tuple: A tuple containing the output and diagnostic results.
+    """
+    process_func = functools.partial(start_multiprocessing, settings=settings, args=args)
+    cpu_count = multiprocessing.cpu_count()
+    with multiprocessing.Pool(cpu_count) as pool:
+        parts = pool.map(process_func, range(cpu_count))
+
+    # Merge model outputs
+    part_outputs = [part[0] for part in parts]
+    output = merge_part_outputs(part_outputs, settings)
+
+    # Merge runtimes
+    if settings["SAVE_DIAGNOSTIC"]:
+        part_diagnostic = [part[1] for part in parts]
+        diagnostic = merge_part_diagnostic(part_diagnostic)
+    else:
+        diagnostic = None
+
+    return output, diagnostic
+
+
+def save_results(timestamp, output, diagnostic, settings):
+    """
+    Save the output, diagnostic, and log files based on the settings.
+
+    Args:
+        timestamp (str): The timestamp to use in the filenames.
+        output (pandas.DataFrame): The output data to save.
+        diagnostic (pandas.DataFrame): The diagnostic data to save.
+        settings (dict): A dictionary containing the settings.
+    """
+    if not (settings["SAVE_OUTPUT"] or settings["SAVE_DIAGNOSTIC"] or settings["SAVE_LOG"]):
+        return None
+
+    if not os.path.exists("output"):
+        os.makedirs("output")
+
+    if settings["SAVE_OUTPUT"]:
+        filepath = f"output/{timestamp}_output.csv"
+        log_message(f"Saving output file: {filepath}", show_time=True)
+        output.to_csv(filepath, index=False)
+
+    if settings["SAVE_DIAGNOSTIC"]:
+        filepath = f"output/{timestamp}_diagnostic.csv"
+        log_message(f"Saving diagnostic file: {filepath}", show_time=True)
+        diagnostic.to_csv(filepath, index=False)
+
+    if settings["SAVE_LOG"]:
+        filepath = f"output/{timestamp}_log.txt"
+        log_message(f"Saving log file: {filepath}", show_time=True)
+        save_log_to_file(timestamp)
+
+
+def log_run_info(timestamp, path, args, settings):
+    """
+    Logs information about the current run.
+
+    Args:
+        timestamp (str): The timestamp of the run.
+        path (str): The path to the model.
+        args (argparse.Namespace): The command line arguments.
+        settings (dict): The settings for the run.
+
+    Returns:
+        None
+    """
+    # Log model info
     if path is not None:
-        print_log(f"Model: '{os.path.basename(path)}'", show_time=True)
-        print_log(f"Path: {path}")
+        log_message(f"Model: '{os.path.basename(path)}'", show_time=True)
+        log_message(f"Path: {path}")
     else:
-        print_log("Model", show_time=True)
-    print_log(f"Timestamp: {timestamp}")
-    print_log(f"User: '{getpass.getuser()}'")
+        log_message("Model", show_time=True)
+    log_message(f"Timestamp: {timestamp}")
+    log_message(f"User: '{getpass.getuser()}'")
     commit = get_git_commit_info()
     if commit is not None:
-        print_log(f"Git commit: {commit}")
-    print_log("")
+        log_message(f"Git commit: {commit}")
+    log_message("")
 
+    # Log command line arguments
     has_arguments = any(arg_value is not None for arg_value in vars(args).values())
     if has_arguments:
-        print_log("Arguments:")
+        log_message("Arguments:")
         for arg_name, arg_value in vars(args).items():
             if arg_value is not None:
-                print_log(f'- {arg_name}: {arg_value}')
-        print_log("")
+                log_message(f'- {arg_name}: {arg_value}')
+        log_message("")
 
-    print_log("Settings:")
+    # Log settings
+    log_message("Settings:")
     for key, value in settings.items():
         msg = f"- {key}: {value}"
-        print_log(msg)
-    print_log("")
+        log_message(msg)
+    log_message("")
+
+
+def run(settings=None, path=None):
+    """
+    Run the model with given settings and path.
 
-    # Run on single core
+    Args:
+        settings (dict, optional): Dictionary containing the settings. Defaults to None.
+        path (str, optional): Path where the model results will be saved. Defaults to None.
+
+    Returns:
+        pandas.DataFrame: The output of the modl.
+    """
+    timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    settings = load_settings(settings)
+    args = parse_arguments()
+    log_run_info(timestamp, path, args, settings)
+
+    # Run on single or multiple cores
     if not settings["MULTIPROCESSING"]:
         output, diagnostic = start_single_core(settings, args=args)
-
-    # Run on multiple cores
-    if settings["MULTIPROCESSING"]:
-        p = functools.partial(start_multiprocessing, settings=settings, args=args)
-        cpu_count = multiprocessing.cpu_count()
-        with multiprocessing.Pool(cpu_count) as pool:
-            parts = pool.map(p, range(cpu_count))
-
-        # Merge model outputs
-        part_outputs = [p[0] for p in parts]
-        output = merge_part_outputs(part_outputs, settings)
-
-        # Merge runtimes
-        if settings["SAVE_DIAGNOSTIC"]:
-            part_diagnostic = [p[1] for p in parts]
-            diagnostic = merge_part_diagnostic(part_diagnostic)
+    else:
+        output, diagnostic = run_multi_core(settings, args)
 
     # Add time column
     values = [*range(settings["T_MAX_OUTPUT"]+1)] * int(output.shape[0] / (settings["T_MAX_OUTPUT"]+1))
     output.insert(0, "t", values)
-    print_log("Finished!", show_time=True)
-    print_log("")
+
+    log_message("Finished!", show_time=True)
+    log_message("")
 
     # Save to csv files
-    if settings["SAVE_OUTPUT"] or settings["SAVE_DIAGNOSTIC"] or settings["SAVE_LOG"]:
-        if not os.path.exists("output"):
-            os.makedirs("output")
-
-        if settings["SAVE_OUTPUT"]:
-            filepath = f"output/{timestamp}_output.csv"
-            print_log(f"Saving output file: {filepath}", show_time=True)
-            output.to_csv(filepath, index=False)
-
-        if settings["SAVE_DIAGNOSTIC"]:
-            filepath = f"output/{timestamp}_diagnostic.csv"
-            print_log(f"Saving diagnostic file: {filepath}", show_time=True)
-            diagnostic.to_csv(filepath, index=False)
-
-        if settings["SAVE_LOG"]:
-            filepath = f"output/{timestamp}_log.txt"
-            print_log(f"Saving log file: {filepath}", show_time=True)
-            save_log_to_file(timestamp)
+    save_results(timestamp, output, diagnostic, settings)
 
     print(f"{'-' * 72}\n")
     return output
```

### Comparing `cashflower-0.7.0/cashflower.egg-info/PKG-INFO` & `cashflower-0.7.1/cashflower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.7.0
+Version: 0.7.1
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 License: UNKNOWN
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
@@ -34,14 +34,15 @@
 ```
 pip install cashflower
 ```
 
 ## Create model
 
 *python console*
+
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
 Creates:
```

### Comparing `cashflower-0.7.0/cashflower.egg-info/SOURCES.txt` & `cashflower-0.7.1/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.7.0/setup.py` & `cashflower-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
         'Cheat sheet': 'https://www.acturtle.com/static/pdf/cheat_sheet.pdf',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.7.0",
+    version="0.7.1",
 )
```

