# Comparing `tmp/okn_py_updater-2.0.1.tar.gz` & `tmp/okn_py_updater-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-2.0.1.tar", last modified: Mon May 13 22:48:32 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.2.tar", last modified: Wed May 15 01:32:38 2024, max compression
```

## Comparing `okn_py_updater-2.0.1.tar` & `okn_py_updater-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 22:48:32.513639 okn_py_updater-2.0.1/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-13 22:48:32.511644 okn_py_updater-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.1/README.md
--rw-rw-rw-   0        0        0      657 2024-05-13 22:47:54.000000 okn_py_updater-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 22:48:32.513639 okn_py_updater-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 22:48:32.475741 okn_py_updater-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 22:48:32.487709 okn_py_updater-2.0.1/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.1/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    17503 2024-05-13 22:47:54.000000 okn_py_updater-2.0.1/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-13 22:48:32.510647 okn_py_updater-2.0.1/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-13 22:48:32.000000 okn_py_updater-2.0.1/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-13 22:48:32.000000 okn_py_updater-2.0.1/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 22:48:32.000000 okn_py_updater-2.0.1/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 22:48:32.000000 okn_py_updater-2.0.1/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.526067 okn_py_updater-2.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-15 01:32:38.525069 okn_py_updater-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-15 01:32:26.000000 okn_py_updater-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 01:32:38.526067 okn_py_updater-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.494028 okn_py_updater-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.506510 okn_py_updater-2.0.2/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    19551 2024-05-15 01:31:58.000000 okn_py_updater-2.0.2/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.524073 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-2.0.1/LICENSE` & `okn_py_updater-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.1/PKG-INFO` & `okn_py_updater-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-2.0.1/README.md` & `okn_py_updater-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.1/pyproject.toml` & `okn_py_updater-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-2.0.1/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.2/src/okn_py_updater/okn_py_updater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections
 import numpy as np
-import math
 # from scipy.signal import medfilt
 import statistics
 
 
 def live_dispatch_function(filter_config_info, data_dict_input):
     match_item = filter_config_info["function"]
     # print(f"Dispatched function name: {match_item}")
@@ -124,15 +123,15 @@
         pass
 
     elif match_item == 'gradient':
         related_column_name_array = filter_config_info["input"]
         f = data_dict_input[related_column_name_array[1]]
         t = data_dict_input[related_column_name_array[0]]
         output_column = filter_config_info["output"]
-        data_dict_input[output_column] = grad(f, t)
+        data_dict_input[output_column] = live_gradient(f, t)
         # # Not tested in live updater
         # pass
 
     else:
         print(f"Function:{match_item} is not found")
 
     return data_dict_input
@@ -257,30 +256,69 @@
 
 def dshift(f):
     y = np.nanmean(f)
     f1 = f - y
     return f1
 
 
-def grad(f, t):
-    try:
-        df = np.gradient(f)
-        dt = np.gradient(t)
-        dfdt = df / dt
-        # print("dfdt", dfdt)
-        for ind, value in enumerate(dfdt):
-            if math.isinf(value):
-                dfdt[ind] = 0
-            if np.isnan(value):
-                dfdt[ind] = 0
-        return dfdt
-    except ValueError:
-        return 0
-    except RuntimeWarning:
-        return 0
+def live_gradient(f, t):
+    f_length = len(f)
+    t_length = len(t)
+    if f_length == t_length:
+        if f_length > 0:
+            data_info_array = []
+            for pos, time in zip(f, t):
+                temp_dict = {}
+                temp_dict["position"] = float(pos)
+                temp_dict["time"] = float(time)
+                data_info_array.append(temp_dict)
+            info_array_length = len(data_info_array)
+            if info_array_length > 2:
+                return_array = []
+                for ind in range(info_array_length):
+                    if ind == 0:
+                        return_array.append(0)
+                    elif ind == 1:
+                        edge_grad_val = grad_by_edge_equation(data_info_array[0],
+                                                              data_info_array[1])
+                        return_array.append(edge_grad_val)
+                    else:
+                        interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
+                                                                      data_info_array[ind - 1],
+                                                                      data_info_array[ind])
+                        return_array.append(interior_grad_val)
+                return return_array
+            else:
+                if info_array_length == 2:
+                    edge_grad_val = grad_by_edge_equation(data_info_array[0],
+                                                          data_info_array[1])
+                    return [0, edge_grad_val]
+                else:
+                    if info_array_length == 1:
+                        return [0]
+                    else:
+                        pass
+    else:
+        raise ValueError("Displacement and time array lengths must be the same.")
+
+
+def grad_by_edge_equation(first_ele, second_ele):
+    displacement = second_ele["position"] - first_ele["position"]
+    time_diff = second_ele["time"] - first_ele["time"]
+    return displacement / time_diff
+
+
+def grad_by_interior_equation(first_ele, second_ele, third_ele):
+    hs = third_ele["time"] - second_ele["time"]
+    hd = second_ele["time"] - first_ele["time"]
+    f2 = third_ele["position"]
+    f1 = second_ele["position"]
+    f0 = first_ele["position"]
+    return ((np.square(hs) * f2) + ((np.square(hd) - np.square(hs)) * f1) - (np.square(hd) * f0)) / (
+                hs * hd * (hd + hs))
 
 
 def cdp_direction(logs, fname, t):
     return t
 
 
 def are_all_elements_nan(input_array):
```

### Comparing `okn_py_updater-2.0.1/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.2/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

