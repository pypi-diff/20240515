# Comparing `tmp/okn_py_updater-2.0.3.tar.gz` & `tmp/okn_py_updater-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-2.0.3.tar", last modified: Wed May 15 03:04:17 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.4.tar", last modified: Wed May 15 09:25:18 2024, max compression
```

## Comparing `okn_py_updater-2.0.3.tar` & `okn_py_updater-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.392922 okn_py_updater-2.0.3/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-15 03:04:17.391925 okn_py_updater-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/README.md
--rw-rw-rw-   0        0        0      657 2024-05-15 03:04:04.000000 okn_py_updater-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 03:04:17.392922 okn_py_updater-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.368985 okn_py_updater-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.373973 okn_py_updater-2.0.3/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    20296 2024-05-15 03:03:43.000000 okn_py_updater-2.0.3/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.390927 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-15 03:12:37.000000 okn_py_updater-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:25:18.032984 okn_py_updater-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.010870 okn_py_updater-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.014183 okn_py_updater-2.0.4/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.4/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    24885 2024-05-15 09:24:08.000000 okn_py_updater-2.0.4/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:25:18.031987 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 09:25:17.000000 okn_py_updater-2.0.4/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-2.0.3/LICENSE` & `okn_py_updater-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.3/PKG-INFO` & `okn_py_updater-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-2.0.3/README.md` & `okn_py_updater-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.3/pyproject.toml` & `okn_py_updater-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-2.0.3/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.4/src/okn_py_updater/okn_py_updater.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import collections
+import math
+
 import numpy as np
 # from scipy.signal import medfilt
 import statistics
 
 
-def live_dispatch_function(filter_config_info, data_dict_input):
+def live_dispatch_function(filter_config_info, data_dict_input, pre_x_nom=0, pre_y_nom=0, pre_time=0, n_value=5):
     match_item = filter_config_info["function"]
     # print(f"Dispatched function name: {match_item}")
     if match_item == 'cdp_direction':
         # t = data_dict_input[filter_config_info["input"]]
         # # need to be fixed ********
         # keyname = "need to be fixed"
         # f = cdp_direction(config_info.log, keyname, t)
@@ -93,17 +95,17 @@
         f = data_dict_input[input_column]
         n = filter_config_info["npoint"]
         if n <= 1:
             raise ValueError("Median Filter: kernel value n must be greater than 1.")
         elif n % 2 == 0:
             raise ValueError("Median Filter: kernel value n must be odd number.")
         if len(f) >= n:
-            last_n_number_array = f[-n:]
+            last_n_number_array = f[:n]
             median_value = statistics.median(last_n_number_array)
-            f[-1] = median_value
+            f[0] = median_value
             data_dict_input[filter_config_info["output"]] = f
         else:
             data_dict_input[filter_config_info["output"]] = f
 
     elif match_item == 'replaceNanBy':
         input_column = filter_config_info["input"][0]
         input_array = data_dict_input[input_column]
@@ -123,18 +125,41 @@
         pass
 
     elif match_item == 'gradient':
         related_column_name_array = filter_config_info["input"]
         f = data_dict_input[related_column_name_array[1]]
         t = data_dict_input[related_column_name_array[0]]
         output_column = filter_config_info["output"]
-        o = data_dict_input[output_column]
-        data_dict_input[output_column] = live_gradient(f, t, o)
-        # # Not tested in live updater
-        # pass
+        # o = data_dict_input[output_column]
+        # data_dict_input[output_column] = live_gradient(f, t, o)
+        if len(f) >= n_value + 2:
+            if "updated_x" in related_column_name_array[1]:
+                f0 = pre_x_nom
+                t0 = pre_time
+                t0 = t[1]
+                f2 = statistics.median(f[1:n_value + 1])
+                # t2 = t[1]
+                t2 = t[3]
+                out_array = data_dict_input[output_column]
+                out_array[0] = (f2 - f0) / (t2 - t0)
+                data_dict_input[output_column] = out_array
+            elif "updated_y" in related_column_name_array[1]:
+                f0 = pre_y_nom
+                t0 = pre_time
+                t0 = t[1]
+                f2 = statistics.median(f[1:n_value + 1])
+                t2 = t[1]
+                t2 = t[3]
+                out_array = data_dict_input[output_column]
+                out_array[0] = (f2 - f0) / (t2 - t0)
+                data_dict_input[output_column] = out_array
+            else:
+                pass
+                # # Not tested in live updater
+        # print(grad(f, t))
 
     else:
         print(f"Function:{match_item} is not found")
 
     return data_dict_input
 
 
@@ -257,87 +282,115 @@
 
 def dshift(f):
     y = np.nanmean(f)
     f1 = f - y
     return f1
 
 
-def live_gradient(f, t, o):
-    f_length = len(f)
-    t_length = len(t)
-    if f_length == t_length:
-        if f_length < 3:
-            if f_length <= 0:
-                pass
-            else:
-                return f_length * [0]
-        else:
-            df = (f[2] - f[0]) / 2
-            dt = (t[2] - t[0]) / 2
-            dfdt = df / dt
-            o[1] = dfdt
-            return o
-    else:
-        raise ValueError("Displacement and time array lengths must be the same.")
-
-# def live_gradient(f, t):
+def grad(f, t):
+    try:
+        df = np.gradient(f)
+        dt = np.gradient(t)
+        dfdt = df / dt
+        # print("dfdt", dfdt)
+        for ind, value in enumerate(dfdt):
+            if math.isinf(value):
+                dfdt[ind] = 0
+            if np.isnan(value):
+                dfdt[ind] = 0
+        return dfdt
+    except ValueError:
+        return 0
+    except RuntimeWarning:
+        return 0
+
+
+# def live_gradient(f, t, out_array):
+#     # print("live grad")
+#     # print(f)
+#     # print(t)
+#     # print(out_array)
 #     f_length = len(f)
 #     t_length = len(t)
 #     if f_length == t_length:
-#         if f_length > 0:
-#             data_info_array = []
-#             for pos, time in zip(f, t):
-#                 temp_dict = {}
-#                 temp_dict["position"] = float(pos)
-#                 temp_dict["time"] = float(time)
-#                 data_info_array.append(temp_dict)
-#             info_array_length = len(data_info_array)
-#             if info_array_length > 2:
-#                 return_array = []
-#                 for ind in range(info_array_length):
-#                     if ind == 0:
-#                         return_array.append(0)
-#                     elif ind == 1:
-#                         edge_grad_val = grad_by_edge_equation(data_info_array[0],
-#                                                               data_info_array[1])
-#                         return_array.append(edge_grad_val)
-#                     else:
-#                         interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
-#                                                                       data_info_array[ind - 1],
-#                                                                       data_info_array[ind])
-#                         return_array.append(interior_grad_val)
-#                 return return_array
+#         if f_length < 3:
+#             if f_length <= 0:
+#                 pass
 #             else:
-#                 if info_array_length == 2:
-#                     edge_grad_val = grad_by_edge_equation(data_info_array[0],
-#                                                           data_info_array[1])
-#                     return [0, edge_grad_val]
-#                 else:
-#                     if info_array_length == 1:
-#                         return [0]
-#                     else:
-#                         pass
+#                 return out_array
+#         else:
+#             max_index = f_length - 1
+#             mid_index = f_length - 2
+#             min_index = f_length - 3
+#             df = (f[max_index] - f[min_index]) / 2
+#             dt = (t[max_index] - t[min_index]) / 2
+#             dfdt = df / dt
+#             # print(dfdt)
+#             out_array[mid_index] = dfdt
+#             # print("Grad", out_array)
+#             return out_array
 #     else:
 #         raise ValueError("Displacement and time array lengths must be the same.")
 
 
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
 def grad_by_edge_equation(first_ele, second_ele):
     displacement = second_ele["position"] - first_ele["position"]
     time_diff = second_ele["time"] - first_ele["time"]
     return displacement / time_diff
 
 
 def grad_by_interior_equation(first_ele, second_ele, third_ele):
     hs = third_ele["time"] - second_ele["time"]
     hd = second_ele["time"] - first_ele["time"]
     f2 = third_ele["position"]
     f1 = second_ele["position"]
     f0 = first_ele["position"]
     return ((np.square(hs) * f2) + ((np.square(hd) - np.square(hs)) * f1) - (np.square(hd) * f0)) / (
-                hs * hd * (hd + hs))
+            hs * hd * (hd + hs))
 
 
 def cdp_direction(logs, fname, t):
     return t
 
 
 def are_all_elements_nan(input_array):
@@ -354,23 +407,30 @@
     #         shifted_array = np.roll(input_array, shift=shift, axis=axis)
     #         idx = ~shifted_array.mask * input_array.mask
     #         input_array[idx] = shifted_array[idx]
     return input_array
 
 
 def get_out_header_array(header_array_input, filter_config_input):
+    data_id_array = ["id"]
+    print(data_id_array)
     output_header_array = [header for header in header_array_input]
+    print(output_header_array)
+    output_header_array = data_id_array + output_header_array
+    print(output_header_array)
     for filter_info in filter_config_input:
         if filter_info["Enabled"]:
             try:
                 output_header = filter_info["output"]
             except KeyError:
                 output_header = None
-            if output_header and output_header not in output_header_array:
-                output_header_array.append(output_header)
+            if output_header is not None:
+                if output_header not in output_header_array:
+                    print(output_header)
+                    output_header_array.append(output_header)
 
     return output_header_array
 
 
 class Updater:
     def __init__(self, config, circular_buffer_length, header_array, drop_rate=0):
         if type(config) is not dict:
@@ -397,105 +457,161 @@
         self.filter_config = filter_config
         self.circular_buffer = collections.deque(maxlen=circular_buffer_length)
         self.buffer_max_length = circular_buffer_length
         self.header_array = header_array
         self.out_header_array = get_out_header_array(header_array, filter_config)
         self.data_drop_rate = drop_rate
         self.currently_working_function = ['passthrough', 'medianFilter', 'replaceNanBy', 'gradient']
+        self.count = 0
+        self.data_id = 1
+        self.pre_x_nom = 0
+        self.pre_y_nom = 0
+        self.pre_time = 0
+        self.n_value = 5
         for filter_info in self.filter_config:
             if filter_info["Enabled"]:
                 function_name = filter_info["function"]
                 if function_name not in self.currently_working_function:
                     if function_name == 'dwnsample':
                         print(f"The function \"dwnsample\" is implemented as drop rate in live updater.")
                     else:
                         print(f"The function \"{function_name}\" is not available in live updater.")
+                else:
+                    if function_name == 'medianFilter':
+                        n_point = filter_info["npoint"]
+                        self.n_value = n_point
             else:
                 pass
-        self.count = 0
 
     def update(self, data_input):
         if self.data_drop_rate == 0:
-            self.circular_buffer.append(data_input)
+            data_input.insert(0, self.data_id)
+            self.data_id += 1
+            temp_dict = {}
+            for header_index, header_name in enumerate(self.out_header_array):
+                try:
+                    temp_dict[header_name] = data_input[header_index]
+                except IndexError:
+                    temp_dict[header_name] = 0
             data_dict = {}
-            output_data = []
-            for header in self.header_array:
+            for header in self.out_header_array:
                 data_dict[header] = []
-            for data in self.circular_buffer:
-                for header_index, header_string in enumerate(self.header_array):
-                    data_dict[header_string].append(float(data[header_index]))
+
+            self.circular_buffer.append(temp_dict)
+            for header in data_dict:
+                for data in self.circular_buffer:
+                    data_dict[header].append(data[header])
 
             # if len(self.circular_buffer) >= 3:
             for filter_info in self.filter_config:
                 if filter_info["Enabled"]:
-                    data_dict = live_dispatch_function(filter_info, data_dict)
-                else:
-                    pass
+                    data_dict = live_dispatch_function(filter_info,
+                                                       data_dict,
+                                                       pre_x_nom=self.pre_x_nom,
+                                                       pre_y_nom=self.pre_y_nom,
+                                                       pre_time=self.pre_time,
+                                                       n_value=self.n_value)
 
+            converting_array = []
             for index in range(len(data_dict[self.out_header_array[0]])):
-                temp_array = []
+                temp_dict = {}
                 for header in self.out_header_array:
-                    try:
-                        temp_array.append(data_dict[header][index])
-                    except KeyError:
-                        temp_array.append(0)
-                    except TypeError:
-                        temp_array.append(0)
-                output_data.append(temp_array)
-                # len_diff = len(output_header_array) - len(self.header_array)
-                # for data in self.circular_buffer:
-                #     temp_array = [ele for ele in data]
-                #     temp_array.extend(len_diff * [0])
-                #     output_data.append(temp_array)
+                    temp_dict[header] = (data_dict[header][index])
+                converting_array.append(temp_dict)
 
-            # print("output_data")
-            # for d in output_data:
+            # print("C before")
+            # for d in self.circular_buffer:
             #     print(d)
-            # print("end")
-            return output_data[-1]
+            # print("C before")
+            for d_dict in self.circular_buffer:
+                d_id = d_dict["id"]
+                for con_dict in converting_array:
+                    con_id = con_dict["id"]
+                    if d_id == con_id:
+                        for att in d_dict:
+                            d_dict[att] = con_dict[att]
+                        break
+            # print("C After")
+            # for d in self.circular_buffer:
+            #     print(d)
+            # print("C After")
+
+            first_data = self.circular_buffer[0]
+            self.pre_x_nom = first_data["updated_x_nom"]
+            self.pre_y_nom = first_data["updated_y_nom"]
+            self.pre_time = first_data["record_timestamp"]
+            out_array = []
+            for header in self.out_header_array:
+                out_array.append(first_data[header])
+            return out_array
         else:
             if self.count == 0:
-                self.circular_buffer.append(data_input)
+                data_input.insert(0, self.data_id)
+                self.data_id += 1
+                temp_dict = {}
+                for header_index, header_name in enumerate(self.out_header_array):
+                    try:
+                        temp_dict[header_name] = data_input[header_index]
+                    except IndexError:
+                        temp_dict[header_name] = 0
                 data_dict = {}
-                output_data = []
-                for header in self.header_array:
+                for header in self.out_header_array:
                     data_dict[header] = []
-                for data in self.circular_buffer:
-                    for header_index, header_string in enumerate(self.header_array):
-                        data_dict[header_string].append(float(data[header_index]))
+
+                self.circular_buffer.append(temp_dict)
+                for header in data_dict:
+                    for data in self.circular_buffer:
+                        data_dict[header].append(data[header])
 
                 # if len(self.circular_buffer) >= 3:
                 for filter_info in self.filter_config:
                     if filter_info["Enabled"]:
-                        data_dict = live_dispatch_function(filter_info, data_dict)
-                    else:
-                        pass
+                        data_dict = live_dispatch_function(filter_info,
+                                                           data_dict,
+                                                           pre_x_nom=self.pre_x_nom,
+                                                           pre_y_nom=self.pre_y_nom,
+                                                           pre_time=self.pre_time,
+                                                           n_value=self.n_value)
 
+                converting_array = []
                 for index in range(len(data_dict[self.out_header_array[0]])):
-                    temp_array = []
+                    temp_dict = {}
                     for header in self.out_header_array:
-                        try:
-                            temp_array.append(data_dict[header][index])
-                        except KeyError:
-                            temp_array.append(0)
-                        except TypeError:
-                            temp_array.append(0)
-                    output_data.append(temp_array)
-                    # len_diff = len(output_header_array) - len(self.header_array)
-                    # for data in self.circular_buffer:
-                    #     temp_array = [ele for ele in data]
-                    #     temp_array.extend(len_diff * [0])
-                    #     output_data.append(temp_array)
+                        temp_dict[header] = (data_dict[header][index])
+                    converting_array.append(temp_dict)
 
-                # print("output_data")
-                # for d in output_data:
+                # print("C before")
+                # for d in self.circular_buffer:
+                #     print(d)
+                # print("C before")
+                for d_dict in self.circular_buffer:
+                    d_id = d_dict["id"]
+                    for con_dict in converting_array:
+                        con_id = con_dict["id"]
+                        if d_id == con_id:
+                            for att in d_dict:
+                                d_dict[att] = con_dict[att]
+                            break
+                # print("C After")
+                # for d in self.circular_buffer:
                 #     print(d)
-                # print("end")
+                # print("C After")
+
                 self.count = 1
-                return output_data[-1]
+                if len(self.circular_buffer) == self.buffer_max_length:
+                    first_data = self.circular_buffer[0]
+                    self.pre_x_nom = first_data["updated_x_nom"]
+                    self.pre_y_nom = first_data["updated_y_nom"]
+                    self.pre_time = first_data["record_timestamp"]
+                    out_array = []
+                    for header in self.out_header_array:
+                        out_array.append(first_data[header])
+                    return out_array
+                else:
+                    return None
             else:
                 if self.count < self.data_drop_rate:
                     self.count += 1
                 else:
                     self.count = 0
                 return None
```

### Comparing `okn_py_updater-2.0.3/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.4/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

