# Comparing `tmp/interactive_dir_utils-0.1.0.tar.gz` & `tmp/interactive_dir_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactive_dir_utils-0.1.0.tar", max compression
+gzip compressed data, was "interactive_dir_utils-0.1.1.tar", max compression
```

## Comparing `interactive_dir_utils-0.1.0.tar` & `interactive_dir_utils-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1090 2023-10-20 11:14:50.223939 interactive_dir_utils-0.1.0/License.txt
--rw-r--r--   0        0        0      441 2023-10-26 11:15:31.452622 interactive_dir_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      126 2023-10-26 11:03:31.916243 interactive_dir_utils-0.1.0/README.md
--rw-r--r--   0        0        0       50 2023-10-26 10:59:48.209730 interactive_dir_utils-0.1.0/src/interactive_dir_utils/__init__.py
--rw-r--r--   0        0        0     4380 2023-10-20 12:57:30.633850 interactive_dir_utils-0.1.0/src/interactive_dir_utils/data_dir_utils.py
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 interactive_dir_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-10-20 11:14:50.000000 interactive_dir_utils-0.1.1/License.txt
+-rw-r--r--   0        0        0      441 2024-05-15 09:46:57.487044 interactive_dir_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-10-26 11:03:31.000000 interactive_dir_utils-0.1.1/README.md
+-rw-r--r--   0        0        0       95 2024-05-15 09:48:53.019068 interactive_dir_utils-0.1.1/src/interactive_dir_utils/__init__.py
+-rw-r--r--   0        0        0     5704 2024-05-15 09:46:20.397355 interactive_dir_utils-0.1.1/src/interactive_dir_utils/data_dir_utils.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 interactive_dir_utils-0.1.1/PKG-INFO
```

### Comparing `interactive_dir_utils-0.1.0/License.txt` & `interactive_dir_utils-0.1.1/License.txt`

 * *Files identical despite different names*

### Comparing `interactive_dir_utils-0.1.0/src/interactive_dir_utils/data_dir_utils.py` & `interactive_dir_utils-0.1.1/src/interactive_dir_utils/data_dir_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,21 +34,50 @@
         print(f"{n + 1}: {option}")
         items[n + 1] = result
 
     selection = 0
     while selection not in items:
         selection = int(input(f"Enter {item_name} number: "))
 
-    if isinstance(obj, dict) or isinstance(obj, pd.DataFrame):
-        if key:
-            return items[selection]
+    if key or isinstance(obj, (list, tuple)):
+        return items[selection]
 
-        return obj[items[selection]]
+    return obj[items[selection]]
 
-    return items[selection]
+
+def select_options(objs: [list, tuple, dict, pd.DataFrame], item_name='item', key=False, extra_options: dict = None):
+    if not extra_options:
+        extra_options = {}
+
+    extra_options.update(Stop=False)
+
+    if isinstance(objs, tuple):
+        objs = list(objs)
+
+    options = []
+
+    while True:
+        if objs:
+            obj = select_option(objs, item_name, key=key, extra_options=extra_options)
+            if not obj:
+                break
+
+            if isinstance(objs, dict):
+                options.append(obj)
+                objs.pop(obj)
+            elif isinstance(objs, pd.DataFrame):
+                options.append(obj)
+                objs.drop(columns=obj, inplace=True)
+            else:
+                options.append(objs.pop(objs.index(obj)))
+
+        else:
+            break
+
+    return options
 
 
 def empty_directory(directory_path, excluded_entries: list = None, excluded_filetype: str = None):
     if not excluded_entries:
         excluded_entries = []
     # Check if the directory exists
     if not os.path.exists(directory_path):
@@ -71,53 +100,65 @@
             os.remove(entry_path)
 
         # Check if it's a directory and remove it recursively
         elif os.path.isdir(entry_path):
             shutil.rmtree(entry_path)
 
 
-def get_data_path(data_current_dir: str = None, file: str = None, exclude_list: list = None, file_format: str = ".csv"):
+def get_data_path(data_current_dir: str = None, file: str = None, exclude_list: list = None, file_format: str = ".csv",
+                  known_entries: list = None):
     if not data_current_dir:
         data_current_dir = os.getcwd()
+    elif not os.path.exists(data_current_dir):
+        print(f"Warning: {data_current_dir} does not exist, using current working directory.")
+        data_current_dir = os.getcwd()
 
     if not exclude_list:
         exclude_list = []
+        
+    if not known_entries:
+        known_entries = []
 
     data_path = data_current_dir
     for dirpath, dirnames, filenames in os.walk(data_current_dir):
-        # Interactively select which directory for the current household. Returns only one output.
+        # Interactively select which directory for the current household
         if dirpath == data_path:
             if dirnames:
-                options = list(filter(lambda dir_: dir_ not in exclude_list, dirnames))
-                data_path = os.path.join(data_path, select_option(options, "directory"))
+                if options := [element for element in known_entries if element in dirnames]:
+                    pass
+                else:
+                    options = list(filter(lambda dir_: dir_ not in exclude_list, dirnames))
+                
+                sub_dir = select_option(options, "directory")
+                data_path = os.path.join(data_path, sub_dir)
+                
             elif file:
                 assert file in filenames, f"{file} is not in {dirpath}."
                 return data_path, file
             else:
                 files = sorted(filter(lambda file_: os.path.splitext(file_)[1] == file_format, filenames))
                 file = select_option(files)
                 return data_path, file
 
 
-def get_file_path(current_dir: str = None, file_exts: list = None, extra_options: dict = None,
-                  exclude_list: list = None, dir_only: bool = False):
-    if not current_dir:
-        current_dir = os.getcwd()
-
-    if not exclude_list:
-        exclude_list = []
-
-    if not file_exts:
-        file_exts = [".csv"]
-
-    while True:
-        include_exts = (*file_exts, "")
-        options = [option for option in os.listdir(current_dir) if os.path.splitext(option)[1] in include_exts
-                   and option not in exclude_list]
-        sub_dir = select_option(options, extra_options=extra_options)
-        if not sub_dir or os.path.isfile(os.path.join(current_dir, sub_dir)):
-            if dir_only:
-                return current_dir
-
-            return current_dir, sub_dir
-
-        current_dir = os.path.join(current_dir, sub_dir)
+# def get_file_path(current_dir: str = None, file_exts: list = None, extra_options: dict = None,
+#                   exclude_list: list = None, dir_only: bool = False):
+#     if not current_dir:
+#         current_dir = os.getcwd()
+#
+#     if not exclude_list:
+#         exclude_list = []
+#
+#     if not file_exts:
+#         file_exts = [".csv"]
+#
+#     while True:
+#         options = [option for option in os.listdir(current_dir) if (os.path.splitext(option)[1] in file_exts
+#                    and option not in exclude_list) or os.path.isdir(os.path.join(current_dir, option))]
+#         sub_dir = select_option(options, extra_options=extra_options)
+#         if not sub_dir or os.path.isfile(os.path.join(current_dir, sub_dir)):
+#             if dir_only:
+#                 return current_dir
+#
+#             return current_dir, sub_dir
+#
+#         current_dir = os.path.join(current_dir, sub_dir)
```

### Comparing `interactive_dir_utils-0.1.0/PKG-INFO` & `interactive_dir_utils-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: interactive-dir-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility package containing functions for manipultaing and traversing data directories interactively.
 License: LICENSE.txt
 Author: corson94
 Author-email: jamie.corson.20@ucl.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.0.2)
 Description-Content-Type: text/markdown
 
 # Interactive-dir-utils
 
 Package to help traverse directories interactively to find files.
```

