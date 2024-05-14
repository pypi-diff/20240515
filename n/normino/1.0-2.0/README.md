# Comparing `tmp/normino-1.0.tar.gz` & `tmp/normino-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normino-1.0.tar", last modified: Mon May 13 17:49:36 2024, max compression
+gzip compressed data, was "normino-2.0.tar", last modified: Tue May 14 22:47:46 2024, max compression
```

## Comparing `normino-1.0.tar` & `normino-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 smasse   (101271) 2024_luxembourg  (4224)        0 2024-05-13 17:49:36.706917 normino-1.0/
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     2232 2024-05-13 17:49:36.706917 normino-1.0/PKG-INFO
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     1766 2024-05-13 07:42:01.000000 normino-1.0/README.md
-drwxr-xr-x   0 smasse   (101271) 2024_luxembourg  (4224)        0 2024-05-13 17:49:36.706917 normino-1.0/normino.egg-info/
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     2232 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/PKG-INFO
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)      217 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/SOURCES.txt
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        1 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/dependency_links.txt
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)       42 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/entry_points.txt
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        9 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/requires.txt
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        8 2024-05-13 17:49:36.000000 normino-1.0/normino.egg-info/top_level.txt
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     6555 2024-05-13 17:47:19.000000 normino-1.0/normino.py
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)       38 2024-05-13 17:49:36.706917 normino-1.0/setup.cfg
--rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)      781 2024-05-13 17:49:07.000000 normino-1.0/setup.py
+drwxr-xr-x   0 smasse   (101271) 2024_luxembourg  (4224)        0 2024-05-14 22:47:46.548399 normino-2.0/
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     2232 2024-05-14 22:47:46.544399 normino-2.0/PKG-INFO
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     1766 2024-05-14 18:04:36.000000 normino-2.0/README.md
+drwxr-xr-x   0 smasse   (101271) 2024_luxembourg  (4224)        0 2024-05-14 22:47:46.544399 normino-2.0/normino.egg-info/
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     2232 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/PKG-INFO
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)      217 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/SOURCES.txt
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        1 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/dependency_links.txt
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)       42 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/entry_points.txt
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        9 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/requires.txt
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)        8 2024-05-14 22:47:46.000000 normino-2.0/normino.egg-info/top_level.txt
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)     8139 2024-05-14 22:43:06.000000 normino-2.0/normino.py
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)       38 2024-05-14 22:47:46.548399 normino-2.0/setup.cfg
+-rw-r--r--   0 smasse   (101271) 2024_luxembourg  (4224)      781 2024-05-14 22:46:36.000000 normino-2.0/setup.py
```

### Comparing `normino-1.0/PKG-INFO` & `normino-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normino
-Version: 1.0
+Version: 2.0
 Summary: UNKNOWN
 Home-page: https://github.com/SLDDL/Normino
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/SLDDL/Normino/blob/main/README.md
 Project-URL: Source, https://github.com/SLDDL/Normino
 Project-URL: Tracker, https://github.com/SLDDL/Normino/issues
 Project-URL: Icon, https://raw.githubusercontent.com/SLDDL/Normino/main/icon.png
```

### Comparing `normino-1.0/README.md` & `normino-2.0/README.md`

 * *Files identical despite different names*

### Comparing `normino-1.0/normino.egg-info/PKG-INFO` & `normino-2.0/normino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normino
-Version: 1.0
+Version: 2.0
 Summary: UNKNOWN
 Home-page: https://github.com/SLDDL/Normino
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/SLDDL/Normino/blob/main/README.md
 Project-URL: Source, https://github.com/SLDDL/Normino
 Project-URL: Tracker, https://github.com/SLDDL/Normino/issues
 Project-URL: Icon, https://raw.githubusercontent.com/SLDDL/Normino/main/icon.png
```

### Comparing `normino-1.0/normino.py` & `normino-2.0/normino.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,54 @@
 init(autoreset=True)
 
 
 def colorize_text(text, color):
     return f"{color}{text}{Style.RESET_ALL}"
 
 
-def display_errors(errors):
-    for error in errors:
-        print(error)
+def display_errors(errors, detailed):
+    column_width = shutil.get_terminal_size().columns
+    if column_width > 137 and not detailed:
+        column_width //= 2
+        print(errors[0])
+        for i in range(1, len(errors), 2):
+            left = textwrap.fill(
+                errors[i], width=column_width, subsequent_indent='    ')
+            right = textwrap.fill(errors[i + 1] if i + 1 < len(errors)
+                                  else '', width=column_width, subsequent_indent='    ')
+            print(f"{left:<{column_width}}{right}")
+    else:
+        for error in errors:
+            print(error)
 
 
-def find_c_and_h_files(path):
-    if not path:
-        path = "."
-    command = ["find", path, "-type", "f",
-               "(", "-name", "*.c", "-o", "-name", "*.h", ")"]
-    result = subprocess.run(
-        command, text=True, capture_output=True, check=True)
-    files = result.stdout.strip().split('\n')
-    return [file for file in files if file]
+def find_c_and_h_files(path, excludes):
+    find_all_command = ["find", path, "-type", "f","(", "-name", "*.c", "-o", "-name", "*.h", ")"]
+    try:
+        result_all = subprocess.run(
+            find_all_command, text=True, capture_output=True, check=True)
+        all_files = result_all.stdout.strip().split('\n')
+    except subprocess.CalledProcessError as e:
+        print(colorize_text(
+            f"Error during file search: {e.stderr.strip()}", Fore.RED))
+        exit(1)
+    excluded_files = set()
+    for pattern in excludes:
+        find_exclude_command = ["find", pattern, "-type",
+                                "f", "(", "-name", "*.c", "-o", "-name", "*.h", ")"]
+        try:
+            result_exclude = subprocess.run(
+                find_exclude_command, text=True, capture_output=True, check=True)
+            excluded_files.update(result_exclude.stdout.strip().split('\n'))
+        except subprocess.CalledProcessError as e:
+            print(colorize_text(
+                f"Error during exclusion search: {e.stderr.strip()}", Fore.RED))
+    included_files = [
+        file for file in all_files if file and file not in excluded_files]
+    return included_files
 
 
 def check_file(file, detailed):
     cmd = ["norminette", file]
     try:
         result = subprocess.run(
             cmd, capture_output=True, text=True, timeout=5)
@@ -98,15 +124,15 @@
         if errors_by_file:
             print(colorize_text(
                 "══════════════[ FAIL ]══════════════════", Fore.RED))
             print(colorize_text(
                 "File    Line    Col    Error Description", Fore.YELLOW))
             errors_by_file.sort
             for file, errors in errors_by_file:
-                display_errors(errors)
+                display_errors(errors, detailed)
         if files_failed:
             print("══════════════[ FAILED ]════════════════")
             files_failed.sort(key=lambda x: x[0])
             for file, msg in files_failed:
                 wrapped_failed_msg = textwrap.fill(colorize_text(
                     f"{file}: {msg}", Fore.YELLOW), width=shutil.get_terminal_size().columns, break_on_hyphens=False)
                 print("\n".join(wrapped_failed_msg.split("\n")))
@@ -127,26 +153,28 @@
         f"Execution time: {execution_time:.2f} seconds", Fore.BLUE))
 
 
 def main():
     parser = argparse.ArgumentParser(description="Run norminette but better!")
     parser.add_argument("paths", nargs="*", default=["."],
                         help="Space-separated directory paths or shell patterns like '*.c'. Default is current directory.")
+    parser.add_argument("-x", "--exclude", nargs="*", default=[],
+                    help="Space-separated list of file patterns to exclude. Example usage: --exclude '*.tmp' 'test/*'")
     parser.add_argument("-e", "--error_only", action="store_true",
                         help="Display only errors.")
     parser.add_argument("-s", "--summary_only", action="store_true",
                         help="Display only the summary.")
     parser.add_argument("-d", "--detailed", action="store_true",
                         help="Display detailed error messages.")
     parser.add_argument("-l", "--list_files", action="store_true",
                         help="List all found .c and .h files and exit.")
     args = parser.parse_args()
     all_files = []
     for path in args.paths:
-        all_files.extend(find_c_and_h_files(path))
+        all_files.extend(find_c_and_h_files(path, args.exclude))
     if args.list_files:
         for file in all_files:
             print(file)
     else:
         run_norminette(all_files, args.error_only,
                        args.summary_only, args.detailed)
```

### Comparing `normino-1.0/setup.py` & `normino-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='normino',
-    version='1.0',
+    version='2.0',
     url='https://github.com/SLDDL/Normino',
     py_modules=['normino'],
     install_requires=[
         'colorama',
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

