# Comparing `tmp/WrenchCL-1.9.0.tar.gz` & `tmp/WrenchCL-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-1.9.0.tar", last modified: Fri Feb 23 08:11:26 2024, max compression
+gzip compressed data, was "WrenchCL-1.9.1.tar", last modified: Wed Mar  6 21:33:46 2024, max compression
```

## Comparing `WrenchCL-1.9.0.tar` & `WrenchCL-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:11:26.075953 WrenchCL-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-02-23 08:11:26.075953 WrenchCL-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:11:26.071953 WrenchCL-1.9.0/WrenchCL/
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/ApiSuperClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/ChatGptSuperClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/RdsSuperClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:11:26.075953 WrenchCL-1.9.0/WrenchCL/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/Utility/ConsoleAnimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/Utility/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24803 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-23 08:10:57.000000 WrenchCL-1.9.0/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 08:11:26.075953 WrenchCL-1.9.0/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-02-23 08:11:26.000000 WrenchCL-1.9.0/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-23 08:11:26.000000 WrenchCL-1.9.0/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 08:11:26.000000 WrenchCL-1.9.0/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-23 08:11:26.000000 WrenchCL-1.9.0/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 08:11:26.000000 WrenchCL-1.9.0/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 08:11:26.075953 WrenchCL-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-23 08:11:24.000000 WrenchCL-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.109665 WrenchCL-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL/
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/ApiSuperClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/ChatGptSuperClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/RdsSuperClass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/ConsoleAnimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:33:46.109665 WrenchCL-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-06 21:33:44.000000 WrenchCL-1.9.1/setup.py
```

### Comparing `WrenchCL-1.9.0/PKG-INFO` & `WrenchCL-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 1.9.0
+Version: 1.9.1
 Summary: This is a code library designed to improve code re-usability and standardize access to APIs, RDS, and logging functionalities
 Author: willem@wrench.ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: pandas>=2.1.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 1.9.0 Summary: This is a code
+Metadata-Version: 2.1 Name: WrenchCL Version: 1.9.1 Summary: This is a code
 library designed to improve code re-usability and standardize access to APIs,
 RDS, and logging functionalities Author: willem@wrench.ai Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Requires-Dist: setuptools>=68.0.0
 Requires-Dist: colorama>=0.4.6 Requires-Dist: pandas>=2.1.2 Requires-Dist:
 requests>=2.31.0 Requires-Dist: paramiko>=3.4.0 Requires-Dist: psycopg2>=2.9.9
 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: openai>=0.27.10 Requires-Dist:
 tenacity>=8.2.3 Requires-Dist: pytest>=7.4.3
```

### Comparing `WrenchCL-1.9.0/README.md` & `WrenchCL-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/ApiSuperClass.py` & `WrenchCL-1.9.1/WrenchCL/ApiSuperClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/ChatGptSuperClass.py` & `WrenchCL-1.9.1/WrenchCL/ChatGptSuperClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/RdsSuperClass.py` & `WrenchCL-1.9.1/WrenchCL/RdsSuperClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/Utility/ConsoleAnimation.py` & `WrenchCL-1.9.1/WrenchCL/Utility/ConsoleAnimation.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/Utility/MaybeMonad.py` & `WrenchCL-1.9.1/WrenchCL/Utility/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-1.9.0/WrenchCL/WrenchLogger.py` & `WrenchCL-1.9.1/WrenchCL/WrenchLogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         stack_level_index = 1
         stack_trace = " --> InternalLogFrames"
         last_level = ""
         write_flag = False
         filepath_out, line_no_out, func_name_out, sinfo_out = self.logger.findCaller(stack_info=stack_info,
                                                                                      stacklevel=stack_level_index)
         # Loop to find the caller
-        while stack_level_index < (1000 if str(traceback.format_exc()) != "NoneType: None\n" else 10):
+        while stack_level_index < (1000 if str(traceback.format_exc()) != "NoneType: None\n" else 1000):
             filepath, line_no, func_name, sinfo = self.logger.findCaller(stack_info=stack_info,
                                                                          stacklevel=stack_level_index)
             if f"{filepath}:{func_name}:{line_no}" != last_level:
                 if self.running_on_lambda:
                     stack_trace = stack_trace + f" <-- {stack_level_index}|{os.path.basename(filepath)}:{func_name}:{line_no}"
                 else:
                     stack_trace = stack_trace + f"\n -- {stack_level_index}|{os.path.basename(filepath)}:{func_name}:{line_no}"
@@ -221,72 +221,72 @@
         self._log(level, text, stack_info)
 
         if colorama_imported or self.running_on_lambda:
             self._handlerFormat()
 
     def info(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log information that might be helpful but isn't essential."""
-        self._log_with_color(logging.INFO, text, ColoramaFore.LIGHTBLUE_EX if colorama_imported else None, stack_info)
+        self._log_with_color(logging.INFO, text, ColoramaFore.LIGHTGREEN_EX if colorama_imported else None, stack_info)
 
     log_info = INFO = info  # Aliases for info
 
     def context(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log contextual information for better understanding of the flow."""
-        self._log_with_color(21, text, ColoramaFore.CYAN if colorama_imported else None, stack_info)
+        self._log_with_color(21, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_context = CONTEXT = context  # Aliases for context
 
     def warning(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log issues that aren't errors but might warrant investigation."""
         self._log_with_color(logging.WARNING, text, ColoramaFore.YELLOW if colorama_imported else None, stack_info)
 
     log_warning = WARNING = warning  # Aliases for warning
 
     def HDL_WARN(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log warnings that have been handled and do not require further action."""
-        self._log_with_color(31, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
+        self._log_with_color(31, text, ColoramaFore.MAGENTA if colorama_imported else None, stack_info)
 
     log_handled_warning = log_hdl_warn = HDL_WARN  # Aliases for HDL_WARN
 
     def error(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that could disrupt normal program flow."""
-        self._log_with_color(logging.ERROR, text, ColoramaFore.LIGHTRED_EX if colorama_imported else None, stack_info)
+        self._log_with_color(logging.ERROR, text, ColoramaFore.RED if colorama_imported else None, stack_info)
 
     log_error = ERROR = error  # Aliases for error
 
     def data(self, data: Any, wrap_length: Optional[int] = None, max_rows: Optional[int] = None,
              stack_info: Optional[bool] = False) -> None:
         """Log Data in a lower contrast, handling formatting for readability."""
         formatted_data = self._format_data(data, wrap_length, max_rows)
         self._log_with_color(41, formatted_data, ColoramaFore.LIGHTWHITE_EX if colorama_imported else None, stack_info)
 
     log_data = print_data = DATA = data
 
     def HDL_ERR(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that have been handled but still need to be reported."""
-        self._log_with_color(42, text, ColoramaFore.MAGENTA if colorama_imported else None, stack_info)
+        self._log_with_color(42, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_handled_error = log_hdl_err = HDL_ERR  # Aliases for HDL_ERR
 
     def RECV_ERR(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log errors from which the system can recover with or without manual intervention."""
-        self._log_with_color(43, text, ColoramaFore.RED if colorama_imported else None, stack_info)
+        self._log_with_color(43, text, ColoramaFore.LIGHTRED_EX if colorama_imported else None, stack_info)
 
     log_recoverable_error = log_recv_err = RECV_ERR  # Aliases for RECV_ERR
 
     def critical(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log critical issues that require immediate attention."""
         self._log_with_color(logging.CRITICAL, text, ColoramaFore.RED if colorama_imported else None,
                              stack_info)
 
     log_critical = CRITICAL = critical  # Aliases for critical
 
     def debug(self, text: str, stack_info: Optional[bool] = False) -> None:
         """Log detailed information, typically of interest only when diagnosing problems."""
-        self._log_with_color(logging.DEBUG, text, ColoramaFore.LIGHTGREEN_EX if colorama_imported else None, stack_info)
+        self._log_with_color(logging.DEBUG, text, ColoramaFore.CYAN if colorama_imported else None, stack_info)
 
     log_debug = DEBUG = debug  # Aliases for debug
 
     # Formatting Methods
 
     def _format_data(self, data, wrap_length=None, max_rows=None, color=True, stack_trace=False):
         """Format data for logging, applying wrapping and color formatting where applicable."""
```

### Comparing `WrenchCL-1.9.0/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-1.9.1/WrenchCL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 1.9.0
+Version: 1.9.1
 Summary: This is a code library designed to improve code re-usability and standardize access to APIs, RDS, and logging functionalities
 Author: willem@wrench.ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: pandas>=2.1.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 1.9.0 Summary: This is a code
+Metadata-Version: 2.1 Name: WrenchCL Version: 1.9.1 Summary: This is a code
 library designed to improve code re-usability and standardize access to APIs,
 RDS, and logging functionalities Author: willem@wrench.ai Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Requires-Dist: setuptools>=68.0.0
 Requires-Dist: colorama>=0.4.6 Requires-Dist: pandas>=2.1.2 Requires-Dist:
 requests>=2.31.0 Requires-Dist: paramiko>=3.4.0 Requires-Dist: psycopg2>=2.9.9
 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: openai>=0.27.10 Requires-Dist:
 tenacity>=8.2.3 Requires-Dist: pytest>=7.4.3
```

### Comparing `WrenchCL-1.9.0/setup.py` & `WrenchCL-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         requires_path = os.path.join(egg_info_folder, 'requires.txt')
         if os.path.exists(requires_path):
             with open(requires_path, "r") as f:
                 required = f.read().splitlines()
 
 setup(
     name='WrenchCL',
-    version='v1.9.0',
+    version='v1.9.1',
     author='willem@wrench.ai',
     description='This is a code library designed to improve code re-usability and standardize access to APIs, RDS, and logging functionalities',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.9',
```

