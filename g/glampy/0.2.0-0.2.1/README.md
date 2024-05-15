# Comparing `tmp/glampy-0.2.0.tar.gz` & `tmp/glampy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glampy-0.2.0.tar", max compression
+gzip compressed data, was "glampy-0.2.1.tar", max compression
```

## Comparing `glampy-0.2.0.tar` & `glampy-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      696 2024-05-15 12:29:06.235592 glampy-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/__init__.py
--rw-r--r--   0        0        0     2304 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/io.py
--rw-r--r--   0        0        0     3884 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/logging.py
--rw-r--r--   0        0        0     1291 2024-05-15 12:29:06.235592 glampy-0.2.0/glampy/style.py
--rw-r--r--   0        0        0      525 2024-05-15 12:29:06.235592 glampy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 glampy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1830 2024-05-15 12:54:25.012413 glampy-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 12:54:25.012413 glampy-0.2.1/glampy/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-15 12:54:25.012413 glampy-0.2.1/glampy/io.py
+-rw-r--r--   0        0        0     3884 2024-05-15 12:54:25.012413 glampy-0.2.1/glampy/logging.py
+-rw-r--r--   0        0        0     1291 2024-05-15 12:54:25.012413 glampy-0.2.1/glampy/style.py
+-rw-r--r--   0        0        0     1108 2024-05-15 12:54:25.012413 glampy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 glampy-0.2.1/PKG-INFO
```

### Comparing `glampy-0.2.0/glampy/io.py` & `glampy-0.2.1/glampy/io.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.0/glampy/logging.py` & `glampy-0.2.1/glampy/logging.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.0/glampy/style.py` & `glampy-0.2.1/glampy/style.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.0/PKG-INFO` & `glampy-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: glampy
-Version: 0.2.0
-Summary: Make your python CLI prints and logs simple but glamorous
-License: MIT
-Author: snaeil
-Author-email: schnegel@posteo.de
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-
 # glampy
 
 This project intends to allow building useful, reliable and beautiful python CLIs with ease.
 
 ## Installation
 
 Stable release version:
@@ -28,15 +14,43 @@
 
 ```bash
 pip install git+https://github.com/snaeil/glampy
 ```
 
 ## Usage
 
-TODO:
+### Logging
+
+The customized logger can be used in it's default optionated way or can be customized.  
+It is fully compatible with the standard python logging module.
+
+```python
+from glampy.logging import Logger
+
+# Example using the Logger class to log to stdout and a file:
+logger = Logger("my_logger", log_file="my_log.log", log_level=logging.DEBUG)
+logger.debug("This is a debug message that will be logged to stdout and the file.")
+
+# Example using the Logger class to log to stdout only:
+logger = Logger("my_logger", log_level=logging.WARNING)
+logger.warning("This is a warning message that will be logged to stdout only.")
+logger.info("This is an info message that will not be logged.")
+```
+
+### Style
+
+The style module provides a simple way to style text in the terminal.  
+See [the source code](https://github.com/snaeil/glampy/blob/main/glampy/style.py) for all available styles.
+
+```python
+from glampy.style import Style, Sign, Foreground_Colour, Background_Colour
+
+# Example using the Style class to style text:
+print(f"{Sign.WARNING} The word {Style.bold}bold{Style.RESET_ALL} is not {style.italic}italic{Style.RESET_ALL}.")
+```
 
 ## Contributing
 
 Contributions are welcome!
 For feature requests, bug reports or questions, please open an issue.
 For code contributions, please open a pull request.
 
@@ -45,8 +59,7 @@
 
 ```bash
 pip install poetry
 poetry install
 cd path/to/glampy
 pre-commit install
 ```
-
```

