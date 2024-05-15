# Comparing `tmp/okn_py_updater-2.0.2.tar.gz` & `tmp/okn_py_updater-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okn_py_updater-2.0.2.tar", last modified: Wed May 15 01:32:38 2024, max compression
+gzip compressed data, was "okn_py_updater-2.0.3.tar", last modified: Wed May 15 03:04:17 2024, max compression
```

## Comparing `okn_py_updater-2.0.2.tar` & `okn_py_updater-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.526067 okn_py_updater-2.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     3706 2024-05-15 01:32:38.525069 okn_py_updater-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/README.md
--rw-rw-rw-   0        0        0      657 2024-05-15 01:32:26.000000 okn_py_updater-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 01:32:38.526067 okn_py_updater-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.494028 okn_py_updater-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.506510 okn_py_updater-2.0.2/src/okn_py_updater/
--rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.2/src/okn_py_updater/__init__.py
--rw-rw-rw-   0        0        0    19551 2024-05-15 01:31:58.000000 okn_py_updater-2.0.2/src/okn_py_updater/okn_py_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-15 01:32:38.524073 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/
--rw-rw-rw-   0        0        0     3706 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 01:32:38.000000 okn_py_updater-2.0.2/src/okn_py_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.392922 okn_py_updater-2.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3706 2024-05-15 03:04:17.391925 okn_py_updater-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/README.md
+-rw-rw-rw-   0        0        0      657 2024-05-15 03:04:04.000000 okn_py_updater-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 03:04:17.392922 okn_py_updater-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.368985 okn_py_updater-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.373973 okn_py_updater-2.0.3/src/okn_py_updater/
+-rw-rw-rw-   0        0        0        0 2024-05-06 22:12:10.000000 okn_py_updater-2.0.3/src/okn_py_updater/__init__.py
+-rw-rw-rw-   0        0        0    20296 2024-05-15 03:03:43.000000 okn_py_updater-2.0.3/src/okn_py_updater/okn_py_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-15 03:04:17.390927 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/
+-rw-rw-rw-   0        0        0     3706 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 03:04:17.000000 okn_py_updater-2.0.3/src/okn_py_updater.egg-info/top_level.txt
```

### Comparing `okn_py_updater-2.0.2/LICENSE` & `okn_py_updater-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.2/PKG-INFO` & `okn_py_updater-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `okn_py_updater-2.0.2/README.md` & `okn_py_updater-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `okn_py_updater-2.0.2/pyproject.toml` & `okn_py_updater-2.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "okn_py_updater"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for OKN Data Updater"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `okn_py_updater-2.0.2/src/okn_py_updater/okn_py_updater.py` & `okn_py_updater-2.0.3/src/okn_py_updater/okn_py_updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,16 @@
         pass
 
     elif match_item == 'gradient':
         related_column_name_array = filter_config_info["input"]
         f = data_dict_input[related_column_name_array[1]]
         t = data_dict_input[related_column_name_array[0]]
         output_column = filter_config_info["output"]
-        data_dict_input[output_column] = live_gradient(f, t)
+        o = data_dict_input[output_column]
+        data_dict_input[output_column] = live_gradient(f, t, o)
         # # Not tested in live updater
         # pass
 
     else:
         print(f"Function:{match_item} is not found")
 
     return data_dict_input
@@ -256,54 +257,72 @@
 
 def dshift(f):
     y = np.nanmean(f)
     f1 = f - y
     return f1
 
 
-def live_gradient(f, t):
+def live_gradient(f, t, o):
     f_length = len(f)
     t_length = len(t)
     if f_length == t_length:
-        if f_length > 0:
-            data_info_array = []
-            for pos, time in zip(f, t):
-                temp_dict = {}
-                temp_dict["position"] = float(pos)
-                temp_dict["time"] = float(time)
-                data_info_array.append(temp_dict)
-            info_array_length = len(data_info_array)
-            if info_array_length > 2:
-                return_array = []
-                for ind in range(info_array_length):
-                    if ind == 0:
-                        return_array.append(0)
-                    elif ind == 1:
-                        edge_grad_val = grad_by_edge_equation(data_info_array[0],
-                                                              data_info_array[1])
-                        return_array.append(edge_grad_val)
-                    else:
-                        interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
-                                                                      data_info_array[ind - 1],
-                                                                      data_info_array[ind])
-                        return_array.append(interior_grad_val)
-                return return_array
+        if f_length < 3:
+            if f_length <= 0:
+                pass
             else:
-                if info_array_length == 2:
-                    edge_grad_val = grad_by_edge_equation(data_info_array[0],
-                                                          data_info_array[1])
-                    return [0, edge_grad_val]
-                else:
-                    if info_array_length == 1:
-                        return [0]
-                    else:
-                        pass
+                return f_length * [0]
+        else:
+            df = (f[2] - f[0]) / 2
+            dt = (t[2] - t[0]) / 2
+            dfdt = df / dt
+            o[1] = dfdt
+            return o
     else:
         raise ValueError("Displacement and time array lengths must be the same.")
 
+# def live_gradient(f, t):
+#     f_length = len(f)
+#     t_length = len(t)
+#     if f_length == t_length:
+#         if f_length > 0:
+#             data_info_array = []
+#             for pos, time in zip(f, t):
+#                 temp_dict = {}
+#                 temp_dict["position"] = float(pos)
+#                 temp_dict["time"] = float(time)
+#                 data_info_array.append(temp_dict)
+#             info_array_length = len(data_info_array)
+#             if info_array_length > 2:
+#                 return_array = []
+#                 for ind in range(info_array_length):
+#                     if ind == 0:
+#                         return_array.append(0)
+#                     elif ind == 1:
+#                         edge_grad_val = grad_by_edge_equation(data_info_array[0],
+#                                                               data_info_array[1])
+#                         return_array.append(edge_grad_val)
+#                     else:
+#                         interior_grad_val = grad_by_interior_equation(data_info_array[ind - 2],
+#                                                                       data_info_array[ind - 1],
+#                                                                       data_info_array[ind])
+#                         return_array.append(interior_grad_val)
+#                 return return_array
+#             else:
+#                 if info_array_length == 2:
+#                     edge_grad_val = grad_by_edge_equation(data_info_array[0],
+#                                                           data_info_array[1])
+#                     return [0, edge_grad_val]
+#                 else:
+#                     if info_array_length == 1:
+#                         return [0]
+#                     else:
+#                         pass
+#     else:
+#         raise ValueError("Displacement and time array lengths must be the same.")
+
 
 def grad_by_edge_equation(first_ele, second_ele):
     displacement = second_ele["position"] - first_ele["position"]
     time_diff = second_ele["time"] - first_ele["time"]
     return displacement / time_diff
 
 
@@ -358,14 +377,16 @@
             raise ValueError("The config input must be dictionary type.")
         try:
             filter_config = config["filters"]
         except KeyError:
             raise KeyError("The config info does not contain filter info.")
         if type(circular_buffer_length) is not int:
             raise ValueError("The circular buffer length input must be integer type.")
+        if circular_buffer_length < 3:
+            raise ValueError("The circular buffer length must be at least 3.")
         if type(header_array) is not list:
             raise ValueError("The header array input must be list type.")
         if not header_array:
             raise ValueError("The header array input must not be empty.")
         if type(drop_rate) is not int:
             raise ValueError("The drop rate input must be integer type.")
         for header in header_array:
```

### Comparing `okn_py_updater-2.0.2/src/okn_py_updater.egg-info/PKG-INFO` & `okn_py_updater-2.0.3/src/okn_py_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okn_py_updater
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python Library for OKN Data Updater
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/okn_data_updater
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/okn_data_updater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

